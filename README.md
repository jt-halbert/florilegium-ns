# florilegium-ns

The files that Florilegium's permanent identifiers resolve to. Florilegium is a reading workspace whose records
are W3C Web Annotations with a few properties of its own.

| Identifier | What it is | File here |
| --- | --- | --- |
| `https://w3id.org/florilegium/ns#` | The namespace of Florilegium's own terms (`fl:`) | `ns/index.html` |
| `https://w3id.org/florilegium/ns/v1.jsonld` | The JSON-LD context, version 1 | `ns/v1.jsonld` |
| `https://w3id.org/florilegium/ns/v1.ttl` | The vocabulary in Turtle (OWL 2), version 1: a label and a definition for every term | `ns/v1.ttl` |
| `https://w3id.org/florilegium/id/v1/…` | Identifiers of records in people's own places. Nothing is published at them; `404.html` says so | `404.html` |

The `w3id.org` identifiers are the ones records carry. They redirect to this repository's GitHub Pages site, and
can be pointed elsewhere later without changing any record.

## Rules for this repository

- A version of the context or the vocabulary is not edited once any record names it. New or changed terms go in
  a new version (`ns/v2.jsonld`, `ns/v2.ttl`), and old records keep naming the version they were written with.
- Version 1 is a draft until the first persisted record that names it, and is frozen from that record on. No later
  release can change what an already-used version means.
- Florilegium bundles its own byte-identical copies of these files and never fetches them. The copies and their
  SHA-256 checksums are in the application's `src/florilegium/contexts/`.
- The namespace IRI itself never changes and carries no version.

Maintainer: J.T. Halbert ([jt-halbert](https://github.com/jt-halbert)).

## License

The files in this repository are dedicated to the public domain under [CC0 1.0](LICENSE), so anyone may copy, serve
or reuse the namespace page and the context.
