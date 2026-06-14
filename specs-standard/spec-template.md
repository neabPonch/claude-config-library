---
id: NNNN
title: <short title>
type: spec
status: draft            # draft | active | shipped | archived | superseded
prd: NNNN-slug.prd.md     # link back to the PRD
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# Spec <NNNN>: <title>

**Approach** — the chosen design in a few sentences. Lead with the decision.

**Components / files** — the key modules/files and what each does.
- `path/to/file.py` — …

**Data & interfaces** — schemas, on-disk files, endpoints, function signatures,
config keys. Enough that someone could re-implement against it.

**Alternatives considered** — what else was on the table and why it lost.

**Risks / rollout** — what could break, how it ships, how to back out, any
cross-repo dependencies.

**Test plan** — what proves it works (tests, manual verification, live checks).
