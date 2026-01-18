Knowledge Definition
The Knowledge Definition phase represents a key step in the iTelos methodology, as it aims to formalize the knowledge structure of the project by using the language terms defined in the previous phase. The objective of this phase is to define a coherent knowledge model (teleology) and align the collected datasets with this structure in order to build the Knowledge Graph.
This phase includes activities at both the knowledge layer and the data layer, focusing on ontology composition, alignment with reference ontologies, and dataset adaptation. The results of this phase are stored in the project repository.
Knowledge Layer

TELEOLOGY DEFINITION:
The teleology of the project was defined by composing and adapting ontology fragments relevant to the Territory and Transportation domain. The teleology reflects the conceptual structure identified during the Purpose Formalization phase and follows the Entity–Relationship model previously defined.
The core of the teleology is built around the entities Activity and Location, which represent the main entry point of user queries and their spatial context. These entities serve as the foundation upon which more specific concepts are structured.
Activity is specialized into contextual entities such as SkiSlope, HikingTrail, CycleRoute, and ClimbingRoute, each representing a specific type of outdoor activity and inheriting common characteristics from the Activity concept.
Location is connected to Coordinate, which models geographic positioning, and is extended by core entities such as Hotel, Restaurant, SkiRental, and Building, representing services associated with activities and locations.
This structure allows the teleology to remain simple and reusable, while still supporting detailed representations of domain-specific activities and services

KNOWLEDGE TELEONTOLOGY ALIGNMENT:
After defining the teleology, the identified entity types, object properties, and data properties were aligned with concepts from existing reference ontologies whenever possible. OpenStreetMap ontology fragments were used as the primary reference, as most entities in the project are derived from OSM data.
Common concepts such as Location, Building, Restaurant, and Hotel could be aligned with existing OSM definitions. However, some domain-specific concepts such as SkiSlope, HikingTrail, and ClimbingRoute are not explicitly defined in the provided ontology fragments. In these cases, project-specific entity types were defined while preserving compatibility with OSM through the use of attributes such as osmId.
No major extensions of the reference knowledge teleontology were required. Instead, the teleology was composed by combining existing ontology fragments and adding minimal custom elements strictly necessary to support the project purpose.
Data Layer
At the data layer, datasets collected during the Information Gathering phase were cleaned and formatted to follow the structure defined in the knowledge layer.
Each dataset was aligned with the corresponding entity type by:
selecting only attributes relevant to the teleology,
harmonizing attribute names and data types,
ensuring consistency across datasets.
For example, activity-specific datasets (ski slopes, hiking trails, cycle routes, climbing routes) were aligned with the Activity structure, while service-related datasets were aligned with Building, Hotel, Restaurant, and SkiRental entities. Geographic information was normalized using the Coordinate entity.
No major restructuring of datasets was required at this stage, as most datasets had already been filtered and simplified in previous phases.
Evaluation - Knowledge Definition
The evaluation of the Knowledge Definition phase focused on assessing the coherence and completeness of the defined teleology and its alignment with available data.
Initially, a broader set of entity types and properties was considered. After evaluation, only those entities that could be reliably supported by the collected datasets were retained. Most entity types could be aligned with OpenStreetMap ontology fragments, while a limited number of project-specific entities were defined to cover domain-specific concepts.
Only a small number of object properties were required, mainly to represent relationships between activities, locations, and services. These properties could be aligned with existing ontology patterns and did not require extensive customization.
All data properties used in the teleology were successfully supported by the datasets, although some attributes were simplified due to data availability limitations.
No changes to the Purpose Definition or Language Definition phases were required as a result of this evaluation. Dataset-level cleaning and formatting were confirmed to be sufficient for supporting the defined teleology.
Overall, the Knowledge Definition phase resulted in a coherent and reusable knowledge structure that aligns with the project purpose and provides a solid foundation for the subsequent Entity Definition and Metadata phases.


