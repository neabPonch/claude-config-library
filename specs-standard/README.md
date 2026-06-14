# PRD / Spec standard

The shared convention for capturing **what we're building and why** (PRD) and
**how** (Spec) across all repos. Lightweight on purpose — fast to write, fast to
keep current, for a fast-moving single-dev system. This folder is the canonical
source; each repo carries its own `specs/` folder following these rules.

## The two docs

- **PRD** (`NNNN-slug.prd.md`) — product/requirements: the problem, goals,
  non-goals, requirements, success criteria. The *what & why*. Write/update one
  **before building a non-trivial feature**.
- **Spec** (`NNNN-slug.spec.md`) — technical design: approach, components,
  interfaces, alternatives, risks, test plan. The *how*. Write/update one
  **before significant design**, and link it to its PRD.

A small change doesn't need either. A new subsystem needs both. Use judgment.

## Where they live

Per repo, flat files in `specs/`:

```
<repo>/specs/
  INDEX.md                     # one line per doc, status + link
  0001-agent-runtime.prd.md
  0001-agent-runtime.spec.md
  0002-autoscheduler.prd.md
  0002-autoscheduler.spec.md
```

- **Numbering**: zero-padded, shared across PRD+spec of the same initiative
  (the PRD and its spec share an `id`). Increment per initiative.
- **Pairing**: a PRD links its spec via `spec:` frontmatter; the spec links back
  via `prd:`. A PRD can exist without a spec (e.g. trivial implementation).

## Lifecycle (the `status:` field)

`draft` → `active` (being built) → `shipped` (done & verified) →
`archived` (no longer relevant) / `superseded` (replaced — link the successor).

Keep `status:` and `updated:` current, and add a line to `specs/INDEX.md`. When a
feature ships, flip status to `shipped` rather than deleting the doc — the trail
is the point.

## Templates

- [`prd-template.md`](prd-template.md)
- [`spec-template.md`](spec-template.md)

## Tooling

- **Skill**: `prd-spec` scaffolds and updates these docs ([canonical copy](prd-spec-skill/SKILL.md)).
- **CLAUDE.md**: every repo pastes [`CLAUDE-fragment.md`](CLAUDE-fragment.md) so
  Claude follows the convention automatically.
