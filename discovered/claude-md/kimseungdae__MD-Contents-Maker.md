---
name: kimseungdae__MD-Contents-Maker
source: https://github.com/kimseungdae/MD-Contents-Maker/blob/1c9df5c21d8cdb42e9294be00384a1f4de6918af/CLAUDE.MD
repo: kimseungdae/MD-Contents-Maker
kind: claude-md
stars: 0
last_pushed: 2025-06-20T08:06:01Z
license: unknown
score: 8
domains: [web-frontend, educational-tech]
tags: [vue-3, typescript, technical-spec]
curated: 2026-06-17
curated_by: config-scout
---

# kimseungdae/MD-Contents-Maker — claude-md

**Why it's worth keeping:** Provides explicit TypeScript interfaces and CSS design tokens which ensure the AI maintains strict type safety and visual consistency across components.

**Summary:** A comprehensive technical specification for a Vue 3/TypeScript educational content creation system.

**Source credibility:** Low; repository has no stars and hasn't been updated in 12 months.

**Recency:** Current; uses modern Vue 3, Vite, and Tailwind patterns.

**Source:** [kimseungdae/MD-Contents-Maker/CLAUDE.MD](https://github.com/kimseungdae/MD-Contents-Maker/blob/1c9df5c21d8cdb42e9294be00384a1f4de6918af/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 초등학생 대상 디지털 학습 콘텐츠 제작 시스템

## 🎯 프로젝트 목표
20~40대 교사들이 **코딩 지식 없이** 직관적인 GUI를 통해 초등학생(1~6학년) 대상의 인터랙티브 학습 콘텐츠를 쉽게 제작할 수 있는 시스템 개발

## 🏗️ 시스템 아키텍처

### 1. 교사용 콘텐츠 작성기 (Teacher Content Creator)
- **대상 사용자**: 20~40대 교사 (IT 숙련도 중급 이하)
- **핵심 원칙**: 직관적, 시각적, 간편함
- **기술 스택**: Vue 3 + Composition API + TypeScript + Tailwind CSS + Pinia

### 2. 학습자용 콘텐츠 플레이어 (Student Content Player)
- **대상 사용자**: 초등학생 1~6학년
- **핵심 원칙**: 반응형, 터치 친화적, 고성능
- **기술 스택**: Vue 3 + Canvas API + MathJax/KaTeX

## 📋 핵심 기능 요구사항

### A. 교사 친화적 UI/UX 필수 요소
1. **직관적 드래그 앤 드롭 인터페이스**
   - 왼쪽 모듈 팔레트에서 오른쪽 문제 캔버스로 드래그
   - 시각적 피드백 (드롭존 하이라이트, 애니메이션)
   - 실시간 미리보기

2. **사용자 친화적 네비게이션**
   - 문제 목록 → 문제 편집 → 미리보기 → 저장의 직관적 플로우
   - 브레드크럼 네비게이션
   - 저장되지 않은 변경사항 경고

3. **수려한 모던 UI 디자인**
   - Material Design 3 또는 Apple Human Interface Guidelines 스타일
   - 일관된 색상 팔레트 (교육용 친화적 색상)
   - 적절한 여백과 타이포그래피
   - 다크모드 지원

### B. 문제 관리 시스템 (CRUD)
```typescript
interface Problem {
  id: string;
  title: string;
  question: string;
  grade: 1 | 2 | 3 | 4 | 5 | 6;
  subject: '수학' | '국어' | '과학' | '사회';
  modules: Module[];
  createdAt: Date;
  updatedAt: Date;
  tags: string[];
  difficulty: 'easy' | 'medium' | 'hard';
}
```

**필수 기능:**
1. **문제
```

</details>
