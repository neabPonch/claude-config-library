---
name: kyirexy__DesignSystem-Pro-Max-skill
source: https://github.com/kyirexy/DesignSystem-Pro-Max-skill/blob/bab7871af7b5e627be85502668b86bb922a16c10/CLAUDE.md
repo: kyirexy/DesignSystem-Pro-Max-skill
kind: claude-md
stars: 1
last_pushed: 2026-01-02T02:06:48Z
license: unknown
score: 8
domains: [cli-tools, design-system, frontend]
tags: [CLI, Automation, Design System]
curated: 2026-06-15
curated_by: config-scout
---

# kyirexy/DesignSystem-Pro-Max-skill — claude-md

**Why it's worth keeping:** It effectively documents 'skills'—specific command patterns with arguments that empower the AI agent to perform complex domain-specific tasks autonomously.

**Summary:** Provides highly structured documentation for a CLI-driven design system toolkit used to search, generate, and audit UI specifications.

**Source credibility:** Low star count/unproven source, but technical content is highly structured and professional.

**Recency:** Very current; explicitly tailors instructions for Claude Code functionality.

**Source:** [kyirexy/DesignSystem-Pro-Max-skill/CLAUDE.md](https://github.com/kyirexy/DesignSystem-Pro-Max-skill/blob/bab7871af7b5e627be85502668b86bb922a16c10/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

**This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.**
<br>**本文件为 Claude Code (claude.ai/code) 在此仓库中工作时提供指导。**

---

## Project Overview / 项目概述

**DesignSystem-Pro-Max** provides searchable design system specifications for AI coding assistants.
<br>**DesignSystem-Pro-Max** 为 AI 编码助手提供可搜索的设计系统规范。

It supports multiple UI frameworks (AntD, Material-UI, Figma, Bootstrap, Tailwind, Chakra, Elements) with capabilities for searching specs, generating compliant code, and auditing compliance.
<br>它支持多种 UI 框架（AntD、Material-UI、Figma、Bootstrap、Tailwind、Chakra、Elements），具有搜索规范、生成符合规范的代码和审计合规性的功能。

---

## Quick Start / 快速开始

```bash
# Search design specifications / 搜索设计规范
python3 .claude/skills/ds-pro-max/scripts/search.py "<query>" --domain <domain> --stack <stack>

# Generate compliant CSS code / 生成符合规范的 CSS 代码
python3 .claude/skills/ds-pro-max/scripts/generate.py "<query>" --stack <stack> --output <file.css>

# Audit CSS for compliance / 审计 CSS 合规性
python3 .claude/skills/ds-pro-max/scripts/audit.py <file.css> --stack <stack>
```

---

## Available Domains / 可用领域

- `component` - UI component specs / UI 组件规范 (Button, Input, Mod
```

</details>
