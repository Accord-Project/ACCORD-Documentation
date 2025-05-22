# Rule Repository Component

The purpose of this component is to provide a single repository of machine-operable building codes and rules within the ACCORD framework. This component, together with the API (2) Building Codes and Rules: 

1. Provides access to all other components of the digitised regulations in a suitable machine-readable format.
2. Provides the ability for digitised regulations to be created/updated/deleted by Rule Formalisation Tool in a frame of the Component 1 Rule Formalization.

The component is implemented as a dedicated repository aec3po running in the ACCORD GraphDB instance. The repository aec3po contains named graphs, each of which stores the digitised rules of a particular building code/ruleset. The name of such a graph should conform to the following pattern:
https://graphdb.accordproject.eu/resource/aec3po/{jurisdiction}/{classification}/{language}/{date}