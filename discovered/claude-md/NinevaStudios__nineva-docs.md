---
name: NinevaStudios__nineva-docs
source: https://github.com/NinevaStudios/nineva-docs/blob/c4ce0007b0b7ee835beba6f54f358efea63838ee/CLAUDE.md
repo: NinevaStudios/nineva-docs
kind: claude-md
stars: 5
last_pushed: 2026-05-22T05:57:59Z
license: unknown
score: 8
domains: [documentation, web-frontend]
tags: [docsify, static-site, markdown]
curated: 2026-06-15
curated_by: config-scout
---

# NinevaStudios/nineva-docs — claude-md

**Why it's worth keeping:** It explicitly documents 'non-obvious' constraints like manual search index maintenance and the requirement to omit .md extensions in internal links.

**Summary:** Provides critical technical context for a Docsify-based static site that lacks a build step and has specific routing requirements.

**Source credibility:** Small, niche repo with recent activity (1 month ago).

**Recency:** Highly current, specifically mentioning Claude Code and modern workflows.

**Source:** [NinevaStudios/nineva-docs/CLAUDE.md](https://github.com/NinevaStudios/nineva-docs/blob/c4ce0007b0b7ee835beba6f54f358efea63838ee/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

A static documentation site for Nineva Studios' Unreal Engine, Unity, and Godot plugins. Content is plain Markdown rendered client-side by Docsify — there is **no build step**. The repo also contains a small Firebase Hosting config and a Jenkins pipeline that deploys to https://docs.ninevastudios.com.

A companion `AGENTS.md` covers the same ground for other agents; keep the two files consistent if either is updated.

## Common commands

- **Local preview**: `docsify serve docs` (install once with `npm i -g docsify-cli`). The site is served as-is from `docs/`.
- **Deploy**: `firebase deploy` against project `nineva-documentation` (see `.firebaserc`). In CI this is invoked by `Jenkinsfile` using `$FIREBASE_TOKEN`; manual deploys generally aren't needed.

There are no tests, no linter, no package.json — don't add them unless explicitly asked.

## Architecture notes (the non-obvious parts)

- **Single-page site, runtime-rendered.** `docs/index.html` is the only HTML shell. It loads Docsify from CDN and configures it inline via `window.$docsify`. Ev
```

</details>
