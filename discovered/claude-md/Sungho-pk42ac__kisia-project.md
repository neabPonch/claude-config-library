---
name: Sungho-pk42ac__kisia-project
source: https://github.com/Sungho-pk42ac/kisia-project/blob/f9742e148a0ed336491ac51051df39a412469160/claude.md
repo: Sungho-pk42ac/kisia-project
kind: claude-md
stars: 1
last_pushed: 2026-01-03T12:01:33Z
license: apache-2.0
score: 9
domains: [backend-api, security, ai-architecture]
tags: [clean-architecture, ascii-diagrams, system-design]
curated: 2026-06-16
curated_by: config-scout
---

# Sungho-pk42ac/kisia-project — claude-md

**Why it's worth keeping:** It explicitly defines the separation of concerns across layers (Presentation/Application/Domain), which provides essential guardrails for an AI to avoid placing logic in the wrong directories.

**Summary:** A high-density technical blueprint featuring ASCII flow diagrams and a strict Clean Architecture folder hierarchy.

**Source credibility:** Single star, but content demonstrates professional-grade software engineering and architectural patterns.

**Recency:** Extremely current, referencing Python 3.13 and Next.js 15.

**Source:** [Sungho-pk42ac/kisia-project/claude.md](https://github.com/Sungho-pk42ac/kisia-project/blob/f9742e148a0ed336491ac51051df39a412469160/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DLP (Data Loss Prevention) 프로젝트 전체 아키텍처

> AI 기반 개인정보 탐지 및 차단 시스템
>
> **최종 업데이트:** 2025-11-04

---

## 목차

1. [프로젝트 개요](#프로젝트-개요)
2. [시스템 아키텍처](#시스템-아키텍처)
3. [백엔드 (DLP-BE)](#백엔드-dlp-be)
4. [프론트엔드 (Admin-FE)](#프론트엔드-admin-fe)
5. [프록시 (Proxy)](#프록시-proxy)
6. [통합 데이터 플로우](#통합-데이터-플로우)
7. [개발 워크플로우](#개발-워크플로우)
8. [주요 파일 경로](#주요-파일-경로)

---

## 프로젝트 개요

### 시스템 명칭
- **백엔드:** AI-TLS-DLP Backend v1.2.0
- **프론트엔드:** DS MASKING AI Admin Dashboard
- **프록시:** ChatGPT PII Detection Proxy

### 핵심 기능
1. **2단계 PII 탐지**
   - Stage 1: RoBERTa 기반 NER (Named Entity Recognition)
   - Stage 2: 정책 위반 탐지 (Policy Violation Detection)

2. **실시간 모니터링 대시보드**
   - 탐지 통계 및 시각화
   - 로그 관리 및 필터링
   - PII 설정 관리

3. **ChatGPT 트래픽 차단**
   - MITM 프록시를 통한 실시간 차단
   - 개인정보 포함 요청 자동 차단
   - SSE 형식 블록 응답 생성

### 기술 스택 요약

| 컴포넌트 | 핵심 기술 |
|---------|----------|
| **백엔드** | Python 3.13, FastAPI, PostgreSQL, Elasticsearch, PyTorch, RoBERTa |
| **프론트엔드** | Next.js 15, React 19, TypeScript, Tailwind CSS, Radix UI |
| **프록시** | Python 3.13, mitmproxy 12.1.1 |
| **인프라** | Docker, Docker Compose |

---

## 시스템 아키텍처

### 전체 구성도

```
┌─────────────────────────────────────────────────────────────────┐
│
```

</details>
