---
name: seo-skills__seo-audit-skill
source: https://github.com/seo-skills/seo-audit-skill/blob/85378025bb0aad504e5c81dc9c5564f136180c2a/claude.md
repo: seo-skills/seo-audit-skill
kind: claude-md
stars: 285
last_pushed: 2026-05-08T16:40:17Z
license: mit
score: 9
domains: [cli-tools, desktop-app, node.js]
tags: [dual-purpose, electron, dependency-management, rule-engine]
curated: 2026-06-16
curated_by: config-scout
---

# seo-skills/seo-audit-skill — claude-md

**Why it's worth keeping:** The 'Critical Rules' section provides high-value constraints on package.json fields that prevent breaking the application. The detailed workflow for adding new rules is an excellent template for AI agent extensibility.

**Summary:** A highly specific guide for maintaining a dual-purpose CLI and Electron project, preventing dependency bloating and entry-point errors. It also defines the architectural pattern for a self-registering rule engine.

**Source credibility:** High; 285 stars and recent activity suggest a well-maintained, real-world tool.

**Recency:** 

**Source:** [seo-skills/seo-audit-skill/claude.md](https://github.com/seo-skills/seo-audit-skill/blob/85378025bb0aad504e5c81dc9c5564f136180c2a/claude.md) · 285★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

SEOmator is a comprehensive SEO audit tool (`@seomator/seo-audit`) with 251 rules across 20 categories. It ships as both a **CLI tool** (published to npm) and an **Electron desktop app** (local only). It fetches web pages, parses HTML with Cheerio, optionally measures Core Web Vitals via Playwright, and scores pages against SEO best practices.

## Critical Rules (read before making changes)

### package.json Dual-Purpose Constraints

The `package.json` serves **both** the npm CLI package and the Electron desktop app. These fields have strict requirements:

| Field | Value | Why |
|-------|-------|-----|
| `main` | `./dist-electron/main/index.js` | **Electron reads this** to find the main process entry. DO NOT change to `./dist/cli.js` or Electron will execute Commander CLI instead of launching the app window. |
| `exports` | `./dist/cli.js` | **npm/Node.js consumers use this** for programmatic imports. Takes priority over `main` in modern Node.js. |
| `bin` | `./dist/cli.js` | **npm CLI users use this** (`seomator` command). |
| `files` | `["dist
```

</details>
