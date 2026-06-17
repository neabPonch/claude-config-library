---
name: microsoft__vscode__skill
source: https://github.com/microsoft/vscode/blob/5ad37552bf432021eb7caee1a366b710c0e49e42/.agents/skills/launch/SKILL.md
repo: microsoft/vscode
kind: skill
stars: 186316
last_pushed: 2026-06-15T08:00:34Z
license: mit
score: 9
domains: [cli-tools, dev-ops, automation]
tags: [vscode, debugging, playwright, cdp, environment-setup]
curated: 2026-06-15
curated_by: config-scout
---

# microsoft/vscode — skill

**Why it's worth keeping:** Demonstrates a sophisticated 'slim-clone' pattern that preserves authentication state while discarding heavy caches. It also provides an excellent example of returning environment metadata as structured JSON for programmatic agent consumption.

**Summary:** Creates an isolated, authenticated development environment for VS Code designed specifically for automated UI testing and debugging via Playwright and DAP. It manages port collisions and profiles to allow multiple concurrent instrumented sessions.

**Source credibility:** Extremely high; sourced from the official Microsoft VS Code repository.

**Recency:** Highly current, reflecting modern development and automation workflows.

**Source:** [microsoft/vscode/.agents/skills/launch/SKILL.md](https://github.com/microsoft/vscode/blob/5ad37552bf432021eb7caee1a366b710c0e49e42/.agents/skills/launch/SKILL.md) · 186316★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: launch
description: "Launch Code OSS (VS Code from sources) into an isolated throwaway profile with unique debug ports so you can drive it with @playwright/cli AND attach a Node debugger via dap-cli in the same session. Use when working on VS Code itself and you want to interact with the running workbench, automate chat or UI flows, test UI features, take screenshots, set breakpoints in the renderer / extension host / main process, or combine UI driving with debugging."
---

# Code OSS Dev - Launch + Debug

You're working on VS Code itself and you want to:

1. Launch a Code OSS build from sources that is **already signed in** (Copilot, GitHub, etc.) so chat / agent flows work end-to-end.
2. Drive it with `@playwright/cli` over CDP (UI automation).
3. Optionally attach a debugger via **dap-cli** to set breakpoints in the renderer, extension host, or main process.
4. Run multiple instances at once without port conflicts.

This skill provides a launcher that clones an authenticated user-data-dir to a throwaway temp folder, picks free ports for every debug surface, and prints them as JSON so you can pick them up programmatically.

The clone is **slim**: workspace storage, bro
```

</details>
