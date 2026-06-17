---
name: unicorn-plugins__npd__skill
source: https://github.com/unicorn-plugins/npd/blob/051ff80a5106f4ada3f88db37aa72172a38e8b30/skills/cicd/SKILL.md
repo: unicorn-plugins/npd
kind: skill
stars: 20
last_pushed: 2026-05-26T12:17:22Z
license: unknown
score: 9
domains: [devops, cicd, gitops, orchestration]
tags: [argocd, jenkins, state-management, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# unicorn-plugins/npd — skill

**Why it's worth keeping:** Uses a robust state-persistence pattern via AGENTS.md to enable progress tracking and seamless workflow resumption. Employs highly structured variable mapping and clear phase/step hierarchies for reliable agent orchestration.

**Summary:** A sophisticated orchestrator for multi-phase CI/CD and GitOps (ArgoCD) infrastructure deployment. It manages complex sub-agent tasks including tool installation, environment detection, and service-specific pipeline creation.

**Source credibility:** Niche specialized plugin with moderate social proof (20 stars).

**Recency:** Very current, following modern GitOps and AI-driven infrastructure patterns.

**Source:** [unicorn-plugins/npd/skills/cicd/SKILL.md](https://github.com/unicorn-plugins/npd/blob/051ff80a5106f4ada3f88db37aa72172a38e8b30/skills/cicd/SKILL.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cicd
description: CI/CD 파이프라인 구성 AI 협업 -- DevOps 엔지니어가 Jenkins/GitHub Actions CI + ArgoCD CD 파이프라인 구축
type: orchestrator
user-invocable: true
---

# CI/CD

[NPD CI/CD 활성화]

## 목표

DevOps 엔지니어가 CI/CD 파이프라인 코드(Jenkinsfile, GitHub Actions Workflow, Kustomize 매니페스트)를 생성하고,
ArgoCD GitOps 방식으로 CD를 분리하는 파이프라인을 구축한다.

## 활성화 조건

사용자가 `/npd:cicd` 호출 시 또는 "CICD 시작", "CI/CD 구성", "파이프라인 작성", "자동 배포" 키워드 감지 시.

주의사항: 중간 단계부터 시작할 때도 진행 모드 결정 + 환경 정보 수집을 위해 Phase 0은 항상 수행해야 합니다.

## 선행 조건

- `/npd:create` 완료 (프로젝트 디렉토리 및 AGENTS.md 존재)
- `/npd:deploy` Phase 5 (K8s 배포)까지 완료된 상태 (기존 K8s 매니페스트 `deployment/k8s/` 존재)
- CI/CD 도구 설치: Phase 1에서 자동 설치 또는 사전 설치 완료 (CI 도구, SonarQube, ArgoCD, Image Registry Credential)

## 작업 환경 변수 로드

AGENTS.md 파일에서 `## 환경변수` 섹션의 환경변수 로딩.
로딩 실패 시 사용자에게 `/npd:create`을 먼저 수행하라고 안내하고 종료.

## 에이전트 호출 규칙

| 에이전트 | FQN |
|----------|-----|
| devops-engineer | `npd:devops-engineer:devops-engineer` |

### 프롬프트 조립

- `{NPD_PLUGIN_DIR}/resources/guides/combine-prompt.md`에 따라
  AGENT.md + agentcard.yaml + tools.yaml 합치기
- `Agent(subagent_type=FQN, model=tier_mapping 결과, prompt=조립된 프롬프트)` 호출
- tier → 모델 매핑은 `{NPD_PLUGIN_DIR}/gateway/runtime-mapping.yaml` 참조

### 서브 에이전트 호출

워크
```

</details>
