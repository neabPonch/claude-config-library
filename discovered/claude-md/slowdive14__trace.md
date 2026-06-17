---
name: slowdive14__trace
source: https://github.com/slowdive14/trace/blob/10b30176d8cadede9b90ee10186ef78c5da6fd98/claude.md
repo: slowdive14/trace
kind: claude-md
stars: 0
last_pushed: 2026-06-10T02:43:25Z
license: unknown
score: 9
domains: [web-frontend, firebase, typescript]
tags: [schema-heavy, comprehensive-context, business-logic]
curated: 2026-06-16
curated_by: config-scout
---

# slowdive14/trace — claude-md

**Why it's worth keeping:** It provides explicit TypeScript interfaces and Firestore collection hierarchies that allow Claude to perform complex CRUD operations without needing to constantly scan the codebase for types or schema structures.

**Summary:** A comprehensive technical blueprint covering component roles, detailed data schemas (TypeScript), and specific business logic for a React/Firebase application.

**Source credibility:** Personal project with low social proof but exceptionally high-quality technical documentation.

**Recency:** Current; uses modern patterns suitable for Claude Code.

**Source:** [slowdive14/trace/claude.md](https://github.com/slowdive14/trace/blob/10b30176d8cadede9b90ee10186ef78c5da6fd98/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

# Serein: AI 기반 지능형 일상 기록 & 가계부 관리

## 🔧 개발 명령어

```bash
# 개발 서버 실행 (기본 포트: 5173)
npm run dev

# 프로덕션 빌드 (TypeScript 컴파일 + Vite 빌드)
npm run build

# 빌드 결과 미리보기
npm run preview

# ESLint로 코드 검사
npm run lint
```

## 📱 앱 개요
✨ "맑은 날 저녁에 내리는 비" - Serein
Serein은 Firebase를 기반으로 하는 지능형 일상 기록 및 가계부 관리 앱입니다. 사용자는 시간대별로 일상 활동(action)과 생각(thought)을 기록하고 관리할 수 있으며, AI(Gemini API)를 활용한 지출 자동 분류 및 통계 분석을 통해 재정 상태를 효과적으로 파악할 수 있습니다. 통합 캘린더와 타임라인 뷰를 통해 모든 기록을 한눈에 확인하고, Obsidian 마크다운 내보내기 기능을 통해 소중한 기록을 외부에서도 유연하게 활용할 수 있습니다.

## 🏗️ 프로젝트 구조

```
trace/
├── src/
│   ├── components/          # React 컴포넌트
│   │   ├── AuthContext.tsx   # 인증 컨텍스트
│   │   ├── CalendarView.tsx  # 캘린더 뷰
│   │   ├── EntryItem.tsx     # 개별 엔트리 항목
│   │   ├── InputBar.tsx      # 입력창 (일상/생각/할일)
│   │   ├── Layout.tsx        # 레이아웃
│   │   ├── SearchBar.tsx     # 검색 바
│   │   ├── Timeline.tsx      # 타임라인 메인 뷰
│   │   ├── TodoTab.tsx       # 할일 탭
│   │   ├── ExpenseCalendar.tsx    # 가계부 캘린더 (접기/펼치기)
│   │   ├── ExpenseInput.tsx       # 가계부 입력창
│   │   ├── ExpenseInsights.tsx    # 가계부 통계/인사이트
│   │   ├── ExpenseTime
```

</details>
