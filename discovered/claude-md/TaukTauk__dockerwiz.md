---
name: TaukTauk__dockerwiz
source: https://github.com/TaukTauk/dockerwiz/blob/024e5add3dfd8b904382b710e9582a46763d0422/CLAUDE.md
repo: TaukTauk/dockerwiz
kind: claude-md
stars: 0
last_pushed: 2026-04-27T10:37:36Z
license: mit
score: 9
domains: [cli-tools, devops-automation]
tags: [python, cli, docker, architecture-first]
curated: 2026-06-16
curated_by: config-scout
---

# TaukTauk/dockerwiz — claude-md

**Why it's worth keeping:** The 'Module Dependency Rules' provide an excellent way to prevent circular imports, while highly specific naming/style conventions (e.g., `_cmd` suffixes) eliminate ambiguity in AI code generation.

**Summary:** A high-maturity configuration that bridges high-level product vision with low-level implementation constraints. It uses a structured hierarchy of scope documents and strict architectural rules.

**Source credibility:** Low social proof (0 stars), but the content demonstrates high technical maturity and sophisticated project structure.

**Recency:** Current; uses modern tech like Python 3.11, Pydantic v2, and Hatch.

**Source:** [TaukTauk/dockerwiz/CLAUDE.md](https://github.com/TaukTauk/dockerwiz/blob/024e5add3dfd8b904382b710e9582a46763d0422/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides context for AI-assisted development on dockerwiz.
Detailed documentation lives in the `scope/` directory.

---

## What is dockerwiz

A Python CLI tool that generates production-ready Docker setups through an
interactive TUI wizard. Developers run `dockerwiz new`, walk through 6 screens,
and get a complete Dockerfile, docker-compose.yml, .env.example, Makefile, and
more — tailored to their stack.

---

## Scope Documents

| File | Contents |
|---|---|
| `scope/PRODUCT.md` | Feature spec (v1.0 & v1.1), commands, stacks, services, naming, Python version |
| `scope/ARCHITECTURE.md` | Module responsibilities, dependency graph, data flow, config schema, error handling, template extensibility |
| `scope/DESIGN.md` | TUI wireframes for all 6 screens, Jinja2 template design for all output files |
| `scope/DEVELOPMENT.md` | pyproject.toml, testing strategy, versioning, CI/CD pipeline, licensing, documentation |

---

## Tech Stack

| Concern | Tool |
|---|---|
| Language | Python 3.11+ |
| TUI framework | Textual |
| CLI framework | Typer |
| Templating | Jinja2 |
| HTTP client | httpx (async) |
| Docker SDK | docker |
| Data validation | Pydantic v2 |
| Term
```

</details>
