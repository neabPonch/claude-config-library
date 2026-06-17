---
name: WebMCP-org__npm-packages__webmcp-userscript-skill
source: https://github.com/WebMCP-org/npm-packages/blob/868ffe0e147ac7b2707691ff8e8100f6dd425354/docs/plans/WEBMCP_USERSCRIPT_SKILL.md
repo: WebMCP-org/npm-packages
kind: skill
stars: 60
last_pushed: 2026-06-14T10:14:18Z
license: mit
score: 9
domains: [agents-ai, browser-automation, web-development, mcp]
tags: [webmcp, chrome-devtools, esbuild, self-testing]
curated: 2026-06-15
curated_by: config-scout
---

# WebMCP-org/npm-packages — skill

**Why it's worth keeping:** The two-tier build system (source files vs. in-memory esbuild injection) is a brilliant pattern for reducing agent friction during iterative development. The concept of an 'Injection Loop' allows the agent to self-verify tools without manual build steps.

**Summary:** Enables agents to create, bundle, and inject MCP tools directly into browser environments via Chrome DevTools. It automates the developer loop from TypeScript source to live-running tool.

**Source credibility:** High; coming from a specialized WebMCP repo with active maintenance and clear architectural focus.

**Recency:** Extremely current, referencing modern toolsets like tsdown and future Chrome versions.

**Source:** [WebMCP-org/npm-packages/docs/plans/WEBMCP_USERSCRIPT_SKILL.md](https://github.com/WebMCP-org/npm-packages/blob/868ffe0e147ac7b2707691ff8e8100f6dd425354/docs/plans/WEBMCP_USERSCRIPT_SKILL.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# WebMCP Development Skill

> **Status:** Implemented
> **Implemented in:** `skills/webmcp/` (SKILL.md + reference docs)
> **Chrome API:** WebMCP available behind flag in Chrome 146+. Skill works with both native and polyfill runtimes.

## Executive Summary

This document outlines the implementation of a **unified Claude Code skill** for WebMCP tool development. The skill teaches agents to create, test, and iterate on MCP tools for any website or web app - using chrome-devtools-mcp for the entire development loop.

### The Power Couple

```
┌─────────────────────────────────────────────────────────────────────┐
│                     UNIFIED SKILL (webmcp)                          │
│           Progressive disclosure - sections loaded as needed        │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  SKILL.md (~300 lines)     references/ (loaded on-demand)          │
│  ├── Quick Start           ├── REACT_INTEGRATION.md                │
│  ├── Injection Loop        ├── USERSCRIPT_GUIDE.md                 │
│  ├── Tool Design           ├── PRODUCTION_TESTING.md               │
│  └── Se
```

</details>
