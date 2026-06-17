---
name: NomaDamas__k-skill__skill
source: https://github.com/NomaDamas/k-skill/blob/1f186af480a49ee55a07ea0af2b0f29a1d98c193/lck-analytics/SKILL.md
repo: NomaDamas/k-skill
kind: skill
stars: 5681
last_pushed: 2026-06-16T04:54:01Z
license: mit
score: 9
domains: [data-analysis, esports, cli-tools]
tags: [sports-analytics, api-integration, automated-reporting]
curated: 2026-06-16
curated_by: config-scout
---

# NomaDamas/k-skill — skill

**Why it's worth keeping:** Demonstrates excellent pattern for team name normalization, multi-step CLI workflows using local scripts, and strict output formatting guidelines based on query intent.

**Summary:** A highly sophisticated skill for LCK esports analysis that integrates live Riot API data with local historical statistical pipelines.

**Source credibility:** High; part of a popular specialized repository (k-skill) with high star count and active maintenance.

**Recency:** Current; uses modern Node.js ESM patterns and detailed API surface mappings.

**Source:** [NomaDamas/k-skill/lck-analytics/SKILL.md](https://github.com/NomaDamas/k-skill/blob/1f186af480a49ee55a07ea0af2b0f29a1d98c193/lck-analytics/SKILL.md) · 5681★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: lck-analytics
description: Riot 공식 LoL Esports 데이터와 Oracle's Elixir 스타일 historical 데이터로 LCK 경기 결과, 현재 순위, live turning point, 밴픽 matchup/synergy, patch meta, 팀 파워 레이팅을 조회한다.
license: MIT
metadata:
  category: sports
  locale: ko-KR
  phase: v1
---

# LCK Results + Advanced Analysis

## What this skill does

이 스킬은 LCK 조회/분석 전용이다.

- 특정 날짜 LCK 경기 결과 조회
- 특정 팀 alias 정규화 후 필터링
- 현재 스플릿 순위 조회
- 진행 중 경기 live stats 조회
- live timeline 기반 turning point 분석
- Oracle's Elixir 스타일 historical row / CSV 기반
  - 팀 파워 레이팅
  - 챔피언 matchup / synergy 분석
  - patch meta 요약
- 날짜별 match analysis 생성

## Origin / attribution

이 스킬은 `jerjangmin` 님이 만든 원본 [`lck-analytics` skill pack](https://github.com/jerjangmin/share/tree/main/SKILL/lck-analytics)을 k-skill 저장소 안으로 옮기고, 이 저장소의 npm workspace / Changesets 배포 방식에 맞게 정리한 버전이다.

## When to use

- "오늘 LCK 경기 결과 알려줘"
- "2026-04-01 한화 경기 결과랑 순위 보여줘"
- "지금 T1 경기 킬/골드/오브젝트 요약해줘"
- "이 경기 turning point가 뭐였어?"
- "이 밴픽에서 어느 쪽 조합이 더 좋았는지 설명해줘"
- "현재 패치에서 어떤 챔피언이 메타 픽인지 보여줘"
- "LCK 팀 파워 레이팅 보여줘"

## Prerequisites

- Node.js 18+
- `npm install -g lck-analytics`

패키지가 없으면 다른 방법으로 우회하지 말고 먼저 전역 설치를 시도한다.

```bash
npm install -g lck-analytics
```

## Inputs

### 기본 입력
```

</details>
