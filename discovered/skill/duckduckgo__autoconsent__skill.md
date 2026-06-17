---
name: duckduckgo__autoconsent__skill
source: https://github.com/duckduckgo/autoconsent/blob/44ac69c5111656d742950a8434205f48ea695cf8/.agents/skills/verify-pr/SKILL.md
repo: duckduckgo/autoconsent
kind: skill
stars: 116
last_pushed: 2026-06-14T11:53:21Z
license: mpl-2.0
score: 9
domains: [web-automation, qa-engineering, devops]
tags: [checklist, verification, e2e-testing, pull-requests]
curated: 2026-06-15
curated_by: config-scout
---

# duckduckgo/autoconsent — skill

**Why it's worth keeping:** It uses a checklist pattern for progress tracking and embeds deep-domain heuristics (e.g., selector stability requirements) that prevent subtle regressions.

**Summary:** A highly structured multi-stage verification protocol that guides an agent through local linting, domain-spsific rule auditing, and CI/E2E inspection.

**Source credibility:** High; comes from a reputable, actively maintained repository by DuckDuckGo.

**Recency:** Very current; utilizes modern tooling like Playwright and Chrome MV3 standards.

**Source:** [duckduckgo/autoconsent/.agents/skills/verify-pr/SKILL.md](https://github.com/duckduckgo/autoconsent/blob/44ac69c5111656d742950a8434205f48ea695cf8/.agents/skills/verify-pr/SKILL.md) · 116★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: verify-pr
description: Verifies an autoconsent pull request by running local CI checks, reviewing rule quality, and inspecting Jenkins E2E results. Use when reviewing, verifying, or approving a PR, when checking if a PR is ready to merge, or when the user asks to validate PR changes.
---

# Verify PR

Copy this checklist and track progress:

```
PR Verification:
- [ ] Step 1: Local checks pass
- [ ] Step 2: Rule review complete
- [ ] Step 3: CI results checked
- [ ] Step 4: Browser verification done
```

## Step 1: Local Checks

```bash
npm run lint
npm run rule-syntax-check
npm run test:lib
npx playwright test tests/<cmp>.spec.ts --project webkit
```

If any check fails, fix the issue and re-run before proceeding.

## Step 2: Rule Review

### JSON rule PRs

- [ ] Test spec exists in `tests/` with reachable URLs
- [ ] Selectors are stable (no CSS module hashes, dynamic IDs, or framework-generated IDs)
- [ ] `optOut` targets a reject/decline button, not a privacy policy link or close button
- [ ] `prehideSelectors` are narrow (no `body` or full-page selectors)
- [ ] `minimumRuleStepVersion: 2` if rule uses `removeClass`, `setStyle`, or `addStyle`
- [ ] Generated rule fixes
```

</details>
