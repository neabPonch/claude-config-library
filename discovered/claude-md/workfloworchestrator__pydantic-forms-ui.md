---
name: workfloworchestrator__pydantic-forms-ui
source: https://github.com/workfloworchestrator/pydantic-forms-ui/blob/513ed881aa017ffee1b6d71600cfc30377f4575c/CLAUDE.md
repo: workfloworchestrator/pydantic-forms-ui
kind: claude-md
stars: 15
last_pushed: 2026-06-04T08:43:51Z
license: unknown
score: 9
domains: [web-frontend, backend-api, monorepo]
tags: [fastapi, nextjs, npm-workspaces, python-venv]
curated: 2026-06-14
curated_by: config-scout
---

# workfloworchestrator/pydantic-forms-ui — claude-md

**Why it's worth keeping:** It explains the high-level logic flow (the 'how it works') rather than just commands, and includes explicit steps for virtual environment activation which is crucial for agentic reliability.

**Summary:** Provides a comprehensive guide for a complex Python/React monorepo, covering architecture, command workflows, and environmental setup.

**Source credibility:** Low star count suggests a niche or newer package, but the documentation depth is highly professional.

**Recency:** Very current, referencing modern tech stacks like Next.js 14-16 and Tailwind CSS 4.

**Source:** [workfloworchestrator/pydantic-forms-ui/CLAUDE.md](https://github.com/workfloworchestrator/pydantic-forms-ui/blob/513ed881aa017ffee1b6d71600cfc30377f4575c/CLAUDE.md) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This repository demonstrates how to use the pydantic-forms library to automatically generate frontend forms from Pydantic models. It consists of:
- A FastAPI backend that defines Pydantic models with validation rules
- A React frontend (Next.js) that dynamically renders forms based on JSON schemas
- A publishable npm package (`pydantic-forms`) that provides the form generation logic

## Repository Structure

### Monorepo Layout
This is a npm workspace monorepo with the following structure:

```
├── backend/                      # FastAPI application
│   ├── main.py                   # Main API with form endpoints
│   ├── demo.py                   # Additional demo forms
│   └── tests/                    # Backend tests
├── frontend/                     # Frontend monorepo (npm workspace)
│   ├── packages/
│   │   └── pydantic-forms/       # NPM package for form generation
│   │       ├── src/
│   │       │   ├── components/   # Form field components
│   │       │   ├── core/         # Core form logic (hooks, handlers)
│   │       │   ├── PydanticForm.tsx
```

</details>
