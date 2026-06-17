---
name: fernandosimoes__time-off-frontend
source: https://github.com/fernandosimoes/time-off-frontend/blob/4ff9605ab8b284781cdc9c6d58a4026a3d1498ed/CLAUDE.MD
repo: fernandosimoes/time-off-frontend
kind: claude-md
stars: 0
last_pushed: 2026-04-28T21:27:45Z
license: unknown
score: 9
domains: [web-frontend, agents-ai]
tags: [spec-driven, nextjs, typescript, strict-instructions]
curated: 2026-06-14
curated_by: config-scout
---

# fernandosimoes/time-off-frontend — claude-md

**Why it's worth keeping:** Uses explicit scope constraints (what NOT to include) and an unambiguous protocol for handling ambiguity or uncertainty. The 'What to Do When Stuck' section is a high-tier technique for reducing AI hallucinations.

**Summary:** Defines a strict 'Spec-Driven Development' workflow that forces the agent to prioritize human-written specifications over its own intuition.

**Source credibility:** Low visibility repo, but the content reflects senior-level engineering standards and clear architectural intent.

**Recency:** Very current; references modern stacks like Next.js 14+, TanStack Query v5, and Storybook 8.

**Source:** [fernandosimoes/time-off-frontend/CLAUDE.MD](https://github.com/fernandosimoes/time-off-frontend/blob/4ff9605ab8b284781cdc9c6d58a4026a3d1498ed/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file is the project constitution. Read it before doing any work in this repository.

## Project Context

This project is a Time-Off frontend for ExampleHR, a fictional HR platform. It demonstrates how to build a UI layer that talks to an external HCM system (Workday-like) as the source of truth, while maintaining instant UX and correctness guarantees.The full architecture and design decisions live in `TRD.md`. **Read TRD.md before generating any non-trivial code.**

The deliverable is evaluated on:
1. Quality of the technical specification (TRD)
2. Rigor of tests (Storybook stories, integration tests, schema tests)
3. Architectural decisions and their defense
4. Code quality, in that order

## Working Method

This project follows Spec-Driven Development. The workflow is:

1. Human writes a milestone spec in `specs/`
2. Agent reads the spec, the TRD, and this file
3. Agent implements the milestone, running tests as it goes
4. Agent reports completion with: what was done, what tests pass, what is deferred
5. Human verifies and refines

**The agent does not improvise scope.** If a milestone spec asks for X, the agent delivers X, even if Y feels like a natural extensi
```

</details>
