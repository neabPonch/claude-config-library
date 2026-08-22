---
id: NNNN
title: <short title>
type: spec
status: draft            # draft | active | shipped | archived | superseded
rigor: anchored          # first | anchored | source  (see specs-standard README)
prd: NNNN-slug.prd.md     # link back to the PRD, or omit if the Brief replaces it
created: YYYY-MM-DD
updated: YYYY-MM-DD
---

# Spec <NNNN>: <title>

<!-- Optional: for single-repo features without a PRD, open with a ## Brief —
the six questions (what / problem / who for / WHAT MATTERS MOST, ranked /
constraints / success). Delete if a PRD exists. -->

**Risk spike** — the assumption that kills this approach if false, and the
spike verdict (question, what was tried, verdict, date). "None" is fine.

**Approach** — the chosen design in a few sentences. Lead with the decision.

**Components / files** — the key modules/files and what each does.
- `path/to/file.py` — …

**Data & interfaces** — schemas, on-disk files, endpoints, function signatures,
config keys. Enough that someone could re-implement against it.

**Alternatives considered** — what else was on the table and why it lost.

**Risks / rollout** — what could break, how it ships, how to back out, any
cross-repo dependencies.

**Test plan** — what proves it works (tests, manual verification, live checks).

**Acceptance criteria** — numbered, for any task an agent runs unattended:
specific, agent-testable (name the command), what-not-how, 3–7 per task.
The agent stops where these stop — unstated criteria are unmet criteria.
