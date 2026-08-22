<!-- Paste this section into each repo's CLAUDE.md (under its own heading). -->

## Specs & PRDs

This repo follows the shared **PRD/Spec standard** (canonical:
`claude-config-library/specs-standard`). Design docs live in `specs/` as numbered
pairs — `NNNN-slug.prd.md` (what & why) and `NNNN-slug.spec.md` (how) — indexed in
`specs/INDEX.md`.

- Before building a **non-trivial feature**, write or update a **PRD**.
- Before **significant design/architecture**, write or update a **Spec** linked to
  its PRD. Small changes need neither — use judgment.
- Keep `status:` current (`draft → active → shipped`) and `updated:` fresh, and add
  a line to `specs/INDEX.md`. Ship by flipping status to `shipped`, not deleting.
- **Same-PR rule**: for `rigor: anchored` specs (the default), read the relevant
  spec before changing described behavior and update it **in the same PR** as
  the behavior change.
- Before structural changes, read `docs/decisions/` (ADRs) if present — don't
  contradict or re-propose what a standing decision already settled.
- Use the **`prd-spec` skill** to scaffold or update these.
