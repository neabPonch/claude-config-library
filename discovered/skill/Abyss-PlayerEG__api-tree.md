---
name: Abyss-PlayerEG__api-tree
source: https://github.com/Abyss-PlayerEG/api-tree/blob/80b64ef5d6e38bf86aa37d2efd57b5a2a339357a/skill.md
repo: Abyss-PlayerEG/api-tree
kind: skill
stars: 3
last_pushed: 2026-06-01T05:55:06Z
license: unknown
score: 9
domains: [backend-api, cli-tools, agents-ai]
tags: [openapi, rag, agent-optimized]
curated: 2026-06-14
curated_by: config-scout
---

# Abyss-PlayerEG/api-tree — skill

**Why it's worth keeping:** It uses an advanced 'Decision Tree' and intent recognition table to instruct the agent on when to switch from human-centric visual output to machine-optimized structural output (--agent-output).

**Summary:** Provides a highly structured skill definition for the api-tree CLI to assist agents in exploring OpenAPI documentation.

**Source credibility:** Low star count, but exceptionally high quality of tool-documentation and agent-instruction logic.

**Recency:** Very current; includes modern RAG (Retrieval-Augmented Generation) chunking and agent-optimization patterns.

**Source:** [Abyss-PlayerEG/api-tree/skill.md](https://github.com/Abyss-PlayerEG/api-tree/blob/80b64ef5d6e38bf86aa37d2efd57b5a2a339357a/skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
iyang---
name: api-tree
description: 使用 api-tree CLI 工具查看和搜索 OpenAPI/Swagger 接口的终端树状图。当用户需要查看 API 接口结构、路由树、搜索特定 API 路径/端点，或提到 "api-tree"、"接口树"、"API 树"、"路由列表"、"swagger 接口"、"openapi 接口"、"查看接口"、"API 端点"、"接口结构"、"show api routes" 时使用。
---

# api-tree

在终端中以彩色树状图展示 OpenAPI 接口结构，支持搜索和过滤。支持多种输出格式，包括为 LLM Agent 优化的输出和 RAG 知识库输出。

## 命令

| 命令 | 说明 |
|------|------|
| `api-tree` | 默认连接 `http://localhost:8080`，自动追加 `/v3/api-docs` |
| `api-tree <url>` | 连接指定 OpenAPI 文档地址 |
| `api-tree <file.json>` | 读取本地 OpenAPI JSON 文件 |
| `api-tree <url> -s <keyword>` | 搜索含关键词的路径/方法/摘要 |
| `api-tree <url> --html` | 同时导出带主题切换的 HTML 文件 |
| `api-tree <url> --agent-output <format>` | 为 LLM Agent 优化的输出（markdown/json/curl） |
| `api-tree <url> --rag-output <format>` | 为 RAG 知识库优化的输出（jsonl/json） |
| `api-tree <url> --rag-chunk-size <n>` | 设置 RAG 切片大小（默认 10 个端点） |
| `api-tree --init-config` | 生成默认配置文件 |
| `api-tree --show-config` | 显示当前配置 |
| `api-tree -h` | 查看帮助 |

## 参数

- **位置参数**: OpenAPI 文档的 URL 或本地 JSON 文件路径。若 URL 不含具体路径（以 `/` 结尾或无路径），自动追加 `/v3/api-docs`。
- **`-s <keyword>`**: 搜索过滤（不区分大小写），匹配路径、摘要或 HTTP 方法。
- **`--html`**: 额外生成 HTML 文件，内置 Catppuccin 浅色/暗色主题切换。输出目录可通过配置文件自定义。
- **`--init-config`**: 在 `~/.config/a
```

</details>
