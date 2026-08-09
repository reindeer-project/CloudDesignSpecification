# ADL — Architecture Description Language

ADL is an open, provider-agnostic format for describing a software system's
architecture as data.

An ADL document states what a system is made of, how the pieces connect, and —
crucially — **what the system is for**: the use cases it serves, the business
meaning behind each part, and the impact a change would have. That last part is
what source code and infrastructure templates cannot tell you, and what is
usually lost when the people who built the system move on.

Because an architecture is plain, schema-validated data rather than a diagram
file, it can be read by both people and programs: rendered as diagrams, diffed
across versions, queried for impact analysis, or handed to an AI assistant as
grounding for questions like *"if I change this database, who is affected?"*

## What is in this repository

| Path | Contents |
|------|----------|
| `ja/`, `en/` | The canonical JSON Schema for ADL, in Japanese and English |
| `index.html`, `index_ja.html` | The specification, rendered for reading — published at [docs.reindeer.tech](https://docs.reindeer.tech/) ([日本語](https://docs.reindeer.tech/index_ja.html)) |
| `resources/` | Stylesheets and scripts used by the rendered specification |
| `LICENSE` | Apache License, Version 2.0 |

The schema files are the single source of truth. Everything else in this
repository, and every copy of the schema elsewhere, is derived from them.

## Using ADL

The schema is a standard JSON Schema document, so any JSON Schema validator can
check an ADL file. Nothing in the format is tied to a particular vendor, cloud,
or tool.

## Licensing

Licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE).
