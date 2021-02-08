# SKOS-AP-NO-Begrep - shacl

This folder contains validation rules for SKOS-AP-NO-Begrep, as shacl-shapes.

About the current version of the shacl-file:
* Except for the 'concept relations', all relevant shapes are included, i.e., also shapes for optional properties and for usage of permitted values.
* sh:targetObjectsOf is used for skos:Concept, in order to avoid validating of imported skos:Concept. However, as a consequence, skos:Concept which is not an object in a triple (e.g., as a skos:member, or referred to by dct:replaces/dct:isReplacedBy etc.) will not be validated.
