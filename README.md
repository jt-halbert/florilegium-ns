# florilegium-ns

The files that Florilegium's permanent identifiers resolve to. Florilegium is a reading workspace whose records
are W3C Web Annotations with a few properties of its own.

| Identifier | What it is | File here |
| --- | --- | --- |
| `https://w3id.org/florilegium/ns#` | The namespace of Florilegium's own terms (`fl:`) | `ns/index.html` |
| `https://w3id.org/florilegium/ns/v1.jsonld` | The JSON-LD context, version 1 | `ns/v1.jsonld` |

The `w3id.org` identifiers are the ones records carry. They redirect to this repository's GitHub Pages site, and
can be pointed elsewhere later without changing any record.

## Rules for this repository

- A context version is not edited once Florilegium has written records that name it. New terms go in a new
  file (`ns/v2.jsonld`), and old records keep naming the version they were written with.
- Version 1 is a draft until the first Florilegium release that writes it into records; it is frozen from then on.
- The namespace IRI itself never changes and carries no version.

Maintainer: J.T. Halbert ([jt-halbert](https://github.com/jt-halbert)).
