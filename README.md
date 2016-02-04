# Rare-Disease-Semantic-Model

This folder contains the ontologies that together form a semantic model for data that the RD-Connect platform wishes to connect. 

DISCLAIMER: work in progress!!
ToDo: 
1. complete for all identifiers in the identifier table
complete mappings and update extended model
2. check with other ontology experts
3. improve
4. back to 2 a few times
5. map to example data / ‘virtualize’ the model

Note that the model defines classes, the data in the various sources that are supposedly accessed via the platform represent the instances or the values for the datatypes. 

Ontologies:
1. rdc-core: the minimal set of classes and properties to map to the data in the sources of the platform. Because of the task at hand the focus is on identifiers. RD core represents little more that the lowest level types of the identifiers.
2. rdc-meta: the actual semantic model, defined as much as possible using existing ontologies (OBIB, etc.).
3. rdc-meta-extended: this model includes the subclasses and properties of the entities that were imported from source ontologies, i.e. when you use the ‘move’ function of protege, rather than just copy the URI.
4. rdc-thesaurus: mappings to ‘concepts’. A SKOS-based thesaurus represents a ‘light-weight’ ontology. This allows us to define in simple terms the relations between similar or equal terms in different terminologies. Thesaurus: focus on how we call things; Ontology: define what things are. 
5. rdc-mapping: mapping between models, for instance between the SKOS concepts and RD-core and RD-meta.
6. rdc-example-instances: example instances (‘individuals’) to show the model at instance level. The instances, especially the IDs relate to actual data. Their datatype properties link to data. Rajaram is working on virtualizing this.

Other files:
1. classes.png: shows the class tree
2. individuals_ontograf.png: shows a graph of the example instances (individuals)

Especially core and meta should be taken together to form a semantic model with sufficient relations.
