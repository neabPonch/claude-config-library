---
name: TriliumNext__Trilium__skill
source: https://github.com/TriliumNext/Trilium/blob/274b4d4154ac03fdd4ee284b2262ac2262bc2b3f/.claude/skills/ckeditor5-testing/SKILL.md
repo: TriliumNext/Trilium
kind: skill
stars: 36456
last_pushed: 2026-06-15T07:14:47Z
license: agpl-3.0
score: 9
domains: [web-frontend, testing]
tags: [ckeditor5, vitest, monorepo, javascript]
curated: 2026-06-15
curated_by: config-scout
---

# TriliumNext/Trilium — skill

**Why it's worth keeping:** Includes exact CLI commands, distinctions between runtime environments (happy-dom vs. WebdriverIO), and precise patterns for model/view data manipulation that prevent agent hallucination.

**Summary:** Provides highly specific instructions for testing CKEditor 5 plugins within a complex monorepo using Vitest.

**Source credibility:** High; comes from a highly-starred, actively maintained open-source project (Trilium).

**Recency:** Extremely current; refers to very recent repository activity.

**Source:** [TriliumNext/Trilium/.claude/skills/ckeditor5-testing/SKILL.md](https://github.com/TriliumNext/Trilium/blob/274b4d4154ac03fdd4ee284b2262ac2262bc2b3f/.claude/skills/ckeditor5-testing/SKILL.md) · 36456★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ckeditor5-testing
description: >-
  Testing CKEditor 5 plugins in the Trilium monorepo. Use when adding or
  reviewing unit tests for a packages/ckeditor5-* package, debugging a failing
  test, or setting up a package's test runner. Covers the two Vitest
  environments Trilium uses (happy-dom and the WebdriverIO browser mode), the
  per-package vitest.config.ts, testing against a real ClassicEditor, the
  model/view helpers imported from 'ckeditor5' (_setModelData / _getModelData /
  _getViewData and their {}/[] selection syntax), vi spies/mocks, idiomatic
  patterns for schema/conversion/command/UI tests, the pnpm --filter runner, and
  Trilium-specific conventions and gotchas. Complements the
  ckeditor5-plugin-development and writing-unit-tests skills.
---

# CKEditor 5 testing (Trilium)

Testing CKEditor 5 plugins in the **Trilium (TriliumNext Notes) monorepo**. **Tests are co-located
`*.spec.ts` next to the source** for the aggregator (`packages/ckeditor5`), in-aggregator plugins,
and any new code — matching the repo-wide convention. The existing standalone packages
(`packages/ckeditor5-<name>/`) keep their legacy `tests/` directories. Browser-mode packages gate
`src
```

</details>
