---
name: clay-good__OpenLore__openspec-skill
source: https://github.com/clay-good/OpenLore/blob/c63daa02eb4ff7037988529316ae6b7b54c9e9b2/skills/openspec-skill.md
repo: clay-good/OpenLore
kind: skill
stars: 171
last_pushed: 2026-06-14T01:13:06Z
license: mit
score: 9
domains: [documentation-engineering, developer-tools, software-architecture]
tags: [reverse-engineering, spec-driven, drift-detection, code-archaeology]
curated: 2026-06-15
curated_by: config-scout
---

# clay-good/OpenLore — skill

**Why it's worth keeping:** The 'Archaeology over Creativity' philosophy prevents hallucinations, while the Phase 5 Drift Detection provides a concrete mechanism for maintaining architectural integrity over time.

**Summary:** A highly structured skill for reverse-engineering codebases into formal OpenSpec documentation and monitoring 'spec drift'. It creates a rigorous ground truth layer to prevent AI hallucination during long-term development.

**Source credibility:** High; the repository shows active maintenance and significant community interest (171 stars).

**Recency:** Highly current; it leverages advanced agentic workflows like drift detection that are critical for modern AI-assisted development.

**Source:** [clay-good/OpenLore/skills/openspec-skill.md](https://github.com/clay-good/OpenLore/blob/c63daa02eb4ff7037988529316ae6b7b54c9e9b2/skills/openspec-skill.md) · 171★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# OpenSpec Skill: openlore

> Reverse-engineer OpenSpec specifications from existing codebases

## Skill Metadata

```yaml
name: openlore
version: 1.0.0
description: Generate OpenSpec specifications by analyzing existing code
author: Clay Good
repository: https://github.com/clay-good/openlore
```

## Instructions

You are performing "code archaeology" — extracting the truth of what code does and documenting it as OpenSpec specifications.

### Philosophy

- **Archaeology over Creativity**: Document what the code ACTUALLY does, not what you imagine it should do
- **Evidence-based**: Every requirement and scenario must trace back to actual code
- **OpenSpec-native**: Output follows OpenSpec conventions exactly

### Process

#### Phase 1: Codebase Survey

First, understand the project structure:

1. **Identify project type** by checking for:
   - `package.json` → Node.js/TypeScript
   - `pyproject.toml` / `setup.py` → Python
   - `go.mod` → Go
   - `Cargo.toml` → Rust
   - `pom.xml` / `build.gradle` → Java

2. **Find high-value files** (prioritize these for analysis):
   - Schema/model files (entities, types, interfaces)
   - Service files (business logic)
   - Route/controller files (
```

</details>
