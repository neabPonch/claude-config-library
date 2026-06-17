---
name: OneKeyHQ__app-monorepo__skill
source: https://github.com/OneKeyHQ/app-monorepo/blob/5df1bac7016807fa04fcbb96f7601cfb501d29f4/.skillshare/skills/1k-dev-commands/SKILL.md
repo: OneKeyHQ/app-monorepo
kind: skill
stars: 2376
last_pushed: 2026-06-16T06:26:58Z
license: other
score: 9
domains: [frontend, mobile, monorepo]
tags: [development, troubleshooting, monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# OneKeyHQ/app-monorepo — skill

**Why it's worth keeping:** The inclusion of 'Runtime' helps the agent manage time expectations, while 'Common issues' provides actionable troubleshooting steps to enable autonomous error recovery without human intervention.

**Summary:** Provides comprehensive command mapping for a multi-platform monorepo including runtime estimates and error recovery paths.

**Source credibility:** High; based on a popular (2k+ stars) and actively maintained open-source project.

**Recency:** Very current; utilizes modern tooling patterns like Rspack and Manifest v3.

**Source:** [OneKeyHQ/app-monorepo/.skillshare/skills/1k-dev-commands/SKILL.md](https://github.com/OneKeyHQ/app-monorepo/blob/5df1bac7016807fa04fcbb96f7601cfb501d29f4/.skillshare/skills/1k-dev-commands/SKILL.md) · 2376★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: 1k-dev-commands
description: Development commands — yarn scripts for dev servers, building, linting, testing, and troubleshooting.
allowed-tools: Bash, Read
---

# OneKey Development Commands

## Application Development Commands

**PLATFORM-SPECIFIC DEVELOPMENT**:
- `yarn app:desktop:rspack` - Start desktop Electron app development
  - **Runtime**: 30-60 seconds to start
  - **Common issues**: Node version conflicts, missing native dependencies
  - **Troubleshooting**: Run `yarn clean && yarn reinstall` if startup fails

- `yarn app:web:rspack` - Start web development server (port 3000)
  - **Runtime**: 15-30 seconds to start
  - **Common issues**: Port 3000 already in use, rspack compilation errors
  - **Troubleshooting**: Kill existing processes on port 3000, check console for specific errors

- `yarn app:ext:rspack` - Start browser extension development
  - **Runtime**: 20-40 seconds to start
  - **Common issues**: Manifest v3 validation errors, permission issues
  - **Troubleshooting**: Check extension manifest validity, verify content security policy

- `yarn app:ios` - Start iOS mobile development
  - **Runtime**: 1-2 minutes (includes Metro bundler)
  - **Common is
```

</details>
