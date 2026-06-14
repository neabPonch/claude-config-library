---
name: microsoft__finnts
source: https://github.com/microsoft/finnts/blob/e8e3859f013d52cfc5f09f680edbce1a5cbfdffc/CLAUDE.md
repo: microsoft/finnts
kind: claude-md
stars: 260
last_pushed: 2026-05-26T20:19:14Z
license: other
score: 7
domains: [data-science, r-programming]
tags: [r, devtools, forecasting]
curated: 2026-06-14
curated_by: config-scout
---

# microsoft/finnts — claude-md

**Why it's worth keeping:** Provides exact command sequences for documentation and testing (e.g., devtools::document()) and enforces a strict policy against unrequested refactors.

**Summary:** Defines a specialized R package development workflow using specific devtools commands to ensure structural integrity.

**Source credibility:** High; originates from a Microsoft-maintained repository with recent activity.

**Recency:** Current; follows modern patterns of planning, minimal intervention, and rule scalability.

**Source:** [microsoft/finnts/CLAUDE.md](https://github.com/microsoft/finnts/blob/e8e3859f013d52cfc5f09f680edbce1a5cbfdffc/CLAUDE.md) · 260★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Claude Code project memory for finnts

@AGENTS.md

## Claude-specific working agreements
- Start by summarizing the plan (bullets) and the files you’ll touch.
- Prefer running `devtools::test()` after code changes, and `devtools::check()` before finalizing.
- If you change roxygen comments, run `devtools::document()` and include generated diffs.
- Keep changes minimal: avoid drive-by refactors unless explicitly requested.
- If a request is ambiguous, ask the smallest number of clarifying questions needed, then proceed conservatively.

## Notes
- If this repo grows, move large topic rules into `.claude/rules/*.md` (testing, style, release).
```

</details>
