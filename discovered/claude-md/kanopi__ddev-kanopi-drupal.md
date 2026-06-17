---
name: kanopi__ddev-kanopi-drupal
source: https://github.com/kanopi/ddev-kanopi-drupal/blob/0a62ff39ba471d07be63b4397d44f63b5f38d4bc/CLAUDE.md
repo: kanopi/ddev-kanopi-drupal
kind: claude-md
stars: 3
last_pushed: 2026-05-31T14:14:33Z
license: gpl-2.0
score: 9
domains: [cli-tools, devops, drupal]
tags: [ddev, workflow-automation, infrastructure]
curated: 2026-06-15
curated_by: config-scout
---

# kanopi/ddev-kanopi-drupal — claude-md

**Why it's worth keeping:** It provides clear distinctions between host/web commands, explicit mapping of environment variable locations, and reusable templates for creating new scripts.

**Summary:** A comprehensive technical manual for a custom DDEV command suite that handles complex Drupal development workflows and hosting integrations.

**Source credibility:** High-quality specialized tooling with recent activity and established star count.

**Recency:** Highly current; reflects modern DDEV and Drupal development patterns.

**Source:** [kanopi/ddev-kanopi-drupal/CLAUDE.md](https://github.com/kanopi/ddev-kanopi-drupal/blob/0a62ff39ba471d07be63b4397d44f63b5f38d4bc/CLAUDE.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a DDEV add-on that provides Kanopi's battle-tested workflow for Drupal development with multi-provider hosting support. The add-on includes 27 custom commands, enhanced provider integration for Pantheon and Acquia, and complete tooling for modern Drupal development.

## Architecture

### Command Structure
Commands are organized into two categories:
- **Host commands** (`commands/host/`): Execute on the host system outside containers
- **Web commands** (`commands/web/`): Execute inside the DDEV web container

### Core Components
- `install.yaml`: Add-on installation configuration and post-install actions
- `commands/`: Custom DDEV commands for development workflow
- `providers/`: Enhanced Pantheon provider configuration (not in this repo but created during installation)

## Common Development Commands

### Essential Commands
- `ddev project-init`: Complete project initialization with dependencies, Lefthook, NVM, and database refresh
- `ddev project-configure`: Interactive configuration wizard for project setup
- `ddev auth ssh`: Adds SSH k
```

</details>
