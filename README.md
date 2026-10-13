# ontospy-examples

Example Ontology documentation auto generated via [Ontospy](https://github.com/lambdamusic/Ontospy).

See the examples: https://lambdamusic.github.io/ontospy-examples/

The source files are in [`rdf/`](rdf/), the generated documentation in [`docs/`](docs/), published with GitHub Pages. To regenerate it, from a checkout of Ontospy:

```bash
python -m ontospy.scripts.export_all -i path/to/ontospy-examples/rdf -o path/to/ontospy-examples/docs --theme stable
```

## Sources

The files added in October 2026, and where they come from (all published under open licences by their maintainers):

| File | Ontology | Source |
|---|---|---|
| `bfo-2020-core.ttl` | Basic Formal Ontology 2020 (ISO/IEC 21838-2) | [BFO-ontology/BFO-2020](https://github.com/BFO-ontology/BFO-2020) |
| `coar-resource-types.nt` | COAR Resource Types 3.2 (SKOS) | [coar-repositories/coar-vocabularies-website](https://github.com/coar-repositories/coar-vocabularies-website) |
| `dcat-ap-shacl.ttl` | DCAT-AP 3.0 SHACL shapes | [SEMICeu/DCAT-AP](https://semiceu.github.io/DCAT-AP/releases/3.0.0/) |
| `dcat3.ttl` | Data Catalog Vocabulary (DCAT) 3 | [W3C](https://www.w3.org/ns/dcat3.ttl) |
| `dcterms.ttl` | DCMI Metadata Terms | [Dublin Core](https://www.dublincore.org/specifications/dublin-core/dcmi-terms/) |
| `fibo-be.ttl` | FIBO Business Entities, merged into one file (without the regional `AllBE-*` aggregators) | [edmcouncil/fibo](https://github.com/edmcouncil/fibo/tree/master/BE) |
| `geosparql-1.1.ttl` | OGC GeoSPARQL 1.1 | [opengeospatial/ogc-geosparql](https://github.com/opengeospatial/ogc-geosparql/blob/1.1.0-ghpages/geosparql11/geo.ttl) (branch `1.1.0-ghpages`) |
| `odrl.ttl` | ODRL Information Model 2.2 | [W3C](https://www.w3.org/ns/odrl/2/) |
| `org.ttl` | The Organization Ontology | [W3C](https://www.w3.org/ns/org) |
| `prov-o.ttl` | PROV-O | [W3C](https://www.w3.org/ns/prov-o) |
| `skos.rdf` | SKOS | [W3C](http://www.w3.org/2004/02/skos/core) |
| `sosa.ttl`, `ssn.ttl` | SOSA and SSN | [W3C/OGC](https://www.w3.org/ns/ssn/) |

## Changelog

- **2026-10-13**: regenerated with Ontospy 2.5, now 32 ontologies.
    - Added widely used standards and vocabularies, see Sources above: PROV-O, DCAT 3, Dublin Core Terms, SKOS, SOSA, SSN, W3C ORG, ODRL, GeoSPARQL 1.1, BFO 2020 (replacing BFO 1.1), FIBO Business Entities, the COAR Resource Types thesaurus (SKOS) and the DCAT-AP 3 SHACL shapes, the first SHACL example.
    - Removed dated, toy or very niche ones: GOLD 2010, Countries, Koala, InstructionalObjects, Uncertainty, LiMo, Resume, EthOn, Finlex (laki) and Conflict.
    - Each ontology's namespaces section now lists only the prefixes it uses or declares, rather than all of rdflib's defaults.
- **2026-10-12**: regenerated with Ontospy 2.4, for all 30 ontologies.
    - The index page is now a table with each ontology's title, description and number of classes, properties, concepts and shapes.
    - Each ontology keeps the same Bootswatch theme across regenerations (`--theme stable`, picked from the file name), instead of a random one each time.
    - The documentation reflects the fixes in Ontospy 2.3 and 2.4, eg properties with no domain or range of their own now show those of their superproperties, property types are reported correctly (eg Pizza's `hasBase` is an `owl:ObjectProperty`, not an `owl:FunctionalProperty`), each property page lists all its types, and namespace prefixes declared in the source files are used. See the [Ontospy changelog](https://lambdamusic.github.io/Ontospy/pages/changelog.html).
- **2022-11-16**: regenerated with Ontospy 2.
- **2021-12**: new index page; RDF sources added to the repository.
- **2021-08**: first version.
