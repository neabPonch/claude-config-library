---
name: kanopi__drupal-starter
source: https://github.com/kanopi/drupal-starter/blob/a503ced00479b5e0f09b41b647b798f4ad74c12f/CLAUDE.md
repo: kanopi/drupal-starter
kind: claude-md
stars: 16
last_pushed: 2026-06-05T21:59:17Z
license: unknown
score: 9
domains: [web-development, cms, devops]
tags: [drupal, ddev, workflow-automation, component-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# kanopi/drupal-starter — claude-md

**Why it's worth keeping:** The inclusion of explicit naming conventions (e.g., 'sa_' prefix), categorized CLI commands, and mandatory pre-commit checklists provides the specific guardrails an AI agent needs to work autonomously without breaking project standards.

**Summary:** A comprehensive guide for a complex Drupal development environment using DDEV and Pantheon. It covers command sets, architectural patterns, and strict testing requirements.

**Source credibility:** High; produced by a professional Drupal agency for a structured starter kit.

**Recency:** Very current; mentions Drupal 11 and PHP 8.3.

**Source:** [kanopi/drupal-starter/CLAUDE.md](https://github.com/kanopi/drupal-starter/blob/a503ced00479b5e0f09b41b647b798f4ad74c12f/CLAUDE.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a modern Drupal 11 starter project configured for Pantheon hosting with comprehensive development tooling. It includes:

- Drupal Recipes system for modular functionality
- Component-based architecture using Saplings theme system
- Comprehensive testing and code quality tools
- DDEV local development using the kanopi/ddev-kanopi-drupal add-on

## Development Commands

### Local Development Setup

This project uses the [kanopi/ddev-kanopi-drupal](https://github.com/kanopi/ddev-kanopi-drupal) add-on which provides 27+ custom commands.

**Initial Setup:**
```bash
ddev config --project-type=drupal11 --docroot=web --database=mariadb:10.6
ddev start
ddev add-on get kanopi/ddev-kanopi-drupal
ddev project-configure       # Interactive configuration for project settings
ddev project-init            # Initialize with dependencies and database
```

**Common Commands:**
```bash
ddev project-init            # Initialize local environment from scratch
ddev db-rebuild              # Run composer install and refresh database
ddev db-refresh [env] -f
```

</details>
