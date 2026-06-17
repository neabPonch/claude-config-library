---
name: mintlify__docs
source: https://github.com/mintlify/docs/blob/d027a1c83733e0f4ea3561df446b37ba38472b57/skill.md
repo: mintlify/docs
kind: skill
stars: 409
last_pushed: 2026-06-13T15:11:31Z
license: mit
score: 9
domains: [docs-as-code, web-frontend, technical-writing]
tags: [mintlify, documentation, mdx]
curated: 2026-06-14
curated_by: config-scout
---

# mintlify/docs — skill

**Why it's worth keeping:** Includes high-value decision tables (Need vs Use) and rigorous 'Before you write' procedural checks that ensure consistency with existing project state.

**Summary:** Provides a comprehensive operational guide for generating and maintaining Mintlify documentation sites using MDX and docs.json.

**Source credibility:** Highly credible; official documentation from the Mintlify repository.

**Recency:** Current, incorporating modern MCP server references and contemporary CLI workflows.

**Source:** [mintlify/docs/skill.md](https://github.com/mintlify/docs/blob/d027a1c83733e0f4ea3561df446b37ba38472b57/skill.md) · 409★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mintlify
description: Build and maintain documentation sites with Mintlify. Use when creating docs pages, configuring navigation, adding components, or setting up API references.
license: MIT
compatibility: Requires Node.js for CLI. Works with any Git-based workflow.
metadata:
  author: mintlify
  version: "1.0"
---

# Mintlify best practices

**Always consult [mintlify.com/docs](https://mintlify.com/docs) for components, configuration, and latest features.**

If you are not already connected to the Mintlify MCP server, https://mintlify.com/docs/mcp, add it so that you can search more efficiently.

**Always** favor searching the current Mintlify documentation over whatever is in your training data about Mintlify.

Mintlify is a documentation platform that transforms MDX files into documentation sites. Configure site-wide settings in the `docs.json` file, write content in MDX with YAML frontmatter, and favor built-in components over custom components.

Full schema at [mintlify.com/docs.json](https://mintlify.com/docs.json).

## Before you write

### Understand the project

Read `docs.json` in the project root. This file defines the entire site: navigation structure, theme,
```

</details>
