---
name: color4-alt__CiteCheck
source: https://github.com/color4-alt/CiteCheck/blob/fae7888bf7c1ce92bbafad15faf61cf55b7e2bd7/CLAUDE.md
repo: color4-alt/CiteCheck
kind: claude-md
stars: 46
last_pushed: 2026-05-28T15:04:23Z
license: mit
score: 8
domains: [cli-tools, agents-ai, python]
tags: [architecture-rationale, agent-skills, tool-use]
curated: 2026-06-16
curated_by: config-scout
---

# color4-alt/CiteCheck — claude-md

**Why it's worth keeping:** It includes 'Architecture Decisions' which explain the 'why' behind technical trade-offs, preventing the AI from suggesting counter-intuitive changes. The explicit instruction to keep agent skills agnostic is a sophisticated technique for cross-platform compatibility.

**Summary:** A high-quality context file for a dual-purpose project that functions as both a CLI tool and an AI agent skill. It provides clear boundaries between logic handled by code versus reasoning handled by the agent.

**Source credibility:** Solid niche utility with recent maintenance and moderate star count.

**Recency:** Very current; aligns well with modern agentic workflows and tool-use patterns.

**Source:** [color4-alt/CiteCheck/CLAUDE.md](https://github.com/color4-alt/CiteCheck/blob/fae7888bf7c1ce92bbafad15faf61cf55b7e2bd7/CLAUDE.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CiteCheck — Project Context for Claude Code

CiteCheck is a Python CLI tool and agent skill for verifying academic paper citations. This repository contains both the installable Python package (`pip install CiteCheck`) and the agent skill definitions.

## When This Context Applies

Load this context when working on:
- The `citecheck` Python package (`src/citecheck/`)
- The agent skill definitions (`skills/`, `references/`)
- CLI behavior, parsing logic, or report generation
- Bug fixes or feature additions to the citation verification pipeline

## Project Structure

```
CiteCheck/
├── src/citecheck/          # Python package source
│   ├── cli.py              # CLI entry point
│   ├── parser.py           # LaTeX / PDF dispatcher
│   ├── bibtex_parser.py    # BibTeX .bib parser
│   ├── pdf_parser.py       # PDF text extraction
│   ├── verifier.py         # Crossref / Semantic Scholar verification
│   ├── matcher.py          # Thematic & semantic scoring (heuristic + LLM)
│   ├── reporter.py         # Markdown report generator
│   └── models.py           # Shared dataclasses
├── skills/citecheck/       # Agent skill (cross-platform)
│   └── SKILL.md            # Skill entry point
├
```

</details>
