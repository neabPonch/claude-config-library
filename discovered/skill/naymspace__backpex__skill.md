---
name: naymspace__backpex__skill
source: https://github.com/naymspace/backpex/blob/3ede4e9d0d45e76d0d675dcade4fb4bd842c09ce/skills/create-field/SKILL.md
repo: naymspace/backpex
kind: skill
stars: 838
last_pushed: 2026-06-16T16:52:38Z
license: mit
score: 9
domains: [web-development, elixir-phoenix]
tags: [backpex, elixir, phoenix-liveview, custom-components]
curated: 2026-06-16
curated_by: config-scout
---

# naymspace/backpex — skill

**Why it's worth keeping:** Uses rich lookup tables for options/assigns and provides a complete 'Implementation-to-Integration' workflow with concrete examples.

**Summary:** Provides a highly structured technical manual for creating and integrating custom field types within the Backpex admin framework.

**Source credibility:** High; backed by a popular, actively maintained Phoenix LiveView library (838 stars).

**Recency:** Current; aligns with modern Elixir/LiveView development patterns.

**Source:** [naymspace/backpex/skills/create-field/SKILL.md](https://github.com/naymspace/backpex/blob/3ede4e9d0d45e76d0d675dcade4fb4bd842c09ce/skills/create-field/SKILL.md) · 838★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: create-field
description: Use when creating custom Backpex field types, implementing the Backpex.Field behaviour, or adding fields to a LiveResource's fields/0 callback.
---

# Creating Backpex Fields

You are an expert at creating fields for Backpex, a Phoenix LiveView admin panel library. When the user wants to add or create a field, follow this process:

1. **Determine if a built-in field works** from the list below
2. **If custom**, generate a module implementing `Backpex.Field`
3. **Wire it into the LiveResource** by updating the `fields/0` callback

## Built-in Field Modules

| Module | Use for |
|--------|---------|
| `Backpex.Fields.Text` | Single-line text inputs |
| `Backpex.Fields.Textarea` | Multi-line text inputs |
| `Backpex.Fields.Number` | Numeric values |
| `Backpex.Fields.Boolean` | Checkboxes / toggles |
| `Backpex.Fields.Select` | Dropdown with static options |
| `Backpex.Fields.MultiSelect` | Multi-value dropdown |
| `Backpex.Fields.Date` | Date picker |
| `Backpex.Fields.DateTime` | Date and time picker |
| `Backpex.Fields.Time` | Time picker |
| `Backpex.Fields.Currency` | Formatted currency values |
| `Backpex.Fields.URL` | URLs with link rendering
```

</details>
