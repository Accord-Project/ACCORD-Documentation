# Eurocode Verification

This microservice has been developed to perform structural compliance checks on building construction elements in accordance with the Eurocodes, a comprehensive set of design standards that govern the structural integrity of the built environment throughout most European countries. Its implementation leverages structural-analysis-related IFC data and requires that structural analysis model results be available for each applicable verification check.
In the absence of such analysis results, the specialized open-source tool IFC2CA  can be utilized to conduct the structural analysis of IFC building models using the Finite Element Method (FEM). The FEM engine employed is Code_Aster, a robust finite element solver developed by EDF (Électricité De France) and validated in the nuclear sector. 

The tool operates on the IFC data and provides three primary high-level functionalities:

1. Mesh Generation: Creation of a discretized numerical model (mesh) for a given IFC structural analysis model.
2. Analysis Execution: Generation of a Code_Aster-specific input file incorporating the model properties, load specifications, and configuration parameters necessary for the analysis.
3. Data Enrichment: Enhancement of the original IFC model with corresponding analysis responses, including internal forces, displacements, and reactions for each associated IFC entity.

These enriched IFC result data are then employed to carry out structural design verifications in full compliance with the relevant design standards.

The microservice is built around an API developed in Python and integrated with the ACCORD Results API . This integration enables its use with the core components of the ACCORD system via Integration Strategy A, using the Eurocode-based Ruleset.

The required input for this service comprises an IFC file, accessed through the Data Storage Component, and the GlobalId of a structural analysis model that contains the necessary analysis results. Upon processing these inputs, the system generates a comprehensive data dictionary for each structural member within the model, indexed by its GlobalId. This dictionary encapsulates all verification parameters needed for every applicable check.

Designed to streamline the validation process, the API facilitates a standardized workflow that includes:

1. Target Type Applicability Validation: Confirming that a specific target type, as a feature of interest, is applicable to a given structural member.
2. Verification Parameter Check: Ensuring that all required verification terms have been computed.
3. Compliance Check Generation: Producing the identified structural compliance verifications based on the enriched analysis data.

It is important to note that the implementation relies on predefined property sets that include properties for materials, cross-sections of uniform members and required design coefficients for structural verifications. The existence of these property sets is checked in the IDS validation phase, but the values themselves are not part of the current Eurocode-based Ruleset. Nonetheless, all required data are captured within the IFC file with applicable templates, and this setup can be readily extended for such checks via the Integration Strategy A.
