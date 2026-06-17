---
name: MadnessEngineering__Omnispindle
source: https://github.com/MadnessEngineering/Omnispindle/blob/31450b925b183595419a71b94c40109f29bf9add/CLAUDE.md
repo: MadnessEngineering/Omnispindle
kind: claude-md
stars: 10
last_pushed: 2026-06-10T15:46:06Z
license: unknown
score: 9
domains: [agents-ai, mcp-server, backend-api, cli-tools]
tags: [mcp, python, deployment, technical-manual]
curated: 2026-06-15
curated_by: config-scout
---

# MadnessEngineering/Omnispindle — claude-md

**Why it's worth keeping:** It includes 'gotcha' warnings for specific MCP failures (like payload structures) and explains nuanced tool behaviors like mandatory metadata or context-passing requirements. The clear distinction between operation modes allows the agent to adapt its execution strategy based on the environment.

**Summary:** This file serves as a highly detailed operational manual that outlines deployment phases, runtime modes, and specific tool interaction requirements. It provides the agent with technical constraints to prevent API errors and ensures correct data routing.

**Source credibility:** The repository shows active, structured development with high-detail maintenance logs and a moderate star count.

**Recency:** Extremely current, explicitly referencing Python 3.13 and modern MCP protocols.

**Source:** [MadnessEngineering/Omnispindle/CLAUDE.md](https://github.com/MadnessEngineering/Omnispindle/blob/31450b925b183595419a71b94c40109f29bf9add/CLAUDE.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Development Commands

### 🚀 v1.0.0 Deployment Status (IMPORTANT!)

**Current Release**: v1.0.0 production-ready with comprehensive deployment modernization completed through Phase 6

**Completed Phases**:
- ✅ **Phase 1**: PM2 ecosystem modernized (Python 3.13, GitHub Actions, modern env vars)
- ✅ **Phase 2**: Docker infrastructure updated (Python 3.13, API-first, health checks)
- ✅ **Phase 3**: PyPI package preparation complete (build scripts, MANIFEST.in, entry points)
- ✅ **Phase 4**: Security review complete (git-secrets, credential audit, hardcoded IP cleanup)
- ✅ **Phase 6**: Documentation review (README.md updated, this CLAUDE.md refresh)

**Key Changes Made**:
- Modernized to Python 3.13 across all deployment configs
- Removed MongoDB dependencies from Docker (API-first architecture)
- Added comprehensive PyPI packaging with CLI entry points
- Implemented git-secrets protection with AWS patterns
- Enhanced .gitignore with comprehensive security patterns
- Updated all hardcoded IPs to use environment variables

**CLI Commands Available** (after `pip install
```

</details>
