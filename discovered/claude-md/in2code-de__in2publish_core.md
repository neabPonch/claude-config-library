---
name: in2code-de__in2publish_core
source: https://github.com/in2code-de/in2publish_core/blob/730cfed8024a3cc8acff0ee935340e03c16abed7/CLAUDE.md
repo: in2code-de/in2publish_core
kind: claude-md
stars: 40
last_pushed: 2026-06-03T09:38:16Z
license: gpl-3.0
score: 9
domains: [php, cms-typo3, devops, backend]
tags: [monorepo, docker, typo3, php-development]
curated: 2026-06-15
curated_by: config-scout
---

# in2code-de/in2publish_core — claude-md

**Why it's worth keeping:** Provides high-value 'Makefile' command mappings for operational tasks and specific framework-version guidelines (TYPO3 v13) to prevent the use of deprecated APIs. The inclusion of a 'Working Mode' section provides excellent clarity on agent autonomy vs. required approval.

**Summary:** A highly structured technical specification for a TYPO3 monorepo that details architecture, dependency injection patterns, and containerized workflows.

**Source credibility:** Active niche project with recent maintenance and updates.

**Recency:** Highly current, referencing modern PHP 8.4 and TYPO3 v14 environments.

**Source:** [in2code-de/in2publish_core/CLAUDE.md](https://github.com/in2code-de/in2publish_core/blob/730cfed8024a3cc8acff0ee935340e03c16abed7/CLAUDE.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Project: in2publish_core (Content Publisher Community Edition)

Content publishing extension to connect stage (Local) and production (Foreign) TYPO3 servers.

## TYPO3 Configuration

**TYPO3 Version**: 14.2.0-dev
**PHP Version**: 8.2 - 8.5 (running: 8.4.8)
**Extension Version**: 14.0.0 (ext_emconf) / develop-v14 (current branch)
**Extension Key**: in2publish_core
**Vendor Namespace**: In2code\In2publishCore
**Project Type**: Docker Compose + Composer Mode (monorepo)

### Project Architecture

This is a **monorepo** for the in2publish Content Publisher suite. The extension connects a **Local** (staging) TYPO3
instance with a **Foreign** (production) instance for content publishing.

Key concepts:
- **Local**: The Build/local TYPO3 instance where editors work
- **Foreign**: The Build/foreign TYPO3 instance that receives published content
- Two separate database connections (`$localDatabase`, `$foreignDatabase`) injected via DI
- Adapter pattern for SSH/HTTP/Native communication between instances

### Extension Class Structure

```
Classes/
├── Backend/          # Backend module related
├── Cache/            # Cache implementations
├── Command/          # CLI commands (Local/ and Fo
```

</details>
