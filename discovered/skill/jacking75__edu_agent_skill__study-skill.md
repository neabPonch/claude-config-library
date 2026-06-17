---
name: jacking75__edu_agent_skill__study-skill
source: https://github.com/jacking75/edu_agent_skill/blob/3bcf543e975aea7707cf46f62d7b01199e22fbb9/study_skill.md
repo: jacking75/edu_agent_skill
kind: skill
stars: 0
last_pushed: 2026-06-08T09:45:30Z
license: unknown
score: 9
domains: [agents-ai, developer-experience]
tags: [guide, skill-design, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# jacking75/edu_agent_skill — skill

**Why it's worth keeping:** It provides specific formulas for trigger-based descriptions and defines a critical three-tier context loading structure (Discovery/Activation/Execution) to prevent model saturation.

**Summary:** A highly technical guide for designing high-performance AI agent skills using the Progressive Disclosure architecture.

**Source credibility:** High; it offers precise technical specifications, naming conventions, and aligns with 2025 industry research.

**Recency:** Very high; incorporates the most recent 2025 data regarding AI code quality trends.

**Source:** [jacking75/edu_agent_skill/study_skill.md](https://github.com/jacking75/edu_agent_skill/blob/3bcf543e975aea7707cf46f62d7b01199e22fbb9/study_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# skill 학습  


## 1단계: 개념과 배경 이해

### 1-1. Skill이란 무엇인가
Skill은 AI 에이전트에게 특정 작업을 수행하는 방법을 가르치는 **지침 폴더**입니다. 핵심 파일인 `SKILL.md` 하나와 선택적 보조 파일들로 구성됩니다. Anthropic의 공식 가이드는 이것을 "신입 사원에게 건네는 업무 인수인계서"에 비유합니다. 한 번 작성해두면 세션이 바뀌어도, 팀원이 프로젝트를 클론해도 동일한 작업 품질이 유지됩니다.

Skill이 없을 때는 매 대화마다 "우리 프로젝트는 Next.js 15를 쓰고, ESLint 설정은 이렇고…"라고 반복 설명해야 합니다. Skill이 있으면 에이전트가 해당 매뉴얼을 자동으로 읽고 정해진 절차와 스타일대로 작업합니다.
  

### 1-2. Skill이 등장한 배경 — 바이브 코딩의 품질 문제
2025년 2월 Andrej Karpathy가 "바이브 코딩"이라는 용어를 만들었습니다. AI에게 자연어로 지시하고 생성된 코드를 그대로 수용하는 방식인데, 이 방식이 확산되면서 코드 품질 문제가 데이터로 드러났습니다.

학습해야 할 핵심 연구 결과는 다음과 같습니다.

**GitClear 보고서 (2025)**: 211백만 줄의 코드를 분석한 결과, AI 도입 이후 코드 중복이 4배 증가했고, 역사상 처음으로 복사/붙여넣기 코드가 리팩토링 코드를 초과했습니다.

**Carnegie Mellon 연구**: 807개 GitHub 저장소에서 Cursor 도입 이후 정적 분석 경고가 30% 증가하고 코드 복잡도가 41% 증가했습니다. 속도 향상은 일시적이었지만 품질 문제는 누적되었습니다.

**Google DORA 보고서 (2025)**: AI 도입과 소프트웨어 전달 안정성 사이에 부정적 상관관계가 있었습니다. 핵심 결론은 "AI는 팀을 고치지 않는다. 이미 있는 것을 증폭시킨다"는 것이었습니다.

**Anthropic Agentic Coding Trends**: 개발자가 업무의 약 60%에 AI를 사용하지만, 완전히 위임할 수 있는 작업은 0~20%에 불과합니다. 나머지는 "사려 깊은 설정, 적극적인 감독, 인간의 판단"이 필요합니다.

이 "설정"과 "감독"을 코드화한 것이 바로 Skill입니다. AI가 빠르게 생산하는 코드에 품질 가드레일을 씌우는 역할을 합니다.
  

### 1-3. AI가 반복하는 전형적인 코드 문제 패턴
Skill이 해결하려는 구
```

</details>
