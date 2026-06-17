---
name: soloterm__dumps
source: https://github.com/soloterm/dumps/blob/829ad564381d8eca34b381c0032656bd7e2a60c6/CLAUDE.md
repo: soloterm/dumps
kind: claude-md
stars: 126
last_pushed: 2026-03-16T16:57:58Z
license: mit
score: 8
domains: [php, laravel, cli-tools]
tags: [architecture-diagrams, testing-guidance, backend]
curated: 2026-06-16
curated_by: config-scout
---

# soloterm/dumps — claude-md

**Why it's worth keeping:** The ASCII data flow diagram is a high-value technique for providing LLMs with a mental model of system logic. It also documents specific fallback behaviors that prevent runtime errors during development.

**Summary:** Provides essential CLI commands and a clear architectural overview of how dumps are intercepted via a TCP server.

**Source credibility:** A niche utility package with moderate GitHub star counts.

**Recency:** Very current; updated within the last 3 months.

**Source:** [soloterm/dumps/CLAUDE.md](https://github.com/soloterm/dumps/blob/829ad564381d8eca34b381c0032656bd7e2a60c6/CLAUDE.md) · 126★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Solo Dumps is a Laravel package that intercepts `dump()` calls and redirects them to a dedicated terminal window via a TCP server. This keeps browser/API responses clean while centralizing debug output.

## Commands

```bash
# Run all tests
./vendor/bin/phpunit

# Run specific test suite
./vendor/bin/phpunit --testsuite=unit
./vendor/bin/phpunit --testsuite=integration

# Run single test
./vendor/bin/phpunit --filter testMethodName

# Start the dump server (for manual testing)
php vendor/bin/testbench solo:dumps
```

## Architecture

### Data Flow

```text
dump() call in app
    ↓
CustomDumper (VarDumper handler)
    ↓ resolves source file/line
    ↓ clones var with dumpSource context
ServerDumper → TCP socket (127.0.0.1:9984)
    ↓
DumpServer in `solo:dumps` command
    ↓ extracts dumpSource from context
CliDumper → terminal output with source info
```

### Key Components

- **CustomDumper** (`src/Support/CustomDumper.php`): Registers a custom VarDumper handler that:
  - Resolves dump source (file:line) before sending
  - Checks if dump server port is o
```

</details>
