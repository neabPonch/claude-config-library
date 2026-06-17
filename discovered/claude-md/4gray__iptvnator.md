---
name: 4gray__iptvnator
source: https://github.com/4gray/iptvnator/blob/3d2549dacea5c98239eb8aab6c3acd494878fef5/CLAUDE.md
repo: 4gray/iptvnator
kind: claude-md
stars: 6251
last_pushed: 2026-06-15T17:50:21Z
license: mit
score: 9
domains: [electron-app, web-frontend, testing-automation]
tags: [plan-management, cdp-debugging, test-validation, documentation-lifecycle]
curated: 2026-06-15
curated_by: config-scout
---

# 4gray/iptvnator — claude-md

**Why it's worth keeping:** The `.plans/` directory pattern is a brilliant way to track agent intent; the 'validation ladder' and advanced CDP tracing flags provide indispensable context for troubleshooting complex desktop-app behavior.

**Summary:** A high-rigor instruction file that mandates specific workflows for planning, documentation updates, and test coverage. It excels at providing deep technical observability instructions for debugging Electron environments.

**Source credibility:** Highly credible; the repository is well-starred, actively maintained, and the file contains highly specific, non-generic technical protocols.

**Recency:** Very current; specifically tailored for Claude Code's capabilities and modern development workflows like Nx and CDP.

**Source:** [4gray/iptvnator/CLAUDE.md](https://github.com/4gray/iptvnator/blob/3d2549dacea5c98239eb8aab6c3acd494878fef5/CLAUDE.md) · 6251★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Plan Mode

- When Claude Code is in Plan Mode and produces a final `<proposed_plan>`, it must also save that finalized plan as a Markdown file in the repo-root `.plans/` directory.
- Save only finalized plans. Do not write interim exploration, question turns, or draft revisions to `.plans/`.
- Use the filename pattern `YYYY-MM-DD-short-topic.md` such as `.plans/2026-03-12-channel-filtering.md`.
- If the intended filename already exists, append a numeric suffix such as `-2`, `-3`, and so on.

## Documentation After Changes

- After implementing a meaningful change, Claude Code must assess whether canonical repo docs need updates before considering the task complete.
- Meaningful changes include new or changed user-visible behavior, architecture or data-flow changes, non-obvious maintenance workflows, new setup/debugging steps, and new subsystem contracts or boundaries.
- Skip doc updates for trivial refactors with unchanged behavior, formatting-only edits, and isolated test-only changes.
- Prefer updating an existing authoritative doc before creating a new one:
```

</details>
