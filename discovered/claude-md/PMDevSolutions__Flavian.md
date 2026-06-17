---
name: PMDevSolutions__Flavian
source: https://github.com/PMDevSolutions/Flavian/blob/8b0d6b23bfc491bf12666d746af0742b600fa338/CLAUDE.md
repo: PMDevSolutions/Flavian
kind: claude-md
stars: 8
last_pushed: 2026-06-08T02:43:42Z
license: mit
score: 9
domains: [wordpress, web-development, devops-automation]
tags: [wp-cli, full-site-editing, structural-guardrails, php]
curated: 2026-06-15
curated_by: config-scout
---

# PMDevSolutions/Flavian — claude-md

**Why it's worth keeping:** The 'CRITICAL' file location section is an excellent example of preventing common LLM hallucinations regarding directory structures. The inclusion of specific, high-utility shell commands enables the agent to perform complex setup/deployment tasks autonomously.

**Summary:** Provides strict structural guardrails to prevent the agent from using standard wp-content paths in this non-standard root-level development environment. It includes highly actionable command libraries for WP-CLI and coding standards.

**Source credibility:** Highly professional structure and documentation; appears to be a specialized framework rather than a generic repo.

**Recency:** Very current; tailored specifically for modern Claude Code workflows and WordPress FSE standards.

**Source:** [PMDevSolutions/Flavian/CLAUDE.md](https://github.com/PMDevSolutions/Flavian/blob/8b0d6b23bfc491bf12666d746af0742b600fa338/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **Claude Code-integrated WordPress development template** providing a clean `wp-content` directory structure with WordPress-specific development tools and scripts.

The template is designed for:
- WordPress FSE (Full Site Editing) block theme development
- Custom WordPress plugin development
- WordPress security, performance, and accessibility auditing
- Integration with Claude Code for WordPress development workflows

## ⚠️ CRITICAL: File Location Requirements

**This project uses ROOT-LEVEL WordPress folders, NOT `wp-content/` subfolders:**

```
project-root/
├── themes/          ← Theme files go HERE (NOT wp-content/themes/)
├── plugins/         ← Plugin files go HERE (NOT wp-content/plugins/)
├── mu-plugins/      ← Must-use plugins go HERE (NOT wp-content/mu-plugins/)
└── .claude/         ← Claude Code configuration
```

**Why root-level?**
- Cleaner development structure
- Easier version control (no nested wp-content)
- Testing copies files to WordPress `wp-content/` for deployment
- Development and testing environments separated
```

</details>
