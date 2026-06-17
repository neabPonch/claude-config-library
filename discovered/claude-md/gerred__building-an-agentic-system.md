---
name: gerred__building-an-agentic-system
source: https://github.com/gerred/building-an-agentic-system/blob/eec7f0226fb0d0019c67dc6f209a80b61720117e/CLAUDE.md
repo: gerred/building-an-agentic-system
kind: claude-md
stars: 318
last_pushed: 2025-06-05T22:05:10Z
license: unknown
score: 9
domains: [documentation, technical-writing, agents-ai]
tags: [style-guide, negative-constraints, voice-control]
curated: 2026-06-15
curated_by: config-scout
---

# gerred/building-an-agentic-system — claude-md

**Why it's worth keeping:** The 'Hard Rules' section uses sophisticated negative constraints to strip away LLM-isms like hedging, speculation, and prescriptive language. The concept of 'IRC-inspired pragmatism' is a brilliant way to define tone through persona rather than just adjectives.

**Summary:** Provides comprehensive project context for an mdBook documentation series, including commands and structure. It excels at defining a highly specific technical voice.

**Source credibility:** High; the repo focuses on agentic systems, so the instructions reflect expert meta-prompting knowledge.

**Recency:** 

**Source:** [gerred/building-an-agentic-system/CLAUDE.md](https://github.com/gerred/building-an-agentic-system/blob/eec7f0226fb0d0019c67dc6f209a80b61720117e/CLAUDE.md) · 318★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is an mdBook documentation project - "The Agentic Systems Series" - a comprehensive two-book guide about building AI coding assistants. It analyzes architecture patterns from Claude Code, anon-kode, and Amp to provide practical insights for engineers building production AI development tools.

The series covers everything from single-user local tools (Book 1) to collaborative enterprise platforms (Book 2).

## Common Commands

```bash
# Local development
mdbook serve        # Start local server at http://localhost:3000
mdbook build        # Build static site to book/ directory
mdbook clean        # Clean build artifacts

# Testing
mdbook test         # Test code examples in documentation
```

## Project Structure

The documentation follows mdBook conventions:
- `src/` - All markdown content files
- `src/SUMMARY.md` - Navigation structure and chapter ordering
- `book.toml` - mdBook configuration
- `amp/` - Contains analyzed source code from amp/Claude Code
- `src/second-edition/` - Book 2: Amping Up an Agentic System

Key content areas:
- **Bo
```

</details>
