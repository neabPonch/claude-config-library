---
name: basecamp__lexxy__skill
source: https://github.com/basecamp/lexxy/blob/9e796964eecd5c1502613ffde3b827c50b239ece/.claude/skills/bugs-reproducer/SKILL.md
repo: basecamp/lexxy
kind: skill
stars: 1114
last_pushed: 2026-06-15T09:01:22Z
license: mit
score: 9
domains: [web-frontend, rails-backend, quality-assurance]
tags: [debugging, reproduction-steps, test-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# basecamp/lexxy — skill

**Why it's worth keeping:** It provides a clear decision tree for selecting test suites and detailed guidance on simulating human-like browser events to ensure reproduction accuracy.

**Summary:** A highly specialized debugging orchestration file that classifies bugs into two distinct technical domains (JS core vs. Rails integration) and prescribes the correct testing tool for each.

**Source credibility:** High; Lexxy is a popular, well-maintained Rails gem/npm package with significant community backing.

**Recency:** Current; utilizes modern testing stacks like Playwright and Capybara suitable for today's Claude Code capabilities.

**Source:** [basecamp/lexxy/.claude/skills/bugs-reproducer/SKILL.md](https://github.com/basecamp/lexxy/blob/9e796964eecd5c1502613ffde3b827c50b239ece/.claude/skills/bugs-reproducer/SKILL.md) · 1114★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bugs-reproducer
description: |
  Bug reproduction for the Lexxy rich text editor. Core editing bugs use
  Playwright (Selenium fallback); system-level bugs use Capybara. All local.
disable-model-invocation: true
---

# Bugs Reproducer

Reproduce bugs in Lexxy — a rich text editor built on [Lexical](https://lexical.dev/), distributed as a Rails gem and npm package. Lexxy replaces Trix as the rich text editor for Rails Action Text.

```
BUG REPORT → CLASSIFY → REPRODUCE → DIAGNOSE → FIX → VERIFY
                          ^^^^^^^^^
                          core editing bug → Playwright (Selenium fallback)
                          system-level bug → Capybara
```

## Understanding Lexxy

Lexxy wraps Lexical in a set of custom elements (`<lexxy-editor>`, `<lexxy-toolbar>`, `<lexxy-table-tools>`, etc.) and extends it with custom nodes, extensions, and an Action Text integration layer. Before writing reproduction steps, understand which layer the bug likely lives in:

**Editor core** — The `<lexxy-editor>` custom element (`src/elements/editor.js`) owns the Lexical editor instance. It is `FormAssociated`, manages the `value` (sanitized HTML) lifecycle, handles Turbo reconnection
```

</details>
