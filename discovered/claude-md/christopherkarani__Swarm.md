---
name: christopherkarani__Swarm
source: https://github.com/christopherkarani/Swarm/blob/c771f189a17d4842f68bfb25a69d208a3372ad7c/CLAUDE.md
repo: christopherkarani/Swarm
kind: claude-md
stars: 492
last_pushed: 2026-06-13T10:10:52Z
license: mit
score: 9
domains: [agents-ai, swift-development, systems-programming]
tags: [swift, concurrency, agent-framework, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# christopherkarani/Swarm — claude-md

**Why it's worth keeping:** It defines strict technical constraints (Swift 6 concurrency/Sendable rules) and provides actionable CLI workflows including environment variable requirements.

**Summary:** Provides high-level architectural context, a detailed repository tree map, and specific build/test commands for the Swarm framework.

**Source credibility:** High-quality open-source project with significant stars and very recent maintenance.

**Recency:** Highly current, specifically targeting Swift 6 and modern agentic frameworks.

**Source:** [christopherkarani/Swarm/CLAUDE.md](https://github.com/christopherkarani/Swarm/blob/c771f189a17d4842f68bfb25a69d208a3372ad7c/CLAUDE.md) · 492★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

Guidance for AI coding assistants (Claude Code, Cursor, etc.) working in this
repository. This file is the canonical, in-repo briefing — read it before making
changes.

## What is Swarm?

Swarm is a Swift 6.2 framework for building **agents and multi-agent
workflows** on Apple platforms (iOS 26+, macOS 26+, tvOS 26+) and Linux. It is
built around:

- **Agents** — `Agent` struct with `@ToolBuilder` trailing closures, an
  `AgentRuntime` protocol, and pluggable inference providers.
- **Workflows** — fluent composition (`.step`, `.parallel`, `.route`,
  `.repeatUntil`) compiled to a DAG with checkpoint/resume.
- **Tools** — the `@Tool` macro generates JSON schemas from Swift structs at
  compile time; `FunctionTool` covers ad-hoc closures.
- **Memory** — conversation, sliding-window, summary, vector, and
  persistent backends.
- **Guardrails / Resilience / Observability** — first-class concerns, not
  bolt-ons.
- **Providers** — Foundation Models, Anthropic, OpenAI, Ollama, Gemini,
  MiniMax, OpenRouter, MLX, all routed through [Conduit](https://github.com/christopherkarani/Conduit).
- **MCP** — Model Context Protocol client and server support.

The package uses Swift 6.2
```

</details>
