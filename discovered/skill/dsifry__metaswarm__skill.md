---
name: dsifry__metaswarm__skill
source: https://github.com/dsifry/metaswarm/blob/398be78231bc1c57b147869c5c80696003e95f31/skills/setup/SKILL.md
repo: dsifry/metaswarm
kind: skill
stars: 311
last_pushed: 2026-05-16T04:02:13Z
license: mit
score: 9
domains: [devops, developer-experience, cli-tools]
tags: [setup, profiling, quality-gates, onboarding]
curated: 2026-06-15
curated_by: config-scout
---

# dsifry/metaswarm — skill

**Why it's worth keeping:** The 'Silent Detection' pattern (detecting language/frameworks via files before asking the user) is a world-class technique for reducing agent friction. The logic for mapping detected tools to specific enforcement commands (e.g., Vitest vs Pytest) creates highly transferable infrastructure templates.

**Summary:** An automated project profiling and bootstrapping skill that detects a stack's architecture and configures quality gates like test coverage enforcement.

**Source credibility:** High; the repository has significant stars and shows active, recent maintenance reflecting modern CLI workflows.

**Recency:** Very current; it is specifically designed for the latest generation of agent CLIs like Claude Code and Gemini.

**Source:** [dsifry/metaswarm/skills/setup/SKILL.md](https://github.com/dsifry/metaswarm/blob/398be78231bc1c57b147869c5c80696003e95f31/skills/setup/SKILL.md) · 311★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: setup
description: Interactive project setup — detects your project, configures metaswarm, writes project-local files
---

# Setup

Interactive setup for metaswarm. Detects your stack, asks targeted questions, writes project-local files, and creates platform-appropriate instruction files and command shims. Replaces both `npx metaswarm init` and the old `/metaswarm-setup` command.

<CRITICAL-REQUIREMENTS>
Setup MUST produce the mandatory outputs for the active platform. A shell script handles them automatically — you MUST run it.

After Phase 2 (user questions), determine the correct coverage command from the detection results, then run this Bash command:

```bash
PLUGIN_ROOT="${PLUGIN_ROOT:-${CLAUDE_PLUGIN_ROOT:-${extensionPath:-}}}"
if [ -z "$PLUGIN_ROOT" ]; then
  setup_script="$(find "${CODEX_HOME:-$HOME/.codex}/plugins/cache" -path '*/metaswarm/*/lib/setup-mandatory-files.sh' -print -quit 2>/dev/null)"
  if [ -n "$setup_script" ]; then
    PLUGIN_ROOT="$(cd "$(dirname "$setup_script")/.." && pwd)"
  fi
fi
if [ -z "$PLUGIN_ROOT" ] && [ -f "$(pwd)/lib/setup-mandatory-files.sh" ]; then
  PLUGIN_ROOT="$(pwd)"
fi
bash "${PLUGIN_ROOT}/lib/setup-mandatory-files.sh" "$(pwd)"
```

</details>
