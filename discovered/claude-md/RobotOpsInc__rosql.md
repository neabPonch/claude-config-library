---
name: RobotOpsInc__rosql
source: https://github.com/RobotOpsInc/rosql/blob/cf142db72fbfe6d3a883863c693de68cbdc94d63/CLAUDE.md
repo: RobotOpsInc/rosql
kind: claude-md
stars: 2
last_pushed: 2026-06-15T00:10:46Z
license: apache-2.0
score: 9
domains: [cli-tools, compiler-development, rust]
tags: [architecture-patterns, testing-protocols, rust-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# RobotOpsInc/rosql — claude-md

**Why it's worth keeping:** It provides high-density technical context like specific testing patterns (insta snapshots), mandatory cross-backend verification steps, and a clear data-flow diagram.

**Summary:** Detailed architectural documentation that defines an 'Integrity Chain' and establishes rigorous protocols for maintaining multi-dialect compiler conformance.

**Source credibility:** High; includes highly specific toolchain commands (just, cargo-clippy) and realistic multi-dialect development constraints.

**Recency:** Current; aligns with modern Rust development standards and CI/CD workflows.

**Source:** [RobotOpsInc/rosql/CLAUDE.md](https://github.com/RobotOpsInc/rosql/blob/cf142db72fbfe6d3a883863c693de68cbdc94d63/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Canopy — Knowledge Graph

The org-wide knowledge graph is at `RobotOpsInc/canopy` (`vault/`). This repo is
documented at `vault/projects/rosql/`.

The vault slug is the repo name lowercased with underscores replaced by hyphens
(e.g. `robot_agent` → `robot-agent`, `web_app` → `web-app`).

### Read Canopy before…

* Making an architectural decision — check `vault/decisions/` and
  `vault/projects/rosql/decisions/`
* Touching a shared interface (protos, RMW API, config schema) — read the relevant
  project pages to understand what downstream repos depend on
* Investigating a regression that might be a known incident — check `vault/incidents/`

### Leave a raw note when…

When something notable happens — a decision is made, a public interface changes, a
non-obvious bug is fixed, a constraint is discovered — create a file at:

`vault/_raw/rosql-YYYY-MM-DD-<short-slug>.md`

in the `RobotOpsInc/canopy` repo and open a PR against `main`. Keep it factual: what
changed, why, any cross-repo implications. Especially for anything architectural or a
new feature, describe in detail. You can use illustrations, links, text — the ingestion
pipeline is very flexible. The canopy ingest workflow han
```

</details>
