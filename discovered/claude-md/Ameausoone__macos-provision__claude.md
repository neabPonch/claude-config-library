---
name: Ameausoone__macos-provision__claude
source: https://github.com/Ameausoone/macos-provision/blob/98d88a973ff4b1583894e6bb9181e39950e0ca88/docs/CLAUDE.md
repo: Ameausoone/macos-provision
kind: claude-md
stars: 13
last_pushed: 2026-06-12T13:38:15Z
license: unknown
score: 7
domains: [technical-writing, content-management]
tags: [workflow, style-guide, markdown]
curated: 2026-06-15
curated_by: config-scout
---

# Ameausoone/macos-provision — claude-md

**Why it's worth keeping:** Shows how to point Claude toward external style guides and provides clear instructions for using custom slash-command skills/workflows.

**Summary:** Defines a structured technical writing workflow including status tracking, specific tone requirements, and content templates.

**Source credibility:** Personal project; highly detailed content suggests a sophisticated manual workflow.

**Recency:** Current; specifically references Claude Code and its command capabilities.

**Source:** [Ameausoone/macos-provision/docs/CLAUDE.md](https://github.com/Ameausoone/macos-provision/blob/98d88a973ff4b1583894e6bb9181e39950e0ca88/docs/CLAUDE.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this folder contains

Two types of content:

- **sfeir.dev articles** (French) — numbered with prefix `NN-<slug>.md`, intended for publication
- **Reference docs** — cheatsheets and personal notes, not for publication

## Article series: `mise`

`00-mise-articles.md` is the planning doc for the full series. It defines:
- Article topics and their order
- Two structural templates to follow (Usage/How-to vs Vision/Architecture)
- LinkedIn post drafts

Published/draft articles so far:

| File | Topic | Status |
|------|-------|--------|
| `01-mise-install.md` | Install & configure mise | Draft |
| `02-mise-backend.md` | mise backends | Draft |

## Writing conventions

- Language: **French**
- Target platform: sfeir.dev (Ghost CMS)
- Style: follow the SFEIR style guide in `~/.claude/rules/sfeir-dev.md`
- Tone: vouvoiement ("vous"), voix active, pas de fluff
- Structure: see templates in `00-mise-articles.md`

## Reviewing articles

Use the `/review-article` skill to review an article before publication:

```bash
/review-article docs/01-mise-install.md
```

The ski
```

</details>
