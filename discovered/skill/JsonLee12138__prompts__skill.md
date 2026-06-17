---
name: JsonLee12138__prompts__skill
source: https://github.com/JsonLee12138/prompts/blob/b03ef762582b1c6772c532b2bfc06cf84f379603/skills/makefile/SKILL.md
repo: JsonLee12138/prompts
kind: skill
stars: 2
last_pushed: 2026-05-11T07:20:36Z
license: apache-2.0
score: 8
domains: [cli-tools, devops, backend]
tags: [makefile, automation, validation]
curated: 2026-06-15
curated_by: config-scout
---

# JsonLee12138/prompts — skill

**Why it's worth keeping:** The inclusion of a 'Validate' mode is excellent; it transforms the agent from a writer into a linter that ensures compliance with specific standards like .PHONY usage and help-target syntax.

**Summary:** Provides a structured workflow for generating and auditing self-documenting Makefiles with 'make help' capabilities. It includes specific logic for project type detection and a strict validation rubric.

**Source credibility:** Low star count but highly structured, high-signal content suggests an intentional developer tool.

**Recency:** Very recent (1 month ago) and uses modern dev-ops conventions.

**Source:** [JsonLee12138/prompts/skills/makefile/SKILL.md](https://github.com/JsonLee12138/prompts/blob/b03ef762582b1c6772c532b2bfc06cf84f379603/skills/makefile/SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: makefile
description: "Use when creating, editing, or validating Makefiles. Provides templates for Go, Node, Python, Docker, and Monorepo projects with self-documenting help targets. Also validates existing Makefiles against conventions. Triggers on: Makefile, makefile, make help, validate makefile, lint makefile."
---

# Makefile Skill

## Overview

Makefile 模板生成与验证工具。支持两种模式：

1. **Generate** — 根据项目类型生成标准化 Makefile 模板
2. **Validate** — 检查现有 Makefile 是否符合规范

核心原则：**注释即文档，`make` 即入口。**

## Mode Selection

```
用户说 "创建/生成 Makefile" → Generate 模式
用户说 "validate/检查/lint Makefile" → Validate 模式
用户未明确 → 询问选择
```

---

## Generate 模式

### Template Selection

根据项目类型选择模板。如果用户未指定，通过以下方式自动检测：

1. 检查 `go.mod` → Go 模板
2. 检查 `package.json` → Node 模板
3. 检查 `pyproject.toml` 或 `setup.py` → Python 模板
4. 检查 `docker-compose.yml` → Docker 模板
5. 检查 `pnpm-workspace.yaml` 或 `lerna.json` → Monorepo 模板
6. 无法检测 → 询问用户选择

### Available Templates

| 模板 | 文件 | 适用场景 |
|------|------|----------|
| Go | `assets/Makefile.go.tmpl` | Go 项目，含 build/test/lint/docker |
| Node | `assets/Makefile.node.tmpl` | Node.js/TypeScript，自动检测包管理器 |
| Python | `assets/Makefile.python.tmpl` | Python 项目，含 venv/pytest/ruff |
|
```

</details>
