---
name: llm4s__llm4s
source: https://github.com/llm4s/llm4s/blob/ce8ba32c7724e9454987d7da9548c0194cb5f28f/CLAUDE.md
repo: llm4s/llm4s
kind: claude-md
stars: 247
last_pushed: 2026-06-14T17:33:43Z
license: mit
score: 9
domains: [agents-ai, backend-scala, llm-orchestration]
tags: [scala, agent-framework, functional-programming, type-safe]
curated: 2026-06-15
curated_by: config-scout
---

# llm4s/llm4s — claude-md

**Why it's worth keeping:** The 'Good vs Bad' code examples provide unmistakable guidance on architectural patterns, while the explicit list of banned patterns prevents common anti-patterns in a functional Scala environment.

**Summary:** A highly structured guide for a Scala LLM framework that emphasizes type-safety and functional error handling. It provides deep context on the library's specific agentic features like guardrails and handoffs.

**Source credibility:** A well-maintained, specialized project focused on LLM orchestration in Scala.

**Recency:** Highly current; reflects modern agentic/LLM programming paradigms and tool usage.

**Source:** [llm4s/llm4s/CLAUDE.md](https://github.com/llm4s/llm4s/blob/ce8ba32c7724e9454987d7da9548c0194cb5f28f/CLAUDE.md) · 247★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for LLM4S

## Project Overview

**LLM4S** (Large Language Models for Scala) is a framework for building LLM-powered applications in Scala with:
- Multi-provider support (OpenAI, Anthropic, Azure, Ollama, Google Gemini)
- Type-safe design with `Result[A]` error handling
- Agent framework with tools, guardrails, handoffs, and memory
- Cross-compilation for Scala 2.13 and 3.x

**Tech Stack:** Scala 2.13/3.x, SBT, ScalaTest, Cats, uPickle, Docker

## Core Principles

1. **Use `Result[A]` instead of exceptions** - `type Result[+A] = Either[LLMError, A]`
2. **Use `Llm4sConfig` at the app edge** - Never use `sys.env`, `System.getenv`, or `ConfigSource.default` directly in core code
3. **Use type-safe newtypes** - `ModelName`, `ApiKey`, `ConversationId` etc.
4. **Cross-version compatibility** - Test with `sbt +test`

## Repository Structure

```
llm4s/
├── modules/
│   ├── core/            # Core library (published)
│   ├── samples/         # Usage examples
│   ├── workspace/       # Containerized execution
│   └── crossTest/       # Cross-version tests
├── docs/                # Documentation
├── project/             # SBT config
└── build.sbt
```

**Key p
```

</details>
