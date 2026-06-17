---
name: webrpc__webrpc
source: https://github.com/webrpc/webrpc/blob/d6d55ddb93ef824e07efd4a0ea6f520adaf690ed/SKILL.md
repo: webrpc/webrpc
kind: skill
stars: 828
last_pushed: 2026-06-08T21:48:04Z
license: mit
score: 9
domains: [backend-api, codegen, schema-design]
tags: [ridl, webrpc, api-schema]
curated: 2026-06-15
curated_by: config-scout
---

# webrpc/webrpc — skill

**Why it's worth keeping:** It utilizes high-value 'Do/Don't' lists and a dedicated 'Common mistakes' section to prevent hallucinated syntax; it also provides specific field metadata patterns crucial for code generation tasks.

**Summary:** Defines the RIDL syntax and structural constraints for creating schema files used by the webrpc framework.

**Source credibility:** High; the source repository is active, well-maintained, and follows professional schema standards.

**Recency:** Current; the syntax rules are highly specific to contemporary schema-driven development.

**Source:** [webrpc/webrpc/SKILL.md](https://github.com/webrpc/webrpc/blob/d6d55ddb93ef824e07efd4a0ea6f520adaf690ed/SKILL.md) · 828★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: webrpc-ridl-schema
description: webrpc schema and RIDL syntax
---

# webrpc schema and RIDL syntax skill for LLMs

## When to use this skill
Use this skill when the user needs to work with RIDL files.

The RIDL file defines schema for HTTP client/server communications (browser-to-server or service-to-service).
The `webrpc-gen` codegen generates a REST-like API with JSON messages, a subset of REST API conventions, which:
- is not RESTful
- always uses POST method
- uses JSON body only (no path params or query params)

## Do and don't
- Prefer editing `.ridl` files; do not manually edit generated `*.gen.*` files.
- Keep syntax strict: identifiers are case‑sensitive; spacing is mostly flexible.
- Use `ridlfmt` after edits when possible.
- Prefer succinct method signatures for request/response structs.
- Avoid mixing succinct and multi‑arg method signatures.
- Don't use circular imports.

## Schema header (required)
```
webrpc = v1
name = <schema-name>
version = <schema-version>
basepath = <api-base-path>
```

## Imports
```
import "path/to/file.ridl"
import "path/to/file.ridl" (TypeA, ServiceB)
```
Imports are merged into the current schema and can be limited to named member
```

</details>
