---
name: SwamysArchitectJourney-2026__system-design-playbook
source: https://github.com/SwamysArchitectJourney-2026/system-design-playbook/blob/e000029eee185ed6398e54273a4b033cc5e2b5ac/claude.md
repo: SwamysArchitectJourney-2026/system-design-playbook
kind: claude-md
stars: 0
last_pushed: 2026-05-31T02:58:20Z
license: mit
score: 9
domains: [documentation-engineering, ai-orchestration, system-design]
tags: [agentic-workflow, structural-governance, knowledge-management]
curated: 2026-06-16
curated_by: config-scout
---

# SwamysArchitectJourney-2026/system-design-playbook — claude-md

**Why it's worth keeping:** The integration of mandatory reasoning frameworks (CoT/ReAct) and the 'Structure Update Protocol' are elite techniques for preventing state drift during AI-led refactoring.

**Summary:** Orchestrates multiple AI agents to manage a complex technical knowledge base through strict structural and content-governance protocols. It establishes a rigorous single source of truth for repository state.

**Source credibility:** Low social proof on GitHub, but demonstrates high-level architectural thinking in its instruction design.

**Recency:** Very current; specifically optimized for modern agentic tools like Claude Code and Cursor Skills.

**Source:** [SwamysArchitectJourney-2026/system-design-playbook/claude.md](https://github.com/SwamysArchitectJourney-2026/system-design-playbook/blob/e000029eee185ed6398e54273a4b033cc5e2b5ac/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — System Design in Practice

## Repository Purpose

Swamy's personal system design playbook. A **thinking system**, not a notes repo. Focused on structured reasoning, reusable architectural patterns, and production-grade decision-making.

---

## Critical Rules

### Naming (Files, Folders & Topics)

- **NEVER** use `00_` prefix on any file, folder, or topic name — use `01_` and above, no exceptions
- Use zero-padded numeric prefixes: `01_`, `02_`, etc.
- Use hyphens for multi-word names: `01_modern-system-design.md`
- Split files use `-part1`, `-part2` (never `A/B/C`)

### File Size

- **≤ 1000 lines per file** — split into parts if exceeded; never trim or condense

### Content Policy

- **Zero-copy policy** — all content must be transformative, not reformative
- **Quality bar**: can it be explained clearly in 5–10 minutes?
- Chain-of-Thought reasoning required in every design decision — show the "why"
- **Staging hygiene**: Do **not** mention `source-material/` (or `reference-material/`) in `README.md`, public content folders, or `docs/**/*.md`. Synthesize into tracked docs; full rule: `.cursor/rules/08_source_material_rules.mdc`.

### Diagrams

- **Mermaid-first**, AS
```

</details>
