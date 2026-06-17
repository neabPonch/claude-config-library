---
name: kbyjoel__castor-starter-old__claude
source: https://github.com/kbyjoel/castor-starter-old/blob/5b9dce8c6e17785926adfd4e8f747697bd60c176/resources/CLAUDE.md
repo: kbyjoel/castor-starter-old
kind: claude-md
stars: 0
last_pushed: 2026-04-21T11:47:31Z
license: unknown
score: 8
domains: [backend, php, web-development]
tags: [symfony, monorepo, phpunit, docker]
curated: 2026-06-16
curated_by: config-scout
---

# kbyjoel/castor-starter-old — claude-md

**Why it's worth keeping:** Excellent command categorization (Lifecycle vs QA vs Tests) and clear explanation of the monorepo's unique 'sandbox vs bundle' relationship.

**Summary:** Defines a complex Symfony multi-bundle architecture and its dedicated sandbox testing environment.

**Source credibility:** Low social proof, but the technical documentation depth suggests a highly professional setup.

**Recency:** Very current; references PHP 8.3+ and modern tool versions like Doctrine 3.6.

**Source:** [kbyjoel/castor-starter-old/resources/CLAUDE.md](https://github.com/kbyjoel/castor-starter-old/blob/5b9dce8c6e17785926adfd4e8f747697bd60c176/resources/CLAUDE.md) · 0★

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
