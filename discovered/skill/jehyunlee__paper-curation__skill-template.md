---
name: jehyunlee__paper-curation__skill-template
source: https://github.com/jehyunlee/paper-curation/blob/67acecc780694d8442950f3a639a124617963514/SKILL.md.template
repo: jehyunlee/paper-curation
kind: skill
stars: 38
last_pushed: 2026-06-14T12:49:07Z
license: unknown
score: 9
domains: [agents-ai, data-pipeline, research-automation]
tags: [orchestrator, workflow-automation, parallel-processing]
curated: 2026-06-15
curated_by: config-scout
---

# jehyunlee/paper-curation — skill

**Why it's worth keeping:** It excels at defining complex state management via mode matrices (full/update/force) and implements a highly transferable 'Orchestrator + Fan-out' architectural pattern for parallelizing agent tasks.

**Summary:** An end-to-end orchestration skill that manages a sophisticated research pipeline, encompassing multi-source discovery, Zotero integration, parallelized AI reviews, and static web deployment.

**Source credibility:** Highly detailed architecture suggests a mature, functional multi-agent system.

**Recency:** Current; demonstrates modern sub-agent orchestration and stateful workflow patterns.

**Source:** [jehyunlee/paper-curation/SKILL.md.template](https://github.com/jehyunlee/paper-curation/blob/67acecc780694d8442950f3a639a124617963514/SKILL.md.template) · 38★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: paper-curation
description: "최신 학술 논문 자동 큐레이션 풀 파이프라인. 검색 → Zotero 등록 → Paper Review → Deep Research 인덱스 빌드 → 정적 호스팅(GitHub Pages, Cloudflare Workers 등) 자동 배포까지 전체 실행. 트리거: '논문 큐레이션', '최신 논문 찾아줘', '논문 수집', 'paper curation', '오늘 나온 논문', '최신 논문 Zotero에', 'curate papers', '논문 모니터링', 'paper curation 배포해줘', '배포해줘'."
---

# Paper Curation — 최신 논문 자동 큐레이션 및 Zotero 등록

<Purpose>
특정 시기(기본: 지난 24시간)와 분야(기본: science of science, bibliometrics, scientometrics)의 최신 논문을 arXiv, Semantic Scholar, OpenAlex에서 자동 검색하고, 중복 제거 및 관련성 필터링 후 Zotero에 일괄 등록한다. 등록된 논문에 대해 paper-review를 실행하고, 토픽 인덱스와 Deep Research 검색 인덱스(`_search_index.json`)를 빌드한 뒤 정적 호스팅(GitHub Pages, Cloudflare Workers 등)에 `master` push로 자동 배포한다. **Phase 1~7 전체를 항상 실행한다 (부분 실행 없음).**
</Purpose>

<Use_When>
- "최신 논문 찾아줘", "오늘 나온 논문" 요청 시
- "논문 큐레이션", "논문 수집", "paper curation" 요청 시
- "최신 논문 Zotero에 넣어줘" 요청 시
- "논문 모니터링", "curate papers" 요청 시
- "paper curation 배포해줘", "배포해줘" 요청 시 → `prepare_deploy.py --topic {topic} --push` 실행
- 특정 분야의 최신 동향을 추적할 때
</Use_When>

<Do_Not_Use_When>
- 특정 논문 1편을 Zotero에 추가 → zotero-add 스킬 사용
- 논문 리뷰/분석 → paper-review 스킬 사용
- 보고서 작성용 논문 수집 → report-gen 스킬 사용
</Do_Not_Use_When>

<Why_This_Exists>
연구자는 자신의 분야
```

</details>
