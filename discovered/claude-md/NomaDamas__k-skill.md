---
name: NomaDamas__k-skill
source: https://github.com/NomaDamas/k-skill/blob/ece355b807221e27f3592a56bb3898b2a8d63ca3/CLAUDE.md
repo: NomaDamas/k-skill
kind: claude-md
stars: 5589
last_pushed: 2026-06-14T09:12:10Z
license: mit
score: 8
domains: [backend-api, devops, ci-cd, web-scraping]
tags: [anti-patterns, gcp-cloud-run, changesets, deployment-guide]
curated: 2026-06-15
curated_by: config-scout
---

# NomaDamas/k-skill — claude-md

**Why it's worth keeping:** The 'Testing anti-patterns' section is highly effective at preventing an AI from breaking release pipelines, while the proxy section provides specific deployment workflows and local test commands.

**Summary:** Provides critical CI/CD anti-patterns regarding changeset management and detailed DevOps deployment instructions for a GCP Cloud Run proxy.

**Source credibility:** High; high star count and active maintenance indicate it's a well-used, real-world project.

**Recency:** Current; uses modern tools like Changesets and Google Cloud Run/Workload Identity Federation.

**Source:** [NomaDamas/k-skill/CLAUDE.md](https://github.com/NomaDamas/k-skill/blob/ece355b807221e27f3592a56bb3898b2a8d63ca3/CLAUDE.md) · 5589★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# k-skill

## Testing anti-patterns

- **Never write tests that assert `.changeset/*.md` files exist.** Changesets are consumed (deleted) by `changeset version` during the release flow. Any test guarding changeset file presence will break CI on the version-bump commit and block the release pipeline.
- **Never write tests that pin a workspace package's `version` field** (in `package.json` or `package-lock.json`). `changeset version` bumps these on every release, so any hardcoded version assertion will fail the next release commit and block the npm publish pipeline. Stable invariants like `name`, `license`, `engines.node`, or workspace link metadata are fine to assert; the `version` is not.

## Crawling/search skill authoring

- 크롤링/검색 k-skill의 목표는 최종적으로 대상 사이트에 맞는 site-dependent 접근 방법을 스킬에 패키징하는 것이다.
- 다만 방법을 고정하기 전에 `insane-search`식 site-agnostic discovery를 먼저 수행한다: 공개 입구, 브라우저에서 보이는 데이터 흐름, RSS/sitemap/정적 JSON/모바일 페이지, 차단·빈 응답·로그인벽 실패 모드를 확인한다.
- 발견한 검색 URL, 필수 입력값, 결과 해석 규칙, fallback 순서, 실패 모드는 `SKILL.md`와 helper 코드에 명확히 남긴다. 자세한 체크리스트는 `docs/adding-a-skill.md`를 따른다.
- 새 크롤링 dependency는 기본값으로 추가하지 말고 기존 기능, 공개 endpoint, 좁은 proxy route로 해결 가능한지 먼저 확인한다.

## Proxy server developmen
```

</details>
