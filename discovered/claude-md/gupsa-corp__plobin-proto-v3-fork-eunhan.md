---
name: gupsa-corp__plobin-proto-v3-fork-eunhan
source: https://github.com/gupsa-corp/plobin-proto-v3-fork-eunhan/blob/06dde985a599969e4ace86223d740c68e0c17a96/CLAUDE.md
repo: gupsa-corp/plobin-proto-v3-fork-eunhan
kind: claude-md
stars: 0
last_pushed: 2025-09-16T07:50:43Z
license: unknown
score: 8
domains: [backend-api, web-frontend, laravel]
tags: [naming-conventions, architectural-constraints, opinionated-workflow]
curated: 2026-06-15
curated_by: config-scout
---

# gupsa-corp/plobin-proto-v3-fork-eunhan — claude-md

**Why it's worth keeping:** The technique of using numerical prefixes for files and mandatory folder-based controller paths provides the AI with an unambiguous blueprint that prevents style drift. It effectively eliminates ambiguity in how many files should exist and where they must live.

**Summary:** This config establishes hyper-specific architectural constraints and naming conventions for a Laravel/Livewire stack. It dictates exact file structures for both frontend components and backend controllers to ensure absolute consistency.

**Source credibility:** Low public social proof (0 stars), but high internal detail suggests a mature, opinionated development workflow.

**Recency:** Current; explicitly mentions Laravel 11.

**Source:** [gupsa-corp/plobin-proto-v3-fork-eunhan/CLAUDE.md](https://github.com/gupsa-corp/plobin-proto-v3-fork-eunhan/blob/06dde985a599969e4ace86223d740c68e0c17a96/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Plobin Proto V3 개발 가이드

계정 : admin@example.com
비번 : password

## 최우선 준수 규칙

### 파일 구조 및 URL 설계 규칙
**modal, dropdown, table, block 급 컴포넌트는 무조건 파일 분리**
- 올바른 예: `200-modal-user-edit.blade.php`, `200-dropdown-menu.blade.php`, `200-table-users.blade.php`
- 잘못된 예: 큰 파일 안에 모달, 드롭다운, 테이블 코드 섞어 놓기
- **원칙**: 재사용 가능한 모든 UI 컴포넌트는 독립 파일로 분리

**page 급은 무조건 폴더별로 분리**
- 올바른 예: `903-page-users/000-index.blade.php`, `903-page-users/100-header-main.blade.php`
- 잘못된 예: 하나의 파일에 전체 페이지 구조 작성
- **원칙**: 각 페이지는 독립된 폴더에 header, sidebar, content 등으로 분리

**탭이 들어가는 화면은 무조건 페이지 URL을 분기처리해서 web.php에 경로 추가**
- 올바른 예: `/admin/users/overview`, `/admin/users/roles`, `/admin/users/permissions`
- 잘못된 예: 하나의 URL에서 JavaScript로만 탭 처리
- **원칙**: 각 탭마다 고유 URL과 라우트를 가져야 함 (SEO, 북마크, 뒤로가기 지원)

### 기술 스택 제한
**순수 JavaScript 사용 금지**
사용 금지: Vanilla JS, jQuery, Alpine.js의 복잡한 로직
사용 필수: Livewire + Filament 조합만 사용
모든 상호작용과 동적 기능은 다음으로만 구현:
- Livewire: 서버사이드 상태관리, 이벤트 처리
- Filament: UI 컴포넌트, 폼, 테이블 등
- 간단한 Alpine.js: 토글, 드롭다운 등 최소한의 UI 상호작용만

JavaScript가 필요한 경우 → Livewire로 재작성 필수
복잡한 UI가 필요한 경우 → Filament 컴포넌트 사용

## 프론트엔드 개발 규칙

### 파일 구조 및 네이밍
**절대 원칙**: 모든 프론트엔드 파일은 **무조건** 숫자 접두사 사용
- 올바른 예: `700-page-dashboard.blade.php`, `30
```

</details>
