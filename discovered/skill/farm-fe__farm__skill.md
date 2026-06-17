---
name: farm-fe__farm__skill
source: https://github.com/farm-fe/farm/blob/2000ef8a790a1b565d1687cfe70564270a826e15/.claude/skills/a5c-ai-docusaurus/SKILL.md
repo: farm-fe/farm
kind: skill
stars: 5577
last_pushed: 2026-06-14T13:57:04Z
license: mit
score: 8
domains: [web-frontend, documentation-tools]
tags: [docusaurus, react, automation]
curated: 2026-06-16
curated_by: config-scout
---

# farm-fe/farm — skill

**Why it's worth keeping:** Includes high-quality, production-ready templates for configuration, sidebars, and custom React components which the agent can use as grounding data to avoid hallucinations.

**Summary:** A specialized skill definition that provides a structured workflow for managing Docusaurus documentation sites via specific actions.

**Source credibility:** High-quality technical structure originating from a well-regarded web build tool repository.

**Recency:** Current; utilizes modern schema-driven prompting patterns suitable for advanced agents.

**Source:** [farm-fe/farm/.claude/skills/a5c-ai-docusaurus/SKILL.md](https://github.com/farm-fe/farm/blob/2000ef8a790a1b565d1687cfe70564270a826e15/.claude/skills/a5c-ai-docusaurus/SKILL.md) · 5577★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: a5c-ai-docusaurus
description: Deep integration with Docusaurus for documentation site
  development. Configure projects, manage sidebars, versioning, i18n, develop
  plugins, and optimize builds for React-based documentation.
allowed-tools: Read, Write, Edit, Bash, Glob, Grep
backlog-id: SK-002
metadata:
  author: babysitter-sdk
  version: 1.0.0
---

# Docusaurus Skill

Deep integration with Docusaurus for documentation site development.

## Capabilities

- Generate Docusaurus project configuration
- Create and manage sidebar structures (sidebars.js)
- Configure versioning and i18n
- Develop custom Docusaurus plugins
- MDX component creation and integration
- Build optimization and debugging
- Algolia DocSearch configuration
- Theme customization

## Usage

Invoke this skill when you need to:
- Set up a new Docusaurus documentation site
- Configure sidebars and navigation
- Implement versioned documentation
- Add internationalization (i18n)
- Create custom plugins or themes

## Inputs

| Parameter | Type | Required | Description |
|-----------|------|----------|-------------|
| action | string | Yes | init, configure, sidebar, version, i18n, plugin |
| projectPath | stri
```

</details>
