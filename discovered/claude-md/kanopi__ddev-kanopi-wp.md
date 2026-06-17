---
name: kanopi__ddev-kanopi-wp
source: https://github.com/kanopi/ddev-kanopi-wp/blob/c9ca2aa4b08c6209ea99e35cec178c71dfd06ada/CLAUDE.md
repo: kanopi/ddev-kanopi-wp
kind: claude-md
stars: 1
last_pushed: 2026-05-31T14:14:30Z
license: gpl-2.0
score: 9
domains: [cli-tools, web-development, devops]
tags: [ddev, wordpress, workflows, hosting]
curated: 2026-06-15
curated_by: config-scout
---

# kanopi/ddev-kanopi-wp — claude-md

**Why it's worth keeping:** It uses clear categorization (Host vs Web commands) and provides explicit mappings of environment variables and provider-specific configurations that an agent can use to troubleshoot or execute workflows.

**Summary:** A highly detailed technical manual for a custom DDEV-based WordPress development ecosystem with multi-provider support.

**Source credibility:** High; comes from a specialized, actively maintained DDEV add-on repository.

**Recency:** Current; aligns with modern containerized development and CLI-driven workflows.

**Source:** [kanopi/ddev-kanopi-wp/CLAUDE.md](https://github.com/kanopi/ddev-kanopi-wp/blob/c9ca2aa4b08c6209ea99e35cec178c71dfd06ada/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a DDEV add-on that provides Kanopi's battle-tested workflow for WordPress development with multi-provider hosting support. The add-on includes 26 custom commands, enhanced provider integration for Pantheon, WPEngine, and Kinsta, and complete tooling for modern WordPress development.

## Architecture

### Command Structure
Commands are organized into two categories:
- **Host commands** (`commands/host/`): Execute on the host system outside containers
- **Web commands** (`commands/web/`): Execute inside the DDEV web container

The add-on uses a **modular command approach** where `project-init` orchestrates multiple smaller, focused commands:
- `project-auth`: Handle SSH key authorization for hosting providers
- `project-lefthook`: Install and initialize Lefthook git hooks
- `project-wp`: Install WordPress core and database if needed
- `project-configure`: Interactive configuration wizard

### Core Components
- `install.yaml`: Add-on installation configuration and post-install actions
- `commands/`: Custom DDEV commands for development workf
```

</details>
