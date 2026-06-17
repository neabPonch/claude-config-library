---
name: ericosiu__ai-marketing-skills__skill
source: https://github.com/ericosiu/ai-marketing-skills/blob/a9f11007aca31cc85f231698e22b64412f847b76/clone-site/SKILL.md
repo: ericosiu/ai-marketing-skills
kind: skill
stars: 2594
last_pushed: 2026-06-14T16:08:10Z
license: mit
score: 8
domains: [web-frontend, agents-ai, automation]
tags: [site-cloner, nextjs, parallel-execution]
curated: 2026-06-16
curated_by: config-scout
---

# ericosiu/ai-marketing-skills — skill

**Why it's worth keeping:** Uses a sophisticated 'Parallel Build' pattern via git worktrees to manage multi-agent task dispatching; provides a clear blueprint for combining tool-use (Chrome MCP) with complex architectural workflows.

**Summary:** Automates full website reverse-engineering into a Next.js and Tailwind project using visual reconnaissance and parallelized agent construction.

**Source credibility:** High popularity with over 2,500 stars and active maintenance.

**Recency:** Current, utilizing modern tech stacks like Tailwind v4 and Chrome MCP capabilities.

**Source:** [ericosiu/ai-marketing-skills/clone-site/SKILL.md](https://github.com/ericosiu/ai-marketing-skills/blob/a9f11007aca31cc85f231698e22b64412f847b76/clone-site/SKILL.md) · 2594★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---

## Preamble (runs on skill start)

```bash
# Version check (silent if up to date)
python3 telemetry/version_check.py 2>/dev/null || true

# Telemetry opt-in (first run only, then remembers your choice)
python3 telemetry/telemetry_init.py 2>/dev/null || true
```

> **Privacy:** This skill logs usage locally to `~/.ai-marketing-skills/analytics/`. Remote telemetry is opt-in only. No code, file paths, or repo content is ever collected. See `telemetry/README.md`.

---
name: clone-site
description: Clone any website into a pixel-perfect Next.js replica. Point it at a URL and it reverse-engineers the design, extracts assets, and rebuilds it section by section using parallel builder agents. Use when asked to clone, copy, replicate, rebuild, or reverse-engineer any website or landing page. Also use for "make it look like this site" or "build a page based on this URL".
---

# Clone Site

Reverse-engineer and rebuild any website as a pixel-perfect Next.js clone.

## Quick Start

User says: "Clone yourcompany.com" or "Make a landing page like this: [url]"

## How It Works

1. **Recon** — Screenshots the target at desktop + mobile, extracts all design tokens (fonts, colors, spacing), down
```

</details>
