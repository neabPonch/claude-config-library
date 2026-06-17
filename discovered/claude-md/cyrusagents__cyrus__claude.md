---
name: cyrusagents__cyrus__claude
source: https://github.com/cyrusagents/cyrus/blob/2b77ac1a4c9fce46b83054a95fb027d16df8e6f9/apps/f1/CLAUDE.md
repo: cyrusagents/cyrus
kind: claude-md
stars: 638
last_pushed: 2026-06-12T18:06:31Z
license: apache-2.0
score: 9
domains: [cli-tools, agents-ai, testing-framework]
tags: [workflow-orchestration, architecture-first, scenario-driven]
curated: 2026-06-15
curated_by: config-scout
---

# cyrusagents/cyrus — claude-md

**Why it's worth keeping:** Uses 'Scenario-Based Instruction' by providing complete lifecycles (scaffold -> server -> issue -> session); includes detailed architecture diagrams to explain service communication flows.

**Summary:** Provides deep architectural context and end-to-end workflow orchestration for a CLI-based testing framework.

**Source credibility:** High: 638 stars, very recent activity, and specialized agentic infrastructure.

**Recency:** Very current; utilizes modern toolchains like Bun and Vitest.

**Source:** [cyrusagents/cyrus/apps/f1/CLAUDE.md](https://github.com/cyrusagents/cyrus/blob/2b77ac1a4c9fce46b83054a95fb027d16df8e6f9/apps/f1/CLAUDE.md) · 638★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# F1 Testing Framework - Developer Documentation

This documentation provides guidance to Claude Code when working with the F1 testing framework.

## Project Overview

The F1 Testing Framework is an end-to-end observable testing platform for the Cyrus agent system. It provides a CLI-based issue tracker that simulates Linear's functionality without requiring external dependencies.

**Key Features:**
- In-memory issue tracking (CLIIssueTrackerService)
- CLI platform mode for EdgeWorker
- Beautiful CLI interface with ANSI colors
- RPC server for CLI-to-EdgeWorker communication
- Zero external dependencies for testing
- Zero `any` types throughout the codebase

## Architecture

The F1 framework follows this flow:

```
CLI Commands (f1 binary)
         ↓
   JSON-RPC over HTTP
         ↓
   CLIRPCServer (Fastify)
         ↓
   CLIIssueTrackerService (in-memory)
         ↓
   EdgeWorker (platform: "cli")
         ↓
   Claude Code Sessions
```

For detailed architecture information, see `/spec/f1/ARCHITECTURE.md`.

## File Structure

```
apps/f1/
├── f1                    # CLI binary (bash script calling bun)
├── server.ts             # Server startup script
├── src/
│   ├── cli.ts
```

</details>
