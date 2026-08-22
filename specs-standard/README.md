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

For a **single-repo feature** where a full PRD is overkill, a **`## Brief`
section at the top of the spec** may replace the PRD (see below). Trivial
changes still need neither.

## Rigor levels

Every spec declares `rigor:` in its frontmatter (default: **anchored**).

- **first** — spec written before build; allowed to go stale after merge. For
  short-lived or exploratory work, or while a feature is still churning.
- **anchored** (default) — living document: any PR that changes described
  behavior updates the spec **in the same PR**. Spec is the source of truth for
  intent; code for behavior.
- **source** — spec is canonical and code is regenerated from it, not
  hand-edited. Only for narrow, well-bounded components with outside-in tests
  that would catch a silently changed behavior. If the only safety net is
  "a human reads the diff", the component is not ready for this level.

Downgrading (anchored → first) is allowed — record it in the frontmatter. An
honest `first` beats a lying `anchored`: agents implement confidently against
wrong documents, so a stale spec is worse than none.

## Briefs

A brief answers six questions, in order, in under a page — as a `## Brief`
section at the top of the spec (the common case) or as a PRD's opening for
bigger efforts:

1. What is it? (1–2 sentences)
2. What problem does it solve? (user-visible, not a technical itch)
3. Who is it for? (named specifically)
4. **What matters most?** — a *ranked* tradeoff order (e.g. correctness >
   speed > polish). This is the tie-breaker the agent reaches for at every
   tradeoff the spec doesn't resolve. A brief that ranks nothing is not a brief.
5. What constraints exist? (non-negotiables)
6. What counts as success? (checkable outcomes)

No implementation detail. If an agent expands a brief into a spec, review the
spec before any implementation session runs — an unreviewed expansion silently
becomes the brief for every later session.

## ADRs

`docs/decisions/NNN-slug.md`, Nygard format, 10–20 minutes each. Write one when
a decision is hard to reverse, affects multiple components, or you've explained
it to an agent **twice**. Never for trivia.

```markdown
# NNN. <Noun-phrase title>
Status: proposed | accepted | superseded by NNN
Context: <2–4 sentences: forces and constraints>
Decision: We will <active voice>.
Consequences: <easier / harder / new constraints>
```

- Agents making structural changes read `docs/decisions/` first (wired into
  the repo's CLAUDE.md).
- Never delete an ADR; supersede it. Why you stopped doing something is as
  valuable as why you started.
- The highest-value ADR type in agent-driven repos is a **standing guardrail
  with a measurable trigger** ("Do not add a read cache until P99 > 200ms;
  currently 45ms") — it ends agent re-proposal loops.

## Risk spikes — the pre-spec gate

Before writing a spec whose approach rests on an unproven assumption, ask:
*what single assumption, if false, kills this approach?* If one exists and is
untested, spike it **before** the spec.

- One question, yes/no answerable. Time-box: one agent session.
- Spike code skips error handling and edge cases by contract, and is
  **deleted**. The deliverable is the answer, recorded in ~5 lines in the
  spec's context (question, what was tried, verdict, date). A kept spike is
  production code written to a throwaway standard.
- Spikes are also how you locate a model's jagged frontier: unsure an agent
  can drive a toolchain? Ask it to, and watch, for the price of a discarded
  attempt.

## Acceptance criteria & task sizing

Any task an agent executes unattended carries numbered acceptance criteria —
the agent stops the moment it believes it's done, so **the finish line you
define is the finish line it crosses; unstated criteria are unmet criteria.**

- Specific and measurable — never "works".
- Testable by the agent itself — name the command ("`pytest -q` passes").
- What, not how. Cover the happy path, the failure modes you care about, and
  non-functionals — agents happy-path unless told otherwise.
- 3–7 criteria per task; more is brittleness, not rigor.

Size tasks to **one agent session**: read the relevant code, make the change,
and *verify it*, within one context window. Verification is part of the task
("add X and run the tests"), never a follow-up. A well-decomposed task list
beats a smarter model with a vague goal.

## Living-doc rules

- **Same-PR rule** (anchored specs): behavior change and spec update land in
  one PR. A spec updated "later" is a spec updated never.
- **Stable paths**: specs in `specs/`, ADRs in `docs/decisions/`. The repo's
  CLAUDE.md tells agents to read the relevant spec before behavior changes and
  update it in the same commit.
- **Inspectability floor**: every artifact must teach a stranger (or a fresh
  agent session) something — no title-only issues, no `fix` commits.
- **Archive, don't delete** — specs get `archived`/`superseded`, ADRs get
  superseded. On resuming stale work, reconcile the doc against reality
  before building.

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
