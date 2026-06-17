---
name: MapleEve__company-aitrack
source: https://github.com/MapleEve/company-aitrack/blob/3bba504f4957d3905f6132fe0e8c6fb26cf2af6b/CLAUDE.md
repo: MapleEve/company-aitrack
kind: claude-md
stars: 10
last_pushed: 2026-06-15T10:56:07Z
license: other
score: 9
domains: [monorepo, security-first, cli-tools, devops]
tags: [hierarchical, security-redlines, git-workflows]
curated: 2026-06-15
curated_by: config-scout
---

# MapleEve/company-aitrack — claude-md

**Why it's worth keeping:** Employs 'negative constraints' (security redlines) and provides exact terminal commands for specific environment quirks like proxy/git issues.

**Summary:** A hierarchical configuration for a multi-language monorepo that uses directory-specific sub-instructions to manage context scale.

**Source credibility:** Active repository with clear, professional-grade engineering standards.

**Recency:** Highly current; leverages advanced agentic context management through sub-directory routing.

**Source:** [MapleEve/company-aitrack/CLAUDE.md](https://github.com/MapleEve/company-aitrack/blob/3bba504f4957d3905f6132fe0e8c6fb26cf2af6b/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — company-aitrack

> Claude Code 执行规则。各子目录有对应 CLAUDE.md，进入子目录时自动加载。

## 仓库结构

| 路径 | 内容 | 详细规则 |
|------|------|---------|
| `client/` | Rust CLI（`aitrack` 二进制） | `client/CLAUDE.md` |
| `server-java/` | Java Spring Boot 服务端（主推） | `server-java/CLAUDE.md` |
| `server-go/` | Go chi 服务端（等价备选） | `server-go/CLAUDE.md` |
| `e2e/` | E2E 集成测试 | `e2e/CLAUDE.md` |
| `docker/` | Dockerfile × 3 + compose | `docker/CLAUDE.md` |
| `docs/` | 公开文档（ARCHITECTURE、API 等） | — |
| `CONTRACT.md` | 客户端/服务端协议 SSoT | — |
| `CHANGELOG.md` | 版本变更记录 | — |

内部 PRD / spec / roadmap 在 Codeup 仓库，不在本仓库。

---

## Git 规则

### main 分支保护

所有变更**必须通过 PR 合并**，禁止直接 push 到 main。

必须通过的 CI checks（9 个）：
`Lint·Rust` / `Lint·Go` / `Build&test·Go` / `Build&test·Java` / `Build&test·Rust` / `Coverage·Go` / `Coverage·Java` / `Coverage·Rust` / `E2E`

### push 必须绕过代理

本机 HTTPS 代理会导致 `LibreSSL SSL_ERROR_SYSCALL`，所有 push/fetch 必须：

```bash
git -c http.proxy="" -c https.proxy="" push origin <branch>
git -c http.proxy="" -c https.proxy="" fetch origin
```

### 分支生命周期

PR 合并或关闭后，对应分支**立即删除**（本地 + 远端）。

```bash
# 删除所有本地已合并分支（保留 main）
git branch | grep -v "^\* main" | xargs git branch -D

# 删除所有远端分支（保留 main）
git branch -r | grep
```

</details>
