---
name: aropixel__castor-starter__claude
source: https://github.com/aropixel/castor-starter/blob/55dbc2058002ba65de3f192c78d9e30e70f36fb3/resources/CLAUDE.md
repo: aropixel/castor-starter
kind: claude-md
stars: 1
last_pushed: 2026-04-29T10:06:55Z
license: mit
score: 9
domains: [php, symfony, backend]
tags: [monorepo, task-runner, sandbox]
curated: 2026-06-16
curated_by: config-scout
---

# aropixel/castor-starter — claude-md

**Why it's worth keeping:** Crucially defines the 'sandbox' constraint to prevent Claude from editing production-like code in the wrong place, and provides precise CLI patterns for running tests and QA tools.

**Summary:** Defines a monorepo workflow for Symfony bundles using a dedicated sandbox and 'Castor' task runner. It emphasizes the specific relationship between bundle development and the testing environment.

**Source credibility:** Single-star repo; appears to be a professional boilerplate/starter kit for specific Symfony workflows.

**Recency:** Very recent (2 months ago) and reflects modern PHP 8.3+ development standards.

**Source:** [aropixel/castor-starter/resources/CLAUDE.md](https://github.com/aropixel/castor-starter/blob/55dbc2058002ba65de3f192c78d9e30e70f36fb3/resources/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A contribution environment for the **Aropixel open source bundles** — a CMS admin suite for Symfony. The goal is to develop and test changes to these bundles:

- **AdminBundle** (`admin-bundle/`) — Core bundle: admin UI, user management, CRUD generation. BlogBundle, PageBundle, and MenuBundle are dependencies of AdminBundle.
- **BlogBundle** (`blog-bundle/`) — Blog/news content management
- **PageBundle** (`page-bundle/`) — Page/subpage management
- **MenuBundle** (`menu-bundle/`) — Navigation menu management

The `application/` directory is a **Symfony sandbox** used exclusively to test bundle modifications. It is not a deliverable — its sole purpose is to provide a working Symfony app where all four bundles are installed and exercisable.

The sandbox uses Docker-first infrastructure via the JoliCode Docker Starter (v4) with **Castor** as the task runner.

## Commands

All commands use **Castor** (PHP CLI task runner). The infrastructure runs inside Docker containers.

### Development Lifecycle

```bash
castor start          # Build images, inst
```

</details>
