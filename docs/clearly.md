# Future Insight Clearly.BIM 

Clearly.BIM is a user-friendly online solution for storing, viewing, sharing, querying, and checking BIM models in IFC. It offers a scalable solution for whoever works with BIM models: municipalities, contractors, the fire department, building owners, housing corporations, etc.  

Clearly.BIM's main capabilities are: 
- Storing IFC models in an online database (fulfils the Data Storage Component) 
- Viewing and interacting with the model in detail.  
- Sharing the BIM models within an organization or between organizations. 
- Streaming BIM models in 3D Tiles to be used directly in 3D City Models or other 3D visualizations. 
- Exporting BIM models in various formats. 
- Executing IDS checks. (Model and Data Requirement Validation Component and subject to the Orchestrating Microservices Component) 
- Executing compliance checks for Building Code or Zoning Plan rules (subject to the Orchestrating Microservices Component) 
- Publishing check results in BCF. 

Clearly.BIM is fully API based. All functionalities are also available through OpenAPI and GraphQL endpoints and can be easily integrated in other software systems. Through these APIs Clearly.BIM is subject to the Process Execution Component and Orchestrating Microservices Component  
In the ACCORD project and in the integration with the ACCORD Architecture, Clearly.BIM is used through API and less through its UI.  

For the Estonian use case in ACCORD, Clearly.BIM has been mainly used for storing BIM models and executing various checks from the Estonian Building code. These functionalities have been implemented through API in: 
- The Estonian Building Registry (EHR / e-ehitus) 
- The draft Process Execution Component 
- The draft Orchestrating Microservices Component  

The general flow that Clearly.BIM executes in this use case is as follows: 
- A BIM model is uploaded by the end user (e.g. a permit applicant) directly in the Clearly.BIM web application and/or in the external interface (in this case of the Estonian Building Registry) as an IFC file. 
- Through API this IFC file is sent to and imported in the Clearly.BIM database, which is based on BIM.works.  
- From the database, the model is directly viewable and queryable in the Clearly.BIM web application and/or external interface. 
- Through API, both IDS and compliance checks (building code or zoning plan) can be initiated. 
- Many different checks were configured, but the initiation process is the same. 
- The results of the checks are provided in both JSON and BCF.  
