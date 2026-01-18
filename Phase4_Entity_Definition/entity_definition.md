Entity Definition
This section describes the Entity Definition phase of the project. As in the previous phases, the goal is to report the activities performed and the results obtained. In this phase, the knowledge layer and data layer are merged, resulting in a single, structured Knowledge Graph that integrates both the teleontology and the aligned datasets.
The Entity Definition phase focuses on identifying entities, mapping data values to the knowledge structure, and resolving heterogeneity across datasets.
OVERVIEW AND OBJECTIVES:
The Entity Definition phase represents the final integration step of the iTelos methodology. The inputs for this phase are:
the teleontology defined during the Knowledge Definition phase,
the cleaned and formatted datasets collected during the Information Gathering phase.
The main objective is to create a unified Knowledge Graph by mapping real-world data values to the corresponding entity types, properties, and relationships defined in the teleontology. This phase addresses heterogeneity at both schema and data levels and ensures that entities are consistently represented across datasets.

ENTITY IDENTIFICATION AND DATA MAPPING (SINGLE DATASET):
For each dataset, entity identification and data mapping were performed by merging the knowledge structure of the corresponding entity type with the data values contained in the dataset.
Each dataset in the project mainly corresponds to a single entity type (e.g., SkiSlope, HikingTrail, CycleRoute, Hotel, Restaurant, ViewPoint). This simplified the mapping process, as no complex reconciliation between multiple datasets representing the same entity type was required.
Whenever data was derived from OpenStreetMap, the osmId attribute was preserved and used as a stable identifier. This decision improves reusability and interoperability with external systems that rely on OSM identifiers. For entities not fully supported by OSM schemas, project-specific identifiers were created to ensure uniqueness.

ENTITY IDENTIFICATION AND DATA MAPPING (MULTIPLE DATASETS):
In some cases, multiple datasets contributed to a single conceptual structure. For example, activities such as ski slopes or hiking trails required the combination of geometric data (paths and coordinates) with descriptive attributes (name, difficulty, length).
In these cases, data mapping was performed by aligning all datasets to the same entity definition in the teleontology, ensuring that attributes from different sources were consistently integrated into a single entity representation.
The mapping process was carried out using Karma, which allowed the association of dataset attributes to entity types, object properties, and data properties defined in the knowledge layer. The output of this process consists of RDF mappings that generate the final Knowledge Graph.

PHASE OUTCOMES:
The main outcome of the Entity Definition phase is a structured and integrated Knowledge Graph that combines:
the conceptual structure defined in the teleontology,
the real-world data values collected from multiple datasets.
The resulting KG supports the previously defined Competency Questions and provides a consistent representation of activities, locations, and services within the Trentino region.

DECISIONS, STRENGTHS, AND WEAKNESSES:
During this phase, several design decisions were made.
Entity mapping was performed primarily on leaf entities (e.g., SkiSlope, HikingTrail, CycleRoute, Hotel, Restaurant, ViewPoint), as these entities directly support the Competency Questions. Superclasses such as Activity, Location, and Building were retained in the teleontology to support inheritance and future extensibility, but they were not directly populated with data values.
Strengths:
The use of osmId improves reusability and alignment with external resources.
The separation between common, core, and contextual entities results in a clean and user-oriented KG structure.
The teleontology supports future extensions without requiring major restructuring.
Weaknesses:
Some datasets contain limited or incomplete information, which restricts the level of detail for certain entities.
Not all Competency Questions can be fully answered due to data availability constraints.

EVALUATION – ENTITY DEFINITION:
The evaluation of the Entity Definition phase focused on assessing the completeness and consistency of the resulting Knowledge Graph.
Initially, a larger number of entities and properties were considered. After evaluation, only those entities that could be reliably populated with available data were retained in the final KG. All retained entities were successfully modeled and mapped.
No major changes were required in the Purpose Definition, Language Definition, or Knowledge Definition phases as a result of this phase. Minor dataset-level formatting and normalization were performed to ensure compatibility with the teleontology and to support the mapping process.
Overall, the Entity Definition phase successfully produced a coherent and reusable Knowledge Graph that integrates knowledge and data layers and fulfills the project purpose.
