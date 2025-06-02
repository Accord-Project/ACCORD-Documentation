# IDS Generation

The IDS generation tool is an experimental component developed to automatically generate IDS from the formalized building codes and rules developed within the ACCORD project. This will be useful as it provides an automated method for generating IDS files, eliminating the need for manual development by a person.

The IDS generation tool is invoked by the IDS provision component when a manually created IDS file is not available for a given building code. Upon receiving this request, it retrieves data for the building code from the Building Codes and Rules Repository and the definitions used by the building code from the data dictionary repository. It will then produce an IDS and store it in the IDS repository.

The IDS generation itself is done in three steps:

1.	Parsing the RASE embedded within BCRL documents.
2.	Generating the minimum set of data requirements needed by the given building code. This is important as certain information is only needed in certain circumstances. Thus, it would be undesirable to fail an IFC model as part of model validation processes if the data is not required for that given building. Thus, the output of this step is a list of data requirements that are always required to check a given building.
3.	Generation of IDS.
