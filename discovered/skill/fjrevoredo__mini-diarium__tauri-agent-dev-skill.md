---
name: fjrevoredo__mini-diarium__tauri-agent-dev-skill
source: https://github.com/fjrevoredo/mini-diarium/blob/3542c365ccc8b96734ce57cdb6559db5aac30702/docs/archive/tauri-agent-dev-skill.md
repo: fjrevoredo/mini-diarium
kind: skill
stars: 274
last_pushed: 2026-06-14T09:18:38Z
license: mit
score: 9
domains: [tauri, ui-automation, dev-tools, desktop-apps]
tags: [tauri, cdp, sandboxing, automated-testing]
curated: 2026-06-15
curated_by: config-scout
---

# fjrevoredo/mini-diarium — skill

**Why it's worth keeping:** Demonstrates advanced state isolation by overriding WebView/backend data paths to prevent test leakage and includes robust process tracking/health probing for reliable automation.

**Summary:** Enables an agent to launch, programmatically drive (via CDP), and clean up a sandboxed Tauri application for end-to-end UI verification.

**Source credibility:** High; reflects deep technical integration within an active open-source project.

**Recency:** Extremely recent (dated May 2026 in metadata).

**Source:** [fjrevoredo/mini-diarium/docs/archive/tauri-agent-dev-skill.md](https://github.com/fjrevoredo/mini-diarium/blob/3542c365ccc8b96734ce57cdb6559db5aac30702/docs/archive/tauri-agent-dev-skill.md) · 274★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# tauri-agent-dev Skill

## Metadata

- Plan Status: COMPLETED
- Created: 2026-05-22
- Last Updated: 2026-05-22 (sandbox journal config + WebView storage isolation added; full smoke test completed)
- Owner: Coding agent
- Approval: APPROVED

## Implementation Status

- **2026-05-22**: Self-check completed. Plan revised to drop Milestone 3 (Playwright fallback) after confirming `agent-browser connect <port|url>` is available. Script runner convention pinned to `npx tsx`. The initial assumption that `MINI_DIARIUM_DATA_DIR` alone would avoid sandbox config seeding was later disproven during smoke testing and corrected in the final implementation.
- **2026-05-22**: Attempted Milestone 1 CDP smoke probe. Blocked: port 1420 (Vite dev server) was already held by an active `tauri dev` session belonging to the user (node PID 19076). User chose to pause all implementation work rather than have the agent kill their running session. No files written; one scratch log file (`.agent-dev-probe.log`) created at repo root from the failed probe attempt and pending cleanup.
- **2026-05-22**: User asked to continue. Pre-resume check found no listeners on ports 1420/1421/9222/9223, so the original Miles
```

</details>
