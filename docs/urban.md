# Urban Regulations

## 1. General Microservice Description
The purpose of the microservice that implements the regulation of urban planning parameters is to automate the process of checking the compliance of building project proposals – for new construction buildings and the renovation of existing buildings – with the urban parameters defined in municipal urban planning plans. This type of check is typically conducted by municipal technicians in city or town councils in countries such as Spain.

## 2. Microservice Implementation and Functionality
This microservice is composed of four parts, each of which is executed in a specific execution order, as shown in Figure 12. 

All the parts have been implemented using Python language and Django, a high-level Python web framework, for their deployment on a server. The source code is available on GitHub . The inputs for this microservice are a BIM model (in IFC format) and a cadastre file (in GML format).

<b>Pre-processing process:</b> This process enriches the data in the cadastre input files with the necessary information so that it can be properly processed by the Urban Regulations checker microservice, as well as removing data that is not necessary. This service is executed only once to generate this information for each cadastre input file. 

<b>IFC Data Requirements Checker:</b> This part is responsible for checking that the BIM of the building project complies with the data requirements necessary to ensure that the part for checking compliance with urban planning regulations is executed. These data requirements are provided in a file specified in the IDS standard format.

<b>Parcel Shape Checker:</b> This part checks if the perimeter of the parcel provided in the cadastre file coincides with the parcel's perimeter specified in the building project's BIM.

<b>Urban Regulation Checker:</b> This part checks that the building project complies with urban planning parameters defined in the municipal urban planning plans. To perform the checking, data from four different sources are required: (1) Cadastre data, (2) Topographic data, (3) urban data, and (4) project data provided in a BIM model represented in the IFC standard. 

The functions of this microservice are exposed to the ACCORD core components via an implementation of the Results API. 

## 3. Comparison against Relevant Technical Requirements
A comparison of the implemented functionality of this compliance-checking microservice and the relevant technical requirements defined in D4.1 is given in Table 18.
Table 17. Urban Regulations - Comparison against Technical Requirements

| TR No	| Requirement Description	| Implementation Detail | 
|-------|-------------------------|-----------------------|
| 68	| The system's checking of compliance with urban regulations must be automated. The permitting process will be applicable to both public and private buildings during the design and construction phases, using BIM and GIS as data input. 	| This microservice implements the urban regulation checking as described above. | 
|69|The system must allow to integrate GIS- and BIM data to carry out checking against urban regulations using one unified model.|As part of the pre-processing and parcel shape checking elements of this microservice, the GIS and BIM data are integrated for the purposes of compliance checking.|






