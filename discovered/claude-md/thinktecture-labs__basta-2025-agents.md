---
name: thinktecture-labs__basta-2025-agents
source: https://github.com/thinktecture-labs/basta-2025-agents/blob/543e8f2952d661f6a94710dcccf92e97c9efe157/CLAUDE.md
repo: thinktecture-labs/basta-2025-agents
kind: claude-md
stars: 3
last_pushed: 2025-09-23T08:59:40Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, .net]
tags: [architectural-spec, csharp, agentic-workflows]
curated: 2026-06-17
curated_by: config-scout
---

# thinktecture-labs/basta-2025-agents — claude-md

**Why it's worth keeping:** The 'Next up' section provides exceptionally granular technical constraints—such as tool reflection, model tiering (reasoning vs. fast), and memory compaction requirements—that eliminate ambiguity for an AI developer.

**Summary:** A dual-purpose file that serves as both project documentation and a highly detailed architectural blueprint for building a .NET 9-based AI agent.

**Source credibility:** High-quality expert specification intended for a 2025 technical conference presentation.

**Recency:** Very current; includes modern concepts like .NET 9, prompt caching, and multi-model orchestration.

**Source:** [thinktecture-labs/basta-2025-agents/CLAUDE.md](https://github.com/thinktecture-labs/basta-2025-agents/blob/543e8f2952d661f6a94710dcccf92e97c9efe157/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is a demo repository for a BASTA 2025 conference talk about building AI agents. It demonstrates core concepts of LLM interactions through HTTP request examples.

## Project Structure

The repository contains educational HTTP request files demonstrating:
- `requests/01 plain llm.http` - Basic LLM API calls showing stateless nature
- `requests/02 memory.http` - Managing conversation context through message history
- `requests/03 functions.http` - Tool/function calling capabilities with LLMs

## Environment Setup

1. Copy `.env.template` to `.env`
2. Configure your LLM provider:
   - **Ollama (default)**: Pre-configured for local models
   - **OpenAI**: Uncomment and add API key
   - **OpenRouter**: Uncomment and add API key

## Required Models for Ollama

```bash
ollama pull mistral-small3.2:24b
ollama pull mistral-large:latest
ollama pull gpt-oss:20b
```

## Key Concepts Demonstrated

The HTTP files showcase progressive complexity in LLM interactions:
1. **Stateless nature** - LLMs don't remember previous interactions without explicit cont
```

</details>
