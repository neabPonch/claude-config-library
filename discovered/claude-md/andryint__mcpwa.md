---
name: andryint__mcpwa
source: https://github.com/andryint/mcpwa/blob/b8651f737e5a62b467ea7d02b68074bb175d7984/Claude.md
repo: andryint/mcpwa
kind: claude-md
stars: 1
last_pushed: 2026-02-21T18:59:13Z
license: unknown
score: 9
domains: [macos, api-integration, automation, mcp]
tags: [cocoa, whatsapp-automation, sse, backend-api]
curated: 2026-06-16
curated_by: config-scout
---

# andryint/mcpwa — claude-md

**Why it's worth keeping:** Contains explicit API request/response schemas and SSE streaming event formats which are vital for preventing AI hallucination during development. It also maps file structure directly to functional responsibilities.

**Summary:** Provides a deep architectural overview of a macOS Cocoa application that integrates with WhatsApp via an MCP backend.

**Source credibility:** Low star count (1), but the technical depth suggests a highly specific, real-world tool.

**Recency:** Current; reflects modern MCP/LLM integration workflows from 4 months ago.

**Source:** [andryint/mcpwa/Claude.md](https://github.com/andryint/mcpwa/blob/b8651f737e5a62b467ea7d02b68074bb175d7984/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MCPWA - WhatsApp Assistant

## Project Overview

MCPWA is a macOS Cocoa application that serves as a WhatsApp Assistant. The app connects to a backend service that provides LLM-powered chat capabilities and can interact with WhatsApp via the Accessibility API through the MCP protocol.

The architecture is:
- **Frontend (this app)**: macOS native UI for chat interaction
- **Backend service**: Handles LLM queries, RAG, and MCP tool execution
- **WhatsApp integration**: Via Accessibility API, accessible through the backend's MCP tools

## Project Structure

```
mcpwa/
├── mcpwa/                    # Main Cocoa App
│   ├── AppDelegate.m/h       # App entry point
│   ├── BotChatWindowController.m/h  # Main chat UI & message handling
│   ├── RAGClient.m/h         # Backend API client
│   ├── SettingsWindowController.m/h # User preferences (theme, backend URL)
│   ├── DebugConfigWindowController.m/h # Debug configuration
│   ├── WAAccessibility.m/h   # WhatsApp UI automation via Accessibility API
│   ├── WAAccessibilityExplorer.m/h # Accessibility tree explorer
│   ├── WALogger.m/h          # Logging utility
│   └── Assets/               # App icons, images
└── mcp-shim/
```

</details>
