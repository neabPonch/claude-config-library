---
name: MicYou-Dev__Website-MicYou__skill
source: https://github.com/MicYou-Dev/Website-MicYou/blob/c8030a2c24544e281e45cf26ac655d9d94f7e502/.agent/Skill.md
repo: MicYou-Dev/Website-MicYou
kind: skill
stars: 8
last_pushed: 2026-06-11T10:02:01Z
license: mit
score: 7
domains: [web-frontend, documentation-management]
tags: [vitepress, i18n, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# MicYou-Dev/Website-MicYou — skill

**Why it's worth keeping:** Uses highly effective 'Trigger -> Steps' patterns and includes specific verification workflows (sync-check) to ensure data consistency across locales.

**Summary:** Defines a structured skill set for managing multi-language documentation and components in a VitePress/Vue project.

**Source credibility:** Low star count; likely internal project documentation for a specific tool website.

**Recency:** 

**Source:** [MicYou-Dev/Website-MicYou/.agent/Skill.md](https://github.com/MicYou-Dev/Website-MicYou/blob/c8030a2c24544e281e45cf26ac655d9d94f7e502/.agent/Skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill Definitions - MicYou Website

This document defines available skills and workflows for the project.

## Available Skills

### 1. Add Document (add-doc)

Add a new documentation page with automatic multi-language translation and navigation config.

**Trigger**: User requests to add a new documentation page

**Steps**:
1. Create Chinese Markdown file in `src/docs/`
2. Create English version in `src/en/docs/`
3. Create Traditional Chinese version in `src/zh-TW/docs/`
4. Update sidebar config in `src/docs/sidebar.ts`
5. Update language files in `.vitepress/data/lang/` if needed

**Template**:

```markdown
---
title: Document Title - Site Name
description: Brief description for SEO (150-160 characters recommended).
---

# Document Title

Content...
```

**Frontmatter Requirements:**

| Field | Description | Example |
|-------|-------------|---------|
| `title` | Page title with site name suffix | `快速开始 - MicYou 安装配置指南` |
| `description` | SEO description | `MicYou 快速开始指南，详细介绍如何安装和配置 MicYou。` |

**Note:** Homepage uses `layout: home` configuration instead of standard frontmatter.

---

### 2. Update i18n (update-i18n)

Update or add new translation content.

**Trigger**: User req
```

</details>
