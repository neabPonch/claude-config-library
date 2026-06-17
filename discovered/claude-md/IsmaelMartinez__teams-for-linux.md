---
name: IsmaelMartinez__teams-for-linux
source: https://github.com/IsmaelMartinez/teams-for-linux/blob/402800af5013bf3239642c0702bf7c065b04c4b7/CLAUDE.md
repo: IsmaelMartinez/teams-for-linux
kind: claude-md
stars: 4779
last_pushed: 2026-06-15T19:44:18Z
license: gpl-3.0
score: 9
domains: [desktop-app, electron-js, security-compliance]
tags: [security-first, architecture-heavy, documentation-driven]
curated: 2026-06-16
curated_by: config-scout
---

# IsmaelMartinez/teams-for-linux — claude-md

**Why it's worth keeping:** The PII protection examples provide critical security guardrails; the directive to prioritize local markdown over web searches prevents hallucination.

**Summary:** Provides deep technical context, strict coding standards for IPC/security, and a roadmap for navigating local documentation.

**Source credibility:** Highly credible: 4.7k stars and very recent maintenance activity.

**Recency:** Current: uses modern tech stack (Playwright, Docusaurus) and optimized agent-specific workflows.

**Source:** [IsmaelMartinez/teams-for-linux/CLAUDE.md](https://github.com/IsmaelMartinez/teams-for-linux/blob/402800af5013bf3239642c0702bf7c065b04c4b7/CLAUDE.md) · 4779★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> [!NOTE]
> **For comprehensive documentation**, see the markdown files in `docs-site/docs/` directory. These files are the source for the [Teams for Linux Documentation Site](https://ismaelmartinez.github.io/teams-for-linux/). This file contains essential quick reference information and critical warnings specific to Claude Code workflows.
>
> **Important for AI agents**: Always read documentation from the local markdown files in `docs-site/docs/` rather than fetching from the web. The URLs are provided for human reference only.

## Essential Commands

**Development:**
- `npm start` - Run application in development mode with trace warnings
- `npm run lint` - Run ESLint validation (mandatory before commits)
- `npm run test:e2e` - Run end-to-end tests with Playwright

**Building:**
- `npm run pack` - Development build without packaging
- `npm run dist:linux` - Build Linux packages (AppImage, deb, rpm, snap)
- `npm run dist` - Build all platforms using electron-builder

**Utility:**
- `npm run generate-release-info` - Generate release information file
- `npm run generat
```

</details>
