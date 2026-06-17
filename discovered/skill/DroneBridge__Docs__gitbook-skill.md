---
name: DroneBridge__Docs__gitbook-skill
source: https://github.com/DroneBridge/Docs/blob/624bd9eef9fb3e742f2a7d3e1330b4b67dec36fe/gitbook-skill.md
repo: DroneBridge/Docs
kind: skill
stars: 6
last_pushed: 2026-05-18T21:32:52Z
license: apache-2.0
score: 8
domains: [documentation, devops]
tags: [gitbook, docs-as-code, markdown]
curated: 2026-06-16
curated_by: config-scout
---

# DroneBridge/Docs — skill

**Why it's worth keeping:** The use of decision tables for block selection and explicit file structure/frontmatter schemas provides the exact level of precision needed for agentic accuracy.

**Summary:** A comprehensive technical reference for managing GitBook-synced repositories via external editors or agents.

**Source credibility:** Part of an active documentation repository; demonstrates real-world utility for 'docs-as-code' workflows.

**Recency:** Current; specifically addresses modern Git-sync and IDE integration workflows.

**Source:** [DroneBridge/Docs/gitbook-skill.md](https://github.com/DroneBridge/Docs/blob/624bd9eef9fb3e742f2a7d3e1330b4b67dec36fe/gitbook-skill.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# skill

A comprehensive guide for editing GitBook documentation in external environments like Cursor, Claude Code, or other text editors. This skill provides all the formatting syntax, configuration options, and best practices needed to create and maintain GitBook content outside the GitBook web interface.

### When to Use This Skill

Use this skill when working with GitBook documentation through:

* Git-synced repositories (GitHub, GitLab)
* Local markdown editors
* IDE integrations
* Command-line tools
* Any environment where you're editing GitBook content as files rather than through the GitBook UI

### Quick Reference

#### GitBook Content Structure

GitBook organizes content through pages, spaces, and collections:

* **Pages** are individual markdown files that make up your documentation
* **Spaces** are collections of pages organized into a documentation site
* **Collections** are groups of spaces

**File structure:**

```
/
  .gitbook/
    assets/              # GitBook-managed images and files
    includes/            # Reusable content blocks
    vars.yaml            # Space-level variables
  .gitbook.yaml          # Configuration
  README.md              # Homepage
  SUM
```

</details>
