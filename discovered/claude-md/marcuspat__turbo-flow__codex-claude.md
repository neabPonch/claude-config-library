---
name: marcuspat__turbo-flow__codex-claude
source: https://github.com/marcuspat/turbo-flow/blob/96d8f47ede9e6f9bca4b7e128edac0d86a54d69f/devpods/context/codex_claude.md
repo: marcuspat/turbo-flow
kind: claude-md
stars: 162
last_pushed: 2026-06-13T16:04:32Z
license: mit
score: 8
domains: [cli-tools, devops, agents-ai]
tags: [setup-automation, idempotency, os-detection, workflow]
curated: 2026-06-16
curated_by: config-scout
---

# marcuspat/turbo-flow — claude-md

**Why it's worth keeping:** It uses a state-machine pattern with explicit OS detection, idempotency checks (skipping existing steps), and error-handling branches that are highly transferable for agentic automation.

**Summary:** A rigorous, logic-driven installation protocol designed to guide Claude through complex environment bootstrapping.

**Source credibility:** The repo has healthy engagement (162 stars) and active maintenance.

**Recency:** Extremely current, based on the '0 months ago' push date.

**Source:** [marcuspat/turbo-flow/devpods/context/codex_claude.md](https://github.com/marcuspat/turbo-flow/blob/96d8f47ede9e6f9bca4b7e128edac0d86a54d69f/devpods/context/codex_claude.md) · 162★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Codex Setup Instructions for Claude Code

**Purpose:** User gives this document to Claude Code with the instruction "Please set up Codex on my system" and Claude executes all steps automatically.

**Prerequisites:**
- Node.js and npm installed
- Basic development environment
- Git installed (for project version control)

---

## ⚡ Claude Execution Flowchart (READ THIS FIRST)

**Claude, follow this exact flowchart to execute the setup correctly:**

### Step 1: Detect the Operating System (DO THIS FIRST)

Execute this command to detect the OS:

```bash
uname -s
```

**Based on the output, remember the OS:**
- If output is `Darwin` → You are on **macOS** (use Part 1c, 5c, 6c)
- If output is `Linux` → You are on **Linux** (use Part 1b, 5b, 6b)
- If output is not recognized, try this Windows command:

```powershell
$PSVersionTable.Platform
```

- If output is `Win32NT` → You are on **Windows** (use Part 1a, 5a, 6a)

**Write down your OS now, you'll need it for the remaining steps.**

### Step 2: Execute the Setup in Order

For each part below, **execute ONLY the section labeled with your detected OS**. Skip all other OS sections.

**Part 0a:** Prerequisites Check (all OS sections - ex
```

</details>
