---
name: domelic__architecture-of-thought
source: https://github.com/domelic/architecture-of-thought/blob/54edd7bff008efae17843bd765f6652b6da7296d/CLAUDE.md
repo: domelic/architecture-of-thought
kind: claude-md
stars: 15
last_pushed: 2026-04-13T14:48:25Z
license: other
score: 9
domains: [latex, ai-agents, documentation]
tags: [cognitive-frameworks, slash-commands, context-management, workflow-automation]
curated: 2026-06-16
curated_by: config-scout
---

# domelic/architecture-of-thought — claude-md

**Why it's worth keeping:** It treats the AI as a thinker by defining 'Available Skills' (e.g., /dcf) for structured Socratic dialogue, rather than just listing file paths; it also provides proactive strategies for session continuity and context management.

**Summary:** Defines high-level cognitive frameworks and custom slash commands to guide AI reasoning behavior within a complex document hierarchy.

**Source credibility:** High-quality repository demonstrating deep architectural/philosophical thought with recent updates.

**Recency:** Highly current; incorporates advanced Claude Code patterns like MCP integration and custom skill definitions.

**Source:** [domelic/architecture-of-thought/CLAUDE.md](https://github.com/domelic/architecture-of-thought/blob/54edd7bff008efae17843bd765f6652b6da7296d/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repository contains **"The Architecture of Thought"** — a treatise presenting the Dialectical Cognition Framework (DCF), a methodology for human-AI collaboration. The main output is a ~267-page LaTeX document (split into chapters) with supporting practical resources in Markdown.

**Read DCF_ESSENTIALS.md first** to understand the core concepts, Socratic toolkit, and 24 modes.

## Commands Quick Reference

| Task | Command |
|------|---------|
| Quick LaTeX compile | `pdflatex THE_ARCHITECTURE_OF_THOUGHT.tex` |
| Full LaTeX build | See [Full Compilation](#latex-compilation) below |
| Spell check all | `cspell --config .cspell.json "**/*.md" --no-progress` |
| Lint all markdown | `markdownlint-cli2 "**/*.md" --config .markdownlint.json --ignore CHANGELOG.md` |
| Single file validation | `cspell --config .cspell.json "file.md" && markdownlint-cli2 "file.md"` |

**Dependencies:** TeX Live 2025 or MacTeX for LaTeX; `npm install -g cspell markdownlint-cli2` for validation.

## Build & Validation Commands

### LaTeX Compilation

```bash
# Quick com
```

</details>
