# Building Codes and Rules Repository

The purpose of this component is to provide a single repository of machine-operable building codes and rules within the ACCORD framework. This component, together with the API (2) Building Codes and Rules: 

1. Provides access to all other components of the digitised regulations in a suitable machine-readable format.
2. Provides the ability for digitised regulations to be created/updated/deleted by Rule Formalisation Tool in a frame of the Component 1 Rule Formalization.

The component is implemented as a dedicated repository `aec3po` running in the ACCORD GraphDB instance. 
The repository `aec3po` contains named graphs, each of which stores the digitised rules of a particular building code/ruleset. 

The regulation graphs obtained within the Rule Formalisation Tool in the form of [JSON-LD](https://json-ld.org/) files are uploaded to Graphwise GraphDB(TM) via REST API provided by GraphDB Workbench. The full description of Graphwise GraphDB(TM) REST API abilities is given at the link [https://graphdb.accordproject.eu/graphdb/webapi](https://graphdb.accordproject.eu/graphdb/webapi). 

JSON-LD is a lightweight Linked Data format. It is easy for humans to read and write. It is based on the JSON format and provides a way to help JSON data interoperate at Web-scale.

A dedicated repository https://graphdb.accordproject.eu/graphdb/repositories/aec3po keeps all the versions of regulation graphs created for a particular building code. 

[Building Codes and Rules API](https://accord-project.github.io/API-Development/buildingcodesandrules.html) is created to communicate rules from Graphwise GraphDB(TM) to other components. 

## Regulation graph naming conventions
The general scenario is one where the graph version of the regulation is published on the same day as the official publication of the regulation in PDF format. The user can define this date manually. For example, a retrospective scenario where a graph is published months or years after a regulation is officially published.

If someone realises that the graph is wrong, a new one must be generated as a different version. Both must be kept. The publication date of the second graph reflects the date the change is made officially: it will contain the publication date of when the new version of the graph is made public (different from the publication date of the PDF). 
URI pattern for regulation graphs is: 
`https://graphdb.accordproject.eu/resource/aec3po/{jurisdiction}/{classification}/{language}/{date}`

Example:
```
https://graphdb.accordproject.eu/resource/aec3po/FI/CO2/en-gb/2024-07-03  
```
To access this graph interactively, you need a login and password, then you can access this URL:
```
https://graphdb.accordproject.eu/graphdb/resource?uri=https:%2F%2Fgraphdb.accordproject.eu%2Fresource%2Faec3po%2FFI%2FCO2%2Fen-gb%2F2024-07-03&role=context  
```