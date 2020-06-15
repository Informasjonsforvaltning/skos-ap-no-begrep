# skos-ap-no ontology WIP

Referanseimplementasjon i OWL av [Forvaltningsstandard for tilgjengeliggjøring av begrepsbeskrivelser basert på SKOS (SKOS-AP-NO-Begrep)](https://data.norge.no/specification/skos-ap-no-begrep/)

Eksempel på kommandolinje verktøy for å validere rdf filer: <http://aksw.org/Projects/RDFUnit.html>

```
$ bin/rdfunit -d test_begrep.ttl -s BegrepShape.ttl
```

Python-basert verktøy <https://github.com/RDFLib/pySHACL>

```
$ pyshacl -s BegrepShape.ttl -m -i rdfs -f human test_begrep.ttl
```
