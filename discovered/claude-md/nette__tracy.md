---
name: nette__tracy
source: https://github.com/nette/tracy/blob/27801ff93e238f37ea56d8c465060d0af998c968/CLAUDE.md
repo: nette/tracy
kind: claude-md
stars: 1828
last_pushed: 2026-05-25T16:58:18Z
license: other
score: 9
domains: [php, web-development, testing, debugging]
tags: [backend, testing-frameworks, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# nette/tracy — claude-md

**Why it's worth keeping:** It includes highly specific command-line instructions for unique SAPI requirements (php-cgi), defines non-standard testing syntax to prevent hallucinations, and maps out architectural design patterns.

**Summary:** This file serves as a comprehensive technical manual that explains not just the 'what' but the 'how' of the project's internal logic and testing requirements.

**Source credibility:** High; Nette is a major PHP ecosystem standard with significant community backing and recent activity.

**Recency:** Very current; it includes specialized instructions for AI agent/automated browser detection.

**Source:** [nette/tracy/CLAUDE.md](https://github.com/nette/tracy/blob/27801ff93e238f37ea56d8c465060d0af998c968/CLAUDE.md) · 1828★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Tracy is a debugging and error visualization library for PHP (8.2-8.5). It provides beautiful error pages (BlueScreen), an interactive debug toolbar (Bar), advanced variable dumping, and production-ready error logging.

**Key features:**
- BlueScreen: Beautiful error/exception visualization with stack traces
- Tracy Bar: Floating debug toolbar with extensible panel system
- Dumper: Advanced variable dumping with multiple output formats
- Logger: Error logging with email notifications
- Production/development mode auto-detection
- AI agent support: automated browsers (navigator.webdriver) get markdown output via console.error/console.log

## Essential Commands

### Testing
```bash
# Run all tests - ALWAYS use php-cgi (html tests only run with php-cgi)
vendor/bin/tester tests -p php-cgi -s

# Run single test file
vendor/bin/tester tests/Tracy/Debugger.timer().phpt -p php-cgi -s

# Run tests in specific directory
vendor/bin/tester tests/Dumper/ -s
```

### Code Quality
```bash
# Run PHPStan static analysis (level 7)
composer run phpstan

# Lint Java
```

</details>
