# ontospy-examples

Example Ontology documentation auto generated via [Ontospy](https://github.com/lambdamusic/Ontospy).

See the examples: https://lambdamusic.github.io/ontospy-examples/

The source files are in [`rdf/`](rdf/), the generated documentation in [`docs/`](docs/), published with GitHub Pages. To regenerate it, from a checkout of Ontospy:

```bash
python -m ontospy.scripts.export_all -i path/to/ontospy-examples/rdf -o path/to/ontospy-examples/docs --theme stable
```

## Changelog

- **2026-10-12**: regenerated with Ontospy 2.4, for all 30 ontologies.
    - The index page is now a table with each ontology's title, description and number of classes, properties, concepts and shapes.
    - Each ontology keeps the same Bootswatch theme across regenerations (`--theme stable`, picked from the file name), instead of a random one each time.
    - The documentation reflects the fixes in Ontospy 2.3 and 2.4, eg properties with no domain or range of their own now show those of their superproperties, property types are reported correctly (eg Pizza's `hasBase` is an `owl:ObjectProperty`, not an `owl:FunctionalProperty`), each property page lists all its types, and namespace prefixes declared in the source files are used. See the [Ontospy changelog](https://lambdamusic.github.io/Ontospy/pages/changelog.html).
- **2022-11-16**: regenerated with Ontospy 2.
- **2021-12**: new index page; RDF sources added to the repository.
- **2021-08**: first version.
