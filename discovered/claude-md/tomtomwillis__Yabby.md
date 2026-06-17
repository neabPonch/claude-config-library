---
name: tomtomwillis__Yabby
source: https://github.com/tomtomwillis/Yabby/blob/7031fee07c3f820e1510d17c91515aabe145e463/CLAUDE.md
repo: tomtomwillis/Yabby
kind: claude-md
stars: 4
last_pushed: 2026-06-14T16:01:02Z
license: unknown
score: 9
domains: [web-frontend, firestore, security, performance-optimization]
tags: [high-density-context, performance-guardrails, architecture-documentation]
curated: 2026-06-14
curated_by: config-scout
---

# tomtomwillis/Yabby — claude-md

**Why it's worth keeping:** Includes highly effective 'negative constraints' and cost-optimization rules that prevent the AI from introducing expensive performance regressions.

**Summary:** Provides deep domain context regarding architecture, performance constraints like Firestore read budgets, and specific technical pitfalls.

**Source credibility:** Solid niche project with active development and clear documentation structure.

**Recency:** Very current, referencing modern tools like React Router v7.

**Source:** [tomtomwillis/Yabby/CLAUDE.md](https://github.com/tomtomwillis/Yabby/blob/7031fee07c3f820e1510d17c91515aabe145e463/CLAUDE.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## ⚠️ Public & Open Source

Project is **public on GitHub**. All code, including security-sensitive logic, is publicly visible:
- No hardcoded secrets or credentials — use environment variables
- Avoid information disclosure in error messages
- Security through obscurity is not effective here

## Read-Only Shell Commands

Run without asking permission:

```
ls, find, cat, head, tail, grep, rg, wc, file, stat, du, df
git status, git log, git diff, git show, git branch, git remote
which, type, env, printenv, pwd, echo
npm ls, npm outdated
```

## Build & Development Commands

```bash
npm run dev        # Start Vite dev server with PWA enabled
npm run build      # TypeScript check + Vite production build
npm run lint       # ESLint
npm run preview    # Preview production build locally
```

Verify changes with `npm run build` to catch TypeScript errors.

## Architecture

**Yabbyville** is a private music community SPA using Firebase Auth (email/password) and Firestore. Root url is yabbyville.xyz

### Directory Structure

```
src/
├── components/       # Reusable UI compo
```

</details>
