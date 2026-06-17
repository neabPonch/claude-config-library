---
name: CronusL-1141__AI-company
source: https://github.com/CronusL-1141/AI-company/blob/ec580d32e86fa9cdaa55afb4adb2d0b732ed222c/CLAUDE.md
repo: CronusL-1141/AI-company
kind: claude-md
stars: 188
last_pushed: 2026-06-12T19:59:50Z
license: mit
score: 7
domains: [agents-ai, backend-api]
tags: [role-based, architecture-enforcement]
curated: 2026-06-14
curated_by: config-scout
---

# CronusL-1141/AI-company — claude-md

**Why it's worth keeping:** Demonstrates how to use role-based instructions (Leader behavior) and single-source-of-truth enforcement (type sharing rules).

**Summary:** Defines high-level persona behaviors and strict architectural constraints for a multi-agent system.

**Source credibility:** High; 188 stars and recent activity suggest an active, popular project.

**Recency:** Very current; utilizes latest tech stacks like Python 3.12 and React 19.

**Source:** [CronusL-1141/AI-company/CLAUDE.md](https://github.com/CronusL-1141/AI-company/blob/ec580d32e86fa9cdaa55afb4adb2d0b732ed222c/CLAUDE.md) · 188★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Team OS

**技术栈**: Python 3.12 + FastAPI | React 19 + Vite | SQLite
**架构**: Storage → API → Dashboard（详见 docs/architecture.md）

## 核心约束
- 所有输出使用中文
- 共享类型只引用 `src/aiteam/types.py`
- 代码风格: PEP 8，类型注解，async优先

## Leader核心行为
- 专注统筹，实施工作委派团队成员
- 新需求先加入任务墙，系统级功能先写设计文档
- 完整规则通过SessionStart自动注入，也可查询 GET /api/system/rules
```

</details>
