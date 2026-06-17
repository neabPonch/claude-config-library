---
name: iosif2__carenet-cursor
source: https://github.com/iosif2/carenet-cursor/blob/c159cf39a05baff4c2527cdad74fae4b53282777/Skill.md
repo: iosif2/carenet-cursor
kind: skill
stars: 0
last_pushed: 2025-08-29T12:18:52Z
license: unknown
score: 8
domains: [web-frontend, state-management, api-integration]
tags: [react, nextjs, typescript, tanstack-query, business-logic]
curated: 2026-06-14
curated_by: config-scout
---

# iosif2/carenet-cursor — skill

**Why it's worth keeping:** It provides explicit API interaction patterns, such as specific TanStack Query mutation/invalidation sequences, which is crucial for agentic accuracy in state management.

**Summary:** A highly detailed technical specification outlining a Next.js/TypeScript frontend stack and granular business logic workflows.

**Source credibility:** The content shows high technical depth despite low repository visibility.

**Recency:** 

**Source:** [iosif2/carenet-cursor/Skill.md](https://github.com/iosif2/carenet-cursor/blob/c159cf39a05baff4c2527cdad74fae4b53282777/Skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 프론트엔드 기술 스택 및 구현 상세

## 1. 기술 스택

이 프로젝트의 프론트엔드 개발은 다음과 같은 핵심 기술 스택을 기반으로 합니다.

- **프레임워크**: React.js (Next.js 기반)
  - `use client` 지시어를 활용하여 클라이언트 컴포넌트 환경에서 풍부한 인터랙션 제공
- **언어**: TypeScript
  - 정적 타입 검사를 통해 코드의 안정성과 유지보수성 향상
- **상태 관리 및 데이터 페칭**: `@tanstack/react-query`
  - 서버 상태 관리를 효율적으로 처리하고 데이터 페칭, 캐싱, 동기화를 간소화
  - `useQuery`를 이용한 데이터 조회 및 `useMutation`을 이용한 데이터 변경 로직 구현
- **UI 컴포넌트**: Shadcn UI 기반 (Tailwind CSS, Radix UI)
  - 모던하고 반응형 UI를 빠르고 효율적으로 구축
  - Card, Dialog, Select, Table, Button, Input, Badge, Pagination 등 다양한 컴포넌트 활용
- **스타일링**: Tailwind CSS
  - 유틸리티-퍼스트 CSS 프레임워크로, 커스텀 스타일링을 신속하게 적용
- **토스트 알림**: `sonner`
  - 사용자 작업 결과에 대한 직관적인 알림 메시지 제공
- **아이콘**: `lucide-react`
  - 경량화된 아이콘 세트를 사용하여 시각적 요소 강화
- **쿠키 관리**: `js-cookie`
  - 클라이언트 측에서 `access_token`과 같은 쿠키 데이터를 간편하게 관리

## 2. 핵심 로직 및 백엔드 연동 사용자 시나리오

현재 구현된 주요 기능과 백엔드 연동 로직은 다음과 같습니다.

### 2.1. CCTV 관리 대시보드 (페이지 로드 시)

1.  **CCTV 정보 목록 조회**:
    - `InfoTable` 컴포넌트 마운트 시 `useQuery` 훅을 사용하여 `GET /api/v1/cctvs` 엔드포인트로부터 전체 CCTV 목록 정보를 비동기적으로 가져옵니다.
    - 가져온 데이터는 테이블 형태로 사용자에게 표시되며, 각 CCTV의 ID, 호실(병실) 이름, IP 주소, 환자 수 등을 포함합니다.
    - 인증을 위해 `js-cookie`로 관리되는 `access_token`이 `Authorization` 헤더에 포함됩니다.

### 2.2. 카메라 추
```

</details>
