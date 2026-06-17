---
name: lance-format__lance-namespace
source: https://github.com/lance-format/lance-namespace/blob/590a4eb7163a85f56e0622f9359efa33d5ad6941/CLAUDE.md
repo: lance-format/lance-namespace
kind: claude-md
stars: 55
last_pushed: 2026-06-12T17:19:59Z
license: apache-2.0
score: 8
domains: [infrastructure, multi-language, data-formats]
tags: [architecture-diagrams, cross-language, build-automation]
curated: 2026-06-15
curated_by: config-scout
---

# lance-format/lance-namespace — claude-md

**Why it's worth keeping:** The Mermaid diagram explains intricate dependency directions across Rust/Python/Java, and the component table provides precise path mappings that help an AI navigate the repo structure.

**Summary:** Provides deep architectural context for a multi-language specification project, detailing complex cross-repo dependency chains.

**Source credibility:** High; part of the active Lance data format ecosystem with recent maintenance.

**Recency:** Current; last pushed 0 months ago.

**Source:** [lance-format/lance-namespace/CLAUDE.md](https://github.com/lance-format/lance-namespace/blob/590a4eb7163a85f56e0622f9359efa33d5ad6941/CLAUDE.md) · 55★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Contributing to Lance Namespace

The Lance Namespace codebase is at [lance-format/lance-namespace](https://github.com/lance-format/lance-namespace).
This codebase contains:

- The Lance Namespace specification
- The core `LanceNamespace` interface and generic connect functionality for all languages except Rust
  (for Rust, these are located in the [lance-format/lance](https://github.com/lance-format/lance) repo)
- Generated clients and servers using OpenAPI generator

This project should only be used to make spec and interface changes to Lance Namespace,
or to add new clients and servers to be generated based on community demand.
In general, we welcome more generated components to be added as long as 
the contributor is willing to set up all the automations for generation and publication.

For contributing changes to directory and REST namespaces, please go to the [lance](https://github.com/lance-format/lance) repo.

For contributing changes to implementations other than the directory and REST namespace, 
or for adding new namespace implementations,
please go to the [lance-namespace-impls](https://github.com/lance-format/lance-namespace-impls) repo.

## Project Dependency

This p
```

</details>
