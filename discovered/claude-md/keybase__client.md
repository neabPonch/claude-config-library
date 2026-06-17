---
name: keybase__client
source: https://github.com/keybase/client/blob/ee3660551bbc1702a67b8a188679e1a54947b724/CLAUDE.md
repo: keybase/client
kind: claude-md
stars: 9220
last_pushed: 2026-06-12T23:12:47Z
license: bsd-3-clause
score: 9
domains: [mobile-app, desktop-app, typescript]
tags: [workflow-guardrails, git-best-practices, dependency-management]
curated: 2026-06-15
curated_by: config-scout
---

# keybase/client — claude-md

**Why it's worth keeping:** Uses highly specific negative constraints to prevent regression, provides precise git/tooling commands (e.g., gh pr view), and defines a clear validation workflow.

**Summary:** Defines strict operational, Git, and dependency management rules for a complex multi-platform codebase.

**Source credibility:** High: Based on the Keybase client, a widely recognized and highly-starred open-source project.

**Recency:** Current; reflects modern workflows for React Native, Expo, and Yarn.

**Source:** [keybase/client/CLAUDE.md](https://github.com/keybase/client/blob/ee3660551bbc1702a67b8a188679e1a54947b724/CLAUDE.md) · 9220★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Rules
- No `Co-Authored-By` in commits. Ever.
- Never interact with the Electron app or iOS simulator (screenshots, driving UI, debug ports) without asking first. The user drives and takes screenshots.
- "Was working before" = base branch, not previous commit. Base branch is almost always `nojima/HOTPOT-next-670-clean-2` (not `master`). Always run `gh pr view --json baseRefName` to confirm before any `git diff` or `git log` comparison.
- Never use `npm`. Always `yarn`.
- Never silently drop features/behavior — ask first, present options.
- In tests/stories, use `testuser` / `testuser-mac` as placeholder usernames — never real usernames like `chrisnojima`.
- No DOM elements (`<div>`, `<span>`, etc.) in plain `.tsx` files — use `Kb.*`. Guard desktop-only DOM with `Styles.isMobile`.
- Temp files go in `/tmp/`.
- Remove unused code when editing: styles, imports, vars, params, dead helpers.
- Comments: no refactoring notes; only add when context isn't obvious from code.
- Exact versions in `package.json` (no `^`/`~`).
- Keep `react`, `react-dom`, `react-native`, `@react-native/*` in sync with Expo SDK.
- When updating deps: edit `package.json` → `yarn` → `yarn ios:pod:install`.
- Whe
```

</details>
