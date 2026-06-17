---
name: shriyanss__js-recon__claude
source: https://github.com/shriyanss/js-recon/blob/7470c2119339650bb798acf1247b594e17d4a214/src/lazyLoad/nuxt_js/CLAUDE.md
repo: shriyanss/js-recon
kind: claude-md
stars: 13
last_pushed: 2026-06-15T05:41:49Z
license: mit
score: 8
domains: [web-security, reverse-engineering]
tags: [nuxt, js-analysis, automation]
curated: 2026-06-15
curated_by: config-scout
---

# shriyanss/js-recon — claude-md

**Why it's worth keeping:** The 'Patterns / gotchas' section is a high-value technique for preemptively preventing AI hallucinations regarding downstream logic and security vulnerabilities.

**Summary:** Technical guide for Nuxt JS chunk crawling that outlines specific file responsibilities and version-specific nuances.

**Source credibility:** Niche specialized tool with recent maintenance activity.

**Recency:** Current; reflects modern Nuxt/JS analysis requirements.

**Source:** [shriyanss/js-recon/src/lazyLoad/nuxt_js/CLAUDE.md](https://github.com/shriyanss/js-recon/blob/7470c2119339650bb798acf1247b594e17d4a214/src/lazyLoad/nuxt_js/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# `src/lazyLoad/nuxt_js` — Nuxt chunk crawler

## Purpose

Discovers and downloads Nuxt JS chunks. Nuxt 3 emits chunks under `/_nuxt/` with a hashed manifest accessible via `__NUXT__` globals or the rendered page's inline JSON.

## Files

- `nuxt_getFromPageSource.ts` — extracts `<script>` references and the `__NUXT__` payload from the rendered HTML.
- `nuxt_astParse.ts` — parses chunks to enumerate `import()` calls and the build manifest entries.
- `nuxt_stringAnalysisJSFiles.ts` — string-scan fallback for hardcoded chunk URLs.

## Patterns / gotchas

- **Pipeline stops after lazyload.** Same as Angular — Nuxt is detected but downstream `map`/`analyze` are not wired. Don't add downstream assumptions here.
- **Nuxt 2 vs 3 differ.** The manifest shape and globals are different. Detection in `../techDetect/checkNuxtJS.ts` lumps them; the parser here tolerates both — preserve that.
- **`__NUXT__` payload can include sensitive server state** (request/response data inlined for hydration). The crawler captures it; downstream tools must NOT log its contents per the security policy in root `CLAUDE.md`.

## How to test changes here

```bash
npx tsc && node build/index.js lazyload -u <nuxt-t
```

</details>
