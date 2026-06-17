---
name: michiel__torque
source: https://github.com/michiel/torque/blob/5c19068657e1015e766063535c3b55d9a7b37de2/CLAUDE.md
repo: michiel/torque
kind: claude-md
stars: 0
last_pushed: 2026-02-03T19:34:42Z
license: unknown
score: 8
domains: [backend-api, web-frontend, systems-programming]
tags: [rust, react, performance-optimization, model-driven]
curated: 2026-06-17
curated_by: config-scout
---

# michiel/torque — claude-md

**Why it's worth keeping:** Includes concrete numerical performance targets (SLAs) and unique architecture patterns that prevent the AI from suggesting generic implementations. It also provides specific tool usage instructions like using 'playwright' for frontend verification and 'notify-send' for task completion.

**Summary:** Provides deep architectural context for a performance-critical Rust/React platform emphasizing model-driven design.

**Source credibility:** Low social proof/stars, but the technical depth suggests a highly structured engineering project.

**Recency:** Current; explicitly references Claude Code and modern integration patterns like playwright-mcp.

**Source:** [michiel/torque/CLAUDE.md](https://github.com/michiel/torque/blob/5c19068657e1015e766063535c3b55d9a7b37de2/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Torque is a high-performance platform for designing, running and presenting applications, targeting Web frontends for humans and MCP APIs for AI agents. The platform emphasizes **speed as the top priority** and uses a model-driven architecture where applications are dynamically generated from visual models.

 - DESIGN.md and IMPLEMENTATION.md contain the project description 
 - DESIGN-MODEL-EDITOR.md contains the description and specifications for the model-editor frontend ui
 - TODO.md contains the implementation plan. Keep this file updated as changes are made
 - Reviews go to docs/reviews, are written in markdown, and are prefixed with the current date (example prefix : '2025-07-02-')
 - Plans go to docs/reviews, are written in markdown, and are prefixed with the current date (example prefix : '2025-07-02-')

## Tooling

 - Use any relevant cargo tooling, request its installation if it is not available
 - Remember to use playwright-mcp for frontend verification and troubleshooting
 - Request any relevant tooling
 - Whenever you stop to ask a q
```

</details>
