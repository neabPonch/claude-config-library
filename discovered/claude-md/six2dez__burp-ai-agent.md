---
name: six2dez__burp-ai-agent
source: https://github.com/six2dez/burp-ai-agent/blob/8b92fc716bd530d45a2d86d28dec6d88203d98fd/CLAUDE.md
repo: six2dez/burp-ai-agent
kind: claude-md
stars: 1239
last_pushed: 2026-06-10T18:54:20Z
license: mit
score: 7
domains: [security, cli-tools, java-kotlin]
tags: [constraints, workflow-enforcement, agentic-patterns]
curated: 2026-06-14
curated_by: config-scout
---

# six2dez/burp-ai-agent — claude-md

**Why it's worth keeping:** The 'Constraints' section uses non-negotiable guardrails for environment/privacy, while the 'GSD Workflow' implements procedural entry points to prevent unguided AI edits.

**Summary:** Defines rigid technical constraints and a command-driven workflow to enforce structured planning before file modification.

**Source credibility:** High-authority source: 1.2k stars on a specialized security tool.

**Recency:** Highly current; active development within the last month.

**Source:** [six2dez/burp-ai-agent/CLAUDE.md](https://github.com/six2dez/burp-ai-agent/blob/8b92fc716bd530d45a2d86d28dec6d88203d98fd/CLAUDE.md) · 1239★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- GSD:project-start source:PROJECT.md -->
## Project

**Burp AI Agent**

A production-grade Burp Suite extension (Kotlin + Montoya API) that embeds an AI reasoning agent with pluggable backends (local + cloud), enforces privacy redaction on outbound traffic, records an auditable history, and exposes Burp operations to external AI agents over the Model Context Protocol (MCP). Targets security professionals running Burp Community or Professional on macOS / Linux / Windows.

**Core Value:** Bring modern AI to a real security workflow **without** leaking sensitive traffic to third-party providers — privacy controls and an audit trail are non-negotiable, AI capability is additive.

### Constraints

- **Tech stack**: Kotlin (JVM 21), Gradle Kotlin DSL, Burp Montoya API — fixed by ADR-1/2/3.
- **Target**: Burp Suite Community + Professional 2023.12+, cross-platform (macOS / Linux / Windows).
- **Network**: MCP server binds to `127.0.0.1` by default; external access requires explicit opt-in + bearer token + optional TLS.
- **Distribution**: single fat JAR via `./gradlew shadowJar`; artifact name `Custom-AI-Agent-<version>.jar` (renamed from `Burp-AI-Agent-*` in `v0.6.0`).
- **Privacy**:
```

</details>
