---
name: MaterializeInc__materialize__index-skill
source: https://github.com/MaterializeInc/materialize/blob/aeab441868b66fef4ad7e67feea1f8abe7912be1/doc/user/layouts/index.skill.md
repo: MaterializeInc/materialize
kind: skill
stars: 6314
last_pushed: 2026-06-15T17:26:28Z
license: other
score: 8
domains: [data-engineering, documentation-automation]
tags: [template, indexing, navigation-guide]
curated: 2026-06-15
curated_by: config-scout
---

# MaterializeInc/materialize — skill

**Why it's worth keeping:** It implements an 'index-first' navigation pattern, teaching the agent exactly which directories to explore for specific intents to minimize token waste.

**Summary:** A Hugo template that auto-generates structured SKILL.md files by mapping documentation sections to specific file paths and providing high-level command summaries.

**Source credibility:** High; Materialize is a prominent, highly-starred (6k+) streaming database project.

**Recency:** Current; perfectly aligned with modern tool-augmented agentic workflows that require efficient document discovery.

**Source:** [MaterializeInc/materialize/doc/user/layouts/index.skill.md](https://github.com/MaterializeInc/materialize/blob/aeab441868b66fef4ad7e67feea1f8abe7912be1/doc/user/layouts/index.skill.md) · 6314★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
{{- /* Home page template - generates SKILL.md for Claude */ -}}
---
name: materialize-docs
description: Materialize documentation for SQL syntax, data ingestion, concepts, and best practices. Use when users ask about Materialize queries, sources, sinks, views, or clusters.
---

# Materialize Documentation

This skill provides comprehensive documentation for Materialize, a streaming database for real-time analytics.

## How to Use This Skill

When a user asks about Materialize:

1. **For SQL syntax/commands**: Read files in the `sql/` directory
2. **For core concepts**: Read files in the `concepts/` directory
3. **For data ingestion**: Read files in the `ingest-data/` directory
4. **For transformations**: Read files in the `transform-data/` directory

## Documentation Sections
{{- range .Site.Sections }}
{{- $sectionName := .Section }}
{{- if not (in (slice "releases" "self-managed" "about" "get-started") $sectionName) }}

### {{ .Title }}
{{- with .Description }}
{{ . }}
{{- end }}
{{ range .Pages | first 10 }}
- **{{ .Title }}**: `{{ strings.TrimPrefix "/" .RelPermalink }}`
{{- end }}
{{- if gt (len .Pages) 10 }}
- _(and {{ sub (len .Pages) 10 }} more files in this section)_
{{-
```

</details>
