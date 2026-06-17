---
name: DeadIntegral__stupidk-blog-astro
source: https://github.com/DeadIntegral/stupidk-blog-astro/blob/cd15f04eb35943725950740ccfbe8af214f239d8/CLAUDE.md
repo: DeadIntegral/stupidk-blog-astro
kind: claude-md
stars: 0
last_pushed: 2026-06-13T08:03:14Z
license: unknown
score: 8
domains: [web-frontend, content-management]
tags: [taxonomy, metadata, astro, workflow]
curated: 2026-06-14
curated_by: config-scout
---

# DeadIntegral/stupidk-blog-astro — claude-md

**Why it's worth keeping:** It uses 'negative constraints' (what not to include) and outlines a sophisticated pattern of separating LLM suggestion from deterministic script enforcement via `normalize-tags.mjs`.

**Summary:** Defines a rigorous tagging taxonomy and normalization workflow for an Astro-based content system to prevent metadata pollution.

**Source credibility:** Low star count, but the highly specific technical constraints suggest an experienced developer writing for themselves.

**Recency:** Current; utilizes modern Astro/Node.js workflows.

**Source:** [DeadIntegral/stupidk-blog-astro/CLAUDE.md](https://github.com/DeadIntegral/stupidk-blog-astro/blob/cd15f04eb35943725950740ccfbe8af214f239d8/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Astro 기반 개인 블로그. 콘텐츠 컬렉션: `blog`(직접 쓴 글), `weekly`(주간 개발 소식 요약), `archive`(예전 글). 스키마는 `src/content.config.ts`.

## 콘텐츠 태그 컨벤션

태그는 각 글 frontmatter 의 `tags:` (문자열 배열)에 들어가며, `/tags` 와 `/tags/[tag]` 로 탐색된다. 태그 시스템은 본문이 실제 다루는 주제를 반영하도록 설계되어 있다 (단순 `javascript`/`node`/`css` 나열 ❌).

**표기 규칙**

- 모두 소문자
- 여러 단어는 kebab-case: `web-components`, `view-transitions`, `source-map`, `css-grid`
- 단수형 명사
- 글당 **4~8개**, 가장 핵심적인 구체 주제 위주
- 과도하게 일반적/모호한 태그 금지: `web`, `etc`, `tutorial`, `tools`, `code`, `dev`, `programming`, `news`, `release`, `set`, `layout`, `transform`, `https`, `viewport`, `module`, `async` 등
- 동의어는 표준형으로 통일: `nodejs`→`node`, `js`→`javascript`, `ts`→`typescript`, `webassembly`→`wasm`, `a11y`→`accessibility`, `db`→`database`, `grid`→`css-grid` (전체 매핑은 `scripts/normalize-tags.mjs` 의 `CANON`)
- **기존 어휘 재사용 우선**: 새 태그를 만들기 전에 현재 쓰이는 태그(예: `/tags` 또는 기존 frontmatter)를 먼저 살펴 같은 개념이면 같은 표기를 쓴다.

자주 쓰는 태그(참고): `node css javascript typescript react performance accessibility deno wasm v8 npm security electron animation testing devtools browser rust web-components eslint nextjs bun bundler angular astro vite svelte chrome go view-transitions http esm database svg pwa compiler e
```

</details>
