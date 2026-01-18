Language Definition
This section describes the Language Definition phase of the project. The main goal of this phase is to clearly define and fix the language that will be used in the Knowledge Graph, reducing ambiguity and ensuring consistency in the interpretation of concepts, properties, and relationships defined in previous phases.
This phase is essential to improve reusability and interoperability, as it establishes a shared vocabulary between the project domain, the available data sources, and the final users.
The outcomes produced during this phase are stored in the project repository as language-related resources.
Language Definition – Knowledge Layer
The Concept Identification activity focused on identifying and formalizing the concepts required to represent information in the Territory and Transportation domain, starting from the elements defined during the Purpose Definition phase.
First, the informal terms corresponding to:
entity types (etypes),
data properties,
and basic relationships
were reviewed and finalized.
The main identified concepts include Activity, Location, SkiSlope, HikingTrail, CycleRoute, ClimbingRoute, Hotel, Restaurant, SkiRental, Building, ViewPoint, and Coordinate.
Whenever possible, these terms were aligned with existing formal resources, mainly OpenStreetMap, by using its tagging system and documentation as a reference. This alignment helps reduce ambiguity and improves interoperability with external systems that rely on OSM data.
In some cases, suitable concepts were not available in general-purpose resources such as the Universal Knowledge Core or Schema.org. Domain-specific concepts like SkiSlope or HikingTrail required more precise definitions than those offered by existing vocabularies. In these cases, custom definitions were adopted, based on domain usage and OpenStreetMap documentation.
During this phase, no additional object properties were introduced. The relationships used in the model rely on standard associations and structural relations such as is-a and has-a, which are already well defined and did not require further formalization.
 Language Definition – Data Layer
At the data layer, the Language Definition phase focused on ensuring consistency between the concepts defined in the knowledge layer and the attributes present in the datasets collected during the Information Gathering phase.
In this project, most of the filtering and cleaning activities were already performed in earlier phases, when only the attributes necessary to answer the Competency Questions were selected. Therefore, no additional dataset filtering was required at this stage.
However, a review of attribute names and data types was carried out to guarantee alignment with the defined concepts. For example, common attributes such as name, difficulty, length, and elevationGain were harmonized across datasets to avoid inconsistencies.
These activities prepare the datasets for the following phases, where a more formal definition of knowledge and entities will be developed.
Evaluation – Language Definition
The evaluation of the Language Definition phase focused on assessing the coherence and adequacy of the defined language with respect to the project purpose.
Initially, a broader set of terms was considered. After review, only those terms that could be clearly aligned with formal resources or precisely defined for the project domain were retained.
Most entity types were successfully aligned with OpenStreetMap concepts, while some domain-specific terms required custom definitions. No enrichment of the Language Teleontology was necessary, as the adopted definitions were sufficient for the scope of the project.
No changes to the Purpose Definition phase were required, since the finalized language remains consistent with the previously defined scenarios, personas, and Competency Questions.
Finally, no additional dataset-level transformations were performed during this phase, as the data had already been cleaned and formatted in earlier steps. Overall, the evaluation confirmed that the defined language is consistent, reusable, and suitable for proceeding to the Knowledge Definition phase.
