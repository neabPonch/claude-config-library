---
name: vietlinhh02__interviewx
source: https://github.com/vietlinhh02/interviewx/blob/6c1075583ce7459c3b1e595f60ca82ae116f821d/CLAUDE.MD
repo: vietlinhh02/interviewx
kind: claude-md
stars: 0
last_pushed: 2026-04-18T19:29:33Z
license: unknown
score: 7
domains: [backend-api, go]
tags: [short, go, monorepo]
curated: 2026-06-14
curated_by: config-scout
---

# vietlinhh02/interviewx — claude-md

**Why it's worth keeping:** Introduces a specific code citation format (startLine:endLine:path) and mandates verification through compilation/testing before completion.

**Summary:** Provides critical architectural context for a Go monorepo, specifically focusing on database migration safety and testing requirements.

**Source credibility:** Low visibility (0 stars), but demonstrates professional-grade structural instructions.

**Recency:** Current; last pushed 2 months ago.

**Source:** [vietlinhh02/interviewx/CLAUDE.MD](https://github.com/vietlinhh02/interviewx/blob/6c1075583ce7459c3b1e595f60ca82ae116f821d/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude — ngữ cảnh dự án InterviewX

Khi làm việc trong repo này, đọc **`agent.md`** (cùng thư mục gốc) để biết stack, cấu trúc và quy ước.

## Tóm tắt nhanh

- Monorepo **Go API**; không có frontend trong repo này.
- Luồng nghiệp vụ tuyển dụng: `internal/workflow` + `internal/repo` + handler trong `internal/httpapi`.
- Mọi thay đổi schema: thêm file `migrations/00000N_*.sql`, không sửa file migration đã apply production (trừ khi user chủ động yêu cầu).

## Claude nên làm

- **Research trước:** đọc code + `docs/` liên quan; tra cứu doc chính thức hoặc nguồn đáng tin khi chạm API/phiên bản lạ — xem mục *Research* trong [agent.md](./agent.md). Không chốt thiết kế chỉ từ trí nhớ.
- Chạy `go build ./...` và `go test ./...` trước khi báo xong (trừ khi môi trường thiếu Go).
- Trích dẫn code bằng format ```startLine:endLine:path``` khi giải thích thay đổi.
- Ưu tiên thư viện **open source** đã ghi trong `docs/agents/opensource-implementation.md` thay vì tự viết tương đương.

## Claude không nên

- Mở rộng scope (UI, agent LLM đầy đủ, đổi framework HTTP) khi user chỉ hỏi sửa nhỏ.
- Xóa hoặc làm mất tương thích migration / tenant isolation.

## Liên kết

- [agent.md](./agent.md) — hướng dẫ
```

</details>
