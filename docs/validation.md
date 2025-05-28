# Model and Data Requirement Validation Component


The Model and Data Requirement Validation Component ensures that the building model (IFC) and additional information (i.e., GIS data sets or supporting product data) that is to be checked on regulation compliance is of a good enough quality to be subject to such checks. 

It is common that many BIM models lack the required detail, structure or information that is needed to execute detailed regulation compliance checks. For example, it is still common practice in the construction sector for supporting information to remain in PDF documents and not be transferred into building models.  As this might result in false positives or negatives and thus misleading results, the Model and Data Requirement Validation Component executes several gatekeeper checks, which can be roughly split into three parts:

1. Validation of IFC Models on IFC validity: Will ensure any IFC models provided to the ACCORD Cloud Architecture are valid IFC models with regards to one of buildingSMART’s published schemas. This is required because any invalid models will not be able to be parsed and understood by ACCORD components.
2. Validation of IFC Models against IDS specifications: Will ensure that IFC models provided to the ACCORD Cloud Architecture meet the requirements of the required IDS files. This is required to ensure that sufficient information is present in the IFC file to allow compliance checking against it to take place.
3. Validation of additional GIS Data: Will ensure that any submitted GIS data conforms to agreed GIS specifications and profiles.



The implementation and functionality of the Model and Data Validation Component will be further described based on its four subcomponents.

Validation of IFC Models on IFC validity: BuildingSMART has been offering their IFC Validation tool , which offers:

1. STEP Syntax checks: The STEP Physical File syntax
2. IFC Schemac checks: An up-to-date (not withdrawn and latest revision) IFC schema referenced in the file, including formal propositions and functions encoded in the EXPRESS schema language
3. Normative IFC Rules checks: Other normative rules of the IFC specification (e.g. implementer agreements and informal propositions)
4. Additionally: Industry Practices: Checking the IFC file against common practice and sensible defaults. None of these checks render the IFC file invalid. Therefore, any issues identified result in warnings rather than errors
5. Additionally: bSDD Compliance Checking whether references to classifications and properties from bSDD, found in an IFC file, comply with the source definitions in bSDD

In order to integrate the buildingSMART IFC Validation tool, a preview version of the IFC Validation Service API (REST) has been developed. The API performs all of the checks mentioned above. After some initial authentication issues, it has been successfully tested using the orchestrator component (in this case, FME).

Results are returned as a list of all validation outcomes, optionally filtered by request_public_id or validation_task_public_id in JSON. 

Validation of IFC Models against IDS specifications: For implementation of IDS validation we made the assumption that a valid IDS was provided. Creating valid IDS was thus out of the scope of this implementation, which solely focused on executing IDS checks as part of the ACCORD Architecture Framework.

For IDS checking, two tools have been used: 

1.	Solibri Cloud Checking: IDS checks for Solibri are stored in cset files and can be invoked through the Solibri Cloud Checking API (Solibri Checking as a Service).  Any cset file can be provided as payload to the API using an array of URIs.
This has been successfully tested using the orchestrator component (in this case FME) and returns the check results both directly in JSON or in BCF (1.0, 2.0, 2.1 or 3.0).
2.	Clearly.BIM: IDS checks for Clearly.BIM have to be configured in the Clearly.BIM backend and can be invoked through API based on their checkUuid . It is not yet possible to dynamically provide an IDS definition as payload to the API. 
This has been successfully tested using the orchestrator component (in this case FME) and returns the check results both directly in JSON or in BCF.
