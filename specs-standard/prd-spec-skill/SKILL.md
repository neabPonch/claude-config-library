---
name: prd-spec
description: Scaffold and maintain PRDs and specs following the shared specs-standard. Use when starting a non-trivial feature, capturing design, or when the user asks to "write a PRD/spec", "capture this in a spec", or regain a paper trail on work in flight.
---

# prd-spec — capture what we're building, and how

Create and maintain lightweight PRDs (what & why) and specs (how) per the
`specs-standard`. Keep them short and current; the goal is a paper trail that
prevents scope-creep, not ceremony.

## When to use
- Starting a **non-trivial feature** → PRD (and a spec if the design is significant).
  For a single-repo feature where a PRD is overkill, a `## Brief` section atop
  the spec may replace it: six questions — what / problem / who for /
  **what matters most (ranked)** / constraints / success. The ranking is the
  tie-breaker agents use for unresolved tradeoffs; a brief that ranks nothing
  is not a brief.
- A subsystem is **already being built** without docs → backfill a PRD+spec to
  capture it (this is the "things are spiraling, capture it" case).
- A design decision needs recording, or status/scope changed → update the doc.
- A decision is hard to reverse, spans components, or you've explained it to an
  agent **twice** → write an **ADR** (`docs/decisions/NNN-slug.md`, Nygard
  format, 10–20 min; supersede, never delete). Best ADR type: a standing
  guardrail with a measurable trigger ("no read cache until P99 > 200ms").
- Skip both for trivial changes.

## Before the spec: risk spike
If the approach rests on one unproven assumption that would kill it, spike that
first: one yes/no question, one agent session max, code deleted afterward, and
the verdict recorded in ~5 lines in the spec (question / tried / verdict / date).

## Where things go
Per repo, flat files in `specs/`:
- `specs/NNNN-slug.prd.md`, `specs/NNNN-slug.spec.md`, `specs/INDEX.md`
- `NNNN` is a zero-padded number shared by a PRD and its spec; increment per
  initiative. Find the next number by scanning existing `specs/`.

## How to create one
1. Determine the repo's `specs/` dir; create it (+ `INDEX.md`) if missing.
2. Pick the next `NNNN` and a short kebab `slug`.
3. Copy the relevant template from `claude-config-library/specs-standard/`
   (`prd-template.md` / `spec-template.md`), fill the frontmatter
   (`id`, `title`, `status`, dates, cross-links) and the body. Keep it tight —
   a PRD is ~one page; a spec leads with the decision.
4. Cross-link: PRD `spec:` ↔ spec `prd:`.
5. Add/update the row in `specs/INDEX.md`.

## Lifecycle
`draft → active → shipped → archived|superseded`. When work ships, flip
`status: shipped` and refresh `updated:` — don't delete. Keep `INDEX.md` in sync.

## Rigor level (`rigor:` frontmatter)
- `first` — spec may go stale after merge (exploratory/churning work).
- `anchored` (default) — living doc: any PR changing described behavior updates
  the spec **in the same PR**. A spec updated "later" is updated never.
- `source` — code regenerated from spec; only where outside-in tests would
  catch a silent behavior change ("human reads the diff" doesn't count).
Downgrading anchored→first is allowed — record it. A stale spec is worse than
none: agents implement confidently against wrong documents.

## Writing guidance
- **PRD**: problem first, then goals, **non-goals** (guard against scope-creep),
  users/use-cases, MUST/SHOULD requirements, success criteria, open questions.
- **Spec**: approach (lead with the decision), components/files, data &
  interfaces (enough to re-implement), alternatives considered, risks/rollout
  (incl. cross-repo deps), test plan.
- Prefer concrete file paths, function/endpoint names, and config keys over prose.
- **Acceptance criteria** for any task an agent runs unattended: numbered,
  specific, agent-testable (name the command), what-not-how, 3–7 per task —
  the agent stops where the criteria stop; unstated criteria are unmet criteria.
- **Task sizing**: decompose to one-agent-session units — read the relevant
  code, change it, and *verify it* in one context window; verification belongs
  inside the task ("add X and run the tests"), never as a follow-up.
