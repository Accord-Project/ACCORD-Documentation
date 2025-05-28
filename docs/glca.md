# Environmental Compliance

This microservice facilitates the checking of environmental compliance with the DGNB green building certification requirements. It builds on a service setup using web-based building LCA tools that create and submit an XML building LCA model to DGNB direct submission API for compliance checking and performance point calculation based on DGNB requirements on building LCA models as defined in the DDNB requirement specification DNG 1.1. 
The model can build on IFC but needs to be translated to XML and to be enriched to be checked by DGNB. The XML schema definition and a test API are provided by DNGB upon request.

The microservice builds on the DGNB API for environmental compliance checking, point calculation and result submission. The requesting agent is a building LCA web software such as Generis®, where users can create building LCA models aiming at environmental compliance with DGNB certification requirements. The models are directly submitted via API (as specified by DGNB; XSD, API link and documentation are available upon request) and checked against LCA calculation rules, model consistency, and environmental performance achievement. 
 
Within the Generis® microservice, the following services are provided: 

1. Model/Data requirement validation through quality and compliance pre-checking routines
2. Building LCA model creation and manipulation
3. Data storage on building and construction level
4. Data export and direct model submission via API
