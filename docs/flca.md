# AC(CO2)RD whole life carbon assessment

AC(CO2)RD is a Proof-of-Concept microservice that automatically extracts information from the IFC model and relevant environmental databases, combines them, and generates a Life Cycle Assessment (LCA) report without requiring user interaction. For the project purpose, only the Global Warming Potential (GWP) category is used, and the results are expressed in kgCO2e. The process is designed to overcome barriers caused by insufficient or mismatched data in the model and/or databases by automatically generating conservative assumptions and providing feedback to the designer on areas of the model that can be improved.

The AC(CO2)RD microservice is an open-source Python tool developed on the ifcopenshell platform, including ifctester and ifcopenshell.validate modules for the input validation.
The following inputs are used by the tool:

1. STEP Physical file (IFC 2X3 to IFC 4.3) together with optional additional information in JSON format,
2. JSON file with material quantities and additional building information 

The AC(CO2)RD microservice can retrieve LCA information about the building materials and products from different databases using HTTP calls:

1. Finnish Emissions database for construction via CO2data service at co2data.fi,
2. ILCD+EPD standard databases such as environdec.com.

In addition to responding to compliance checks via the results API, the tool has the following file based output options in JSON or Microsoft Excel:

1. LCA report (minimum report with the overall whole life carbon footprint of the model, standard LCA report according to EN 15978 (Sustainability of Construction Works), or full report with all the calculation results of each LCA stage by material, by type and by entity) in tonnes of CO2e,
2. Material report (bill of materials, or material flows report including the recycling rates and recycled content) in tonnes, square meters or cubic meters of each material,
3. Environmental declaration according to the Finnish Decree on Climate Declaration in kgCO2e/sqm of heated area.


The microservice is based on two basic principles: (1) The calculation shall be fully automated and (2) in the case of any uncertainties, the most conservative results shall be produced. The specific mechanisms how this is achieved are described in the following sections:
Selection of the appropriate entities: All the model data (all entities represented by 3D geometry) may not apply to the LCA calculation. For instance, the building regulations are restricted only to certain product groups. The conservative approach is to calculate the impact of each entity unless it can be explicitly excluded from the assessment. The exclusion of certain IFC entities can be specified in the accompanying JSON file.
Missing information about the material: In certain cases, the entities may not have associated materials, or the material names may be ambiguous (“Undefined”, “Default”, etc.). The tool assumes conservative values of CO2 emissions for such entities as the highest possible value in the database for a certain product class.

Material not matching the records in the environmental database: In a common design practice, the only information about the material in the permitting phase is its name assigned by the designer, the BIM authoring tool, or its template. This name is typically not pointing directly to any specific record in the environmental database. The tool, therefore, uses an extensive mapping dictionary of common material names linked to the Finnish national database. If the material name is not in the dictionary, the tool automatically uses conservative emissions for this material.

Missing information about the quantities: Environmental data is typically related to a certain unit flow, for instance, mass, volume, surface area or just the number of products. The relevant quantities must be recognisable from the model. The tool mainly relies on quantities stored in the IFC file, but if the information is not found in the model, a thorough search of all element properties is performed. The last option is to calculate the quantities directly from the model geometry to ensure a conservative result is delivered in any situation.  The tool uses bounding boxes of the elements to optimise the performance of the calculation, but other methods (such as tetrahedral meshing) may be implemented in the future if they ensure conservative results and reasonable computational time.
Missing entities: During the permitting stage, verifying whether the designer has provided a digital model of all components required for the compliance check is impossible. Therefore, in this case, the tool cannot guarantee the conservativeness of the calculated results. 
