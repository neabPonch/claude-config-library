---
name: 404-novel-project__novel-downloader
source: https://github.com/404-novel-project/novel-downloader/blob/cf78ec37c8e5736ddc272602aaeb43fc5abe0037/CLAUDE.md
repo: 404-novel-project/novel-downloader
kind: claude-md
stars: 1754
last_pushed: 2026-06-10T17:38:28Z
license: agpl-3.0
score: 8
domains: [web-scraping, automation, userscripts]
tags: [javascript, tampermonkey, testing]
curated: 2026-06-15
curated_by: config-scout
---

# 404-novel-project/novel-downloader — claude-md

**Why it's worth keeping:** Includes high-value 'negative constraints' regarding regex usage and a mandatory instruction to use real HTML instead of accessibility snapshots when scraping.

**Summary:** Provides specialized instructions for userscript development, covering specific build pipelines, site rule management, and E2E testing requirements.

**Source credibility:** Highly credible source with 1754 stars and very recent maintenance activity.

**Recency:** Current; uses modern tooling like tsx and specific dev server workflows.

**Source:** [404-novel-project/novel-downloader/CLAUDE.md](https://github.com/404-novel-project/novel-downloader/blob/cf78ec37c8e5736ddc272602aaeb43fc5abe0037/CLAUDE.md) · 1754★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Copilot Instructions

## Project Type

- This repository is a webpack-userscript project targeting Tampermonkey, Violentmonkey, and compatible userscript managers.
- The main entry is `src/index.ts`, and userscript metadata is generated from `src/header.json` by `webpack-userscript`.

## Local Development

- Use `yarn dev` for local proxy-script development. The dev server serves `http://webpack.localhost:11944/bundle.proxy.user.js`.
- Use `yarn build` for the production userscript bundle and `yarn build-greasyfork` for the unminified GreasyFork bundle.
- When a change affects userscript execution, prefer validating both `yarn lint` and `yarn build`.
- The integrated browser can verify generated pages and local dev endpoints, but actual Tampermonkey or Violentmonkey runtime validation must happen in a browser profile where the extension is installed.

## Site Rule Changes

- Add or update match patterns in `src/header.json`.
- Register routing changes in `src/router/download.ts`.
- Keep rule implementations inside the existing site-specific folders under `src/rules/`.
- Follow the existing rule style. Prefer the smallest site-specific rule that fits the target website instead of
```

</details>
