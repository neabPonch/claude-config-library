---
name: compound-life-ai__Turri
source: https://github.com/compound-life-ai/Turri/blob/582389f84775804179791efdac47e796b339e98b/skill.md
repo: compound-life-ai/Turri
kind: skill
stars: 7
last_pushed: 2026-04-06T04:32:32Z
license: unknown
score: 9
domains: [agents-ai, health-tech, cli-tools]
tags: [meta-skill, routing, onboarding, environment-awareness]
curated: 2026-06-16
curated_by: config-scout
---

# compound-life-ai/Turri — skill

**Why it's worth keeping:** It utilizes shell commands for real-time file/state detection and implements strict delegation logic ('route, don't play doctor') to ensure specialized agents handle sensitive reasoning.

**Summary:** An advanced meta-skill that acts as an intelligent router and onboarding orchestrator for a multi-agent health system. It uses environmental state checks to tailor its personality and guidance based on existing data.

**Source credibility:** Low star count, but the density of specific system architecture suggests a high-effort personal project.

**Recency:** Very current; uses modern patterns for directory awareness and agentic routing.

**Source:** [compound-life-ai/Turri/skill.md](https://github.com/compound-life-ai/Turri/blob/582389f84775804179791efdac47e796b339e98b/skill.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: compound-clawskill
description: Meta-skill for the Turri bundle that routes natural language health conversations to the right capability — nutrition logging, health profile, pattern discovery, experiments, news, or daily coaching.
user-invocable: true
---

# Turri

Use this skill when:

- the user wants an overview of everything available in this repository
- the user wants to know how to install the bundled skills in this directory
- the user sends a health-related message that could be handled by one of the sub-skills
- the user wants links to the repository or the bundled skill directories
- the user asks "what can you do?", "help", "get started", or anything that suggests they want orientation

## Welcome and orientation

When the user asks what you can do, wants an overview, or appears to be new, **run the status check first** to tailor your response:

```bash
profile_exists=false; whoop_connected=false; has_meals=false; has_experiments=false; has_news=false
[ -f "{baseDir}/longevityOS-data/health/profile.json" ] && profile_exists=true
[ -f "{baseDir}/longevityOS-data/health/whoop_tokens.json" ] && whoop_connected=true
[ -f "{baseDir}/longevityOS-data/nutrition/meal
```

</details>
