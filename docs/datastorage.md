# Data Storage Component

The data storage component forms the central location where data that is used in the cloud-based permitting service is stored. The ‘single store multiple use’ concept is important here. Information should be stored only once to create a single source of truth and be useable and used by multiple applications. The primary use of the data storage component will be to store BIM and GIS models, along with any metadata relevant to these models.  

Two methods will be utilised to provide this storage: (1) standard static file storage, and (2) semantic storage.

- Standard static file storage. This component will store models as a single file. Access to these files will be provided via the OpenCDE Documents API. 
    - Clearly.BIM static storage has been implemented, and models can be retrieved through a protected URI. 
    - CloudPermit static storage contains the models and pre-processed Solibri BCRL rulesets. 

- Semantic Data Storage. This storage component will allow retrieval of only parts of a model. i.e. ‘give me all doors’ or ‘give me all objects related to fire safety’. 
[Graphwise GraphDB(TM)](https://graphwise.ai/components/graphdb/) is an RDF database that was chosen as a data storage created in compliance with the Semantic Web technologies stack, to adopt its best practices to serve regulation compliance checks. 
There is no open standard for retrieving only specific parts of a BIM model yet. SPARQL is utilised as a medium to provide access to BIM data in RDF. 
To store BIM data in this format, it should be converted into RDF and stored in Graphwise GraphDB. The correspondent workflow was created and tested in the [Planned Land Use Checker Microservice](./landuse.html).
