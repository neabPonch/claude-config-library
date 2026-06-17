---
name: gabrielmoreira__agent-skills-mirror__claude
source: https://github.com/gabrielmoreira/agent-skills-mirror/blob/656c913d1465fe2e4b2c362656e27545997c7003/mirrors/repos/algoderiv@agent-skills/CLAUDE.md
repo: gabrielmoreira/agent-skills-mirror
kind: claude-md
stars: 9
last_pushed: 2026-06-15T04:55:10Z
license: mit
score: 7
domains: [agents-ai, cli-tools]
tags: [skill-management, agent-instructions, structured-knowledge]
curated: 2026-06-15
curated_by: config-scout
---

# gabrielmoreira/agent-skills-mirror — claude-md

**Why it's worth keeping:** Establishes strict naming conventions and required file mappings to ensure agents can reliably navigate specialized documentation and executable scripts.

**Summary:** Defines a formalized system for packaging and installing domain-specific 'skills' directly into the Claude Code environment.

**Source credibility:** Low star count (9), but provides a highly technical and structured specification rather than generic advice.

**Recency:** Very current; specifically addresses Claude Code's installation patterns for skills.

**Source:** [gabrielmoreira/agent-skills-mirror/mirrors/repos/algoderiv@agent-skills/CLAUDE.md](https://github.com/gabrielmoreira/agent-skills-mirror/blob/656c913d1465fe2e4b2c362656e27545997c7003/mirrors/repos/algoderiv@agent-skills/CLAUDE.md) · 9★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AGENTS.md

This file provides guidance to AI coding agents (Claude Code, Cursor, Copilot, etc.) when working with code in this repository.

## Repository Overview

A collection of skills for AI coding agents focused on quantitative trading development, video generation APIs, and payment platform integrations. Skills are packaged instructions and reference documentation that extend agent capabilities for CTP futures/options trading, market data APIs, algorithmic trading platforms, WonderTrader/wtpy quantitative trading development, Seedance video generation, and Stripe payment integration.

## Skill Structure

```
skills/
  {skill-name}/           # kebab-case directory name
    SKILL.md              # Required: skill definition
    references/           # Required: supporting documentation
      {topic}.md          # Reference files loaded on demand
    scripts/              # Optional: executable scripts
    assets/               # Optional: static assets
  {skill-name}.zip        # Required: packaged for distribution
```

### Naming Conventions

- **Skill directory**: `kebab-case` (e.g., `ctp-api`, `rice-quant`)
- **SKILL.md**: Always uppercase, always this exact filename
- **R
```

</details>
