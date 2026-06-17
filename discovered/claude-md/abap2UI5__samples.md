---
name: abap2UI5__samples
source: https://github.com/abap2UI5/samples/blob/8b5ec8a4500af417d932861c13c5bf40ceac7108/CLAUDE.md
repo: abap2UI5/samples
kind: claude-md
stars: 53
last_pushed: 2026-06-11T10:56:52Z
license: mit
score: 9
domains: [backend, erp, abap]
tags: [coding-standards, framework-guide, structural-rules]
curated: 2026-06-15
curated_by: config-scout
---

# abap2UI5/samples — claude-md

**Why it's worth keeping:** It uses granular structural constraints (e.g., exact blank line counts) to enforce consistency; provides a technical 'cheat sheet' of the framework's lifecycle and methods essential for domain-specific reasoning.

**Summary:** Defines hyper-specific ABAP coding standards, including precise whitespace rules and linting requirements, alongside a detailed framework API reference.

**Source credibility:** High; part of an active, specialized open-source project.

**Recency:** Very recent/current.

**Source:** [abap2UI5/samples/CLAUDE.md](https://github.com/abap2UI5/samples/blob/8b5ec8a4500af417d932861c13c5bf40ceac7108/CLAUDE.md) · 53★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project

abap2UI5 Samples - Collection of demo apps for the abap2UI5 framework.

## Language

- **This entire project is in English.** All code, comments, commit messages, PR titles, PR descriptions, and any other text must be written in English.

## Rules

### abaplint

- **Run `abaplint` before every commit. It must report 0 issues.**
- Configuration: `abaplint.jsonc`
- Install: `npm install -g @abaplint/cli`
- Run: `abaplint`

### abapGit file consistency

All serialized files (`.abap`, `.xml`, and any other abapGit-managed file types) must conform to the abapGit file format:
- **Encoding**: UTF-8 (with optional BOM: `xEF BB BF`)
- **Line endings**: LF (`x0A`) only — never CRLF
- **Final newline**: every file must end with a single newline character after the last line
- **Indentation**: 2 spaces — never tabs

**Always verify consistency for all file types before committing**, not just `.abap` files. abaplint covers `.abap` files; for `.xml` and other files, check manually or via editor tooling that the above rules are met.

### Code Conventions

- Follow the [SAP ABAP Style Guide](https://github.com/SAP/styleguides/blob/main/clean-abap/CleanABAP.md).
- Never use
```

</details>
