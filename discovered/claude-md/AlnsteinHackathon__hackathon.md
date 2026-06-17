---
name: AlnsteinHackathon__hackathon
source: https://github.com/AlnsteinHackathon/hackathon/blob/c08623a84f3ce789d9451a209890e75dab4c3af6/Claude.md
repo: AlnsteinHackathon/hackathon
kind: claude-md
stars: 0
last_pushed: 2025-10-26T15:59:39Z
license: unknown
score: 9
domains: [full-stack, web-frontend, backend-api]
tags: [workflow-optimization, tool-mapping, standard-operating-procedure]
curated: 2026-06-15
curated_by: config-scout
---

# AlnsteinHackathon/hackathon — claude-md

**Why it's worth keeping:** Features a brilliant 'Document Index' to reduce agent uncertainty and provides explicit mappings of business scenarios to specific Claude Code tools.

**Summary:** A comprehensive operational manual that bridges high-level requirements with specific technical execution patterns and tool usage.

**Source credibility:** Low social proof on GitHub, but the internal structure demonstrates highly disciplined engineering practices.

**Recency:** Highly current; reflects modern agentic workflows with tool-specific instructions like apply_diff usage.

**Source:** [AlnsteinHackathon/hackathon/Claude.md](https://github.com/AlnsteinHackathon/hackathon/blob/c08623a84f3ce789d9451a209890e75dab4c3af6/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI 工作指南

> AutoAnime 项目的 AI 协作规范 - 简洁版

**版本**: v1.0  
**更新日期**: 2025-10-25

---

## 🚨 核心原则

1. **📖 文档优先**：不确定时先查阅项目文档（PRD.md / 技术文档.md / UI设计.md）
2. **🎯 小步前进**：复杂任务必须分解，使用 `update_todo_list` 跟踪进度
3. **✅ 等待确认**：每次工具使用后等待用户确认，不要假设成功
4. **🔍 理解上下文**：修改前先读取相关文件，一次最多读5个
5. **💡 保持一致**：遵循项目现有代码风格和模式
6. **🛡️ 安全第一**：输入验证、错误处理、权限控制不可省略
7. **📝 小提交**：每个commit < 200行，1-5个文件，单一功能点

---

## 项目上下文

### 技术栈
```
前端：React 18 + TypeScript + Zustand + Ant Design
后端：Go + Gin + MongoDB + Redis
AI：Claude + veo-3.1 + 七牛云TTS
```

### 项目结构
```
backend/internal/app/     # 后端核心业务
  ├── config/            # 配置
  ├── handler/           # HTTP处理器
  ├── service/           # 业务逻辑
  ├── models/            # 数据模型
  └── worker/            # 任务处理

frontend/src/
  ├── pages/             # 页面组件
  ├── services/          # API服务
  ├── stores/            # 状态管理
  └── utils/             # 工具函数
```

### 文档索引
| 问题 | 查阅文档 |
|------|---------|
| 功能需求 | [`PRD.md`](PRD.md) |
| 技术实现 | [`技术文档.md`](技术文档.md) |
| UI规范 | [`UI设计.md`](UI设计.md) |
| API接口 | [`IMPLEMENTATION_SUMMARY.md`](IMPLEMENTATION_SUMMARY.md) |
| 快速启动 | [`START_HERE.md`](START_HERE.md) |

---

## 工作流程

### 标准流程
```
1. 理解需求 → 查阅相关文档
2. 分析上下文 → 读取相关代码（一次最多5个文件）
3
```

</details>
