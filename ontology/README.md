# skos-ap-no ontology WIP

Referanseimplementasjon i OWL av [Forvaltningsstandard for tilgjengeliggjøring av begrepsbeskrivelser basert på SKOS (SKOS-AP-NO-Begrep)](https://doc.difi.no/data/begrep-skos-ap-no/)

Eksempel på kommandolinje verktøy for å validere rdf filer: <http://aksw.org/Projects/RDFUnit.html>

```
Jeg har lagt til en test fil "test_begrep.ttl" for å teste løsningen.

$ bin/rdfunit -d test_begrep.ttl -s BegrepShape.ttl
```

Python-basert verktøy <https://github.com/RDFLib/pySHACL>

```
$ pyshacl -s BegrepShape.ttl -m -i rdfs -f human test_begrep.ttl
```
