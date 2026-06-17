---
name: logicalclocks__rondb
source: https://github.com/logicalclocks/rondb/blob/f136cc623b7bf7bf09a0f457282027ea0fe8c251/CLAUDE.md
repo: logicalclocks/rondb
kind: claude-md
stars: 710
last_pushed: 2026-06-12T06:57:16Z
license: other
score: 9
domains: [cli-tools, systems-programming, database]
tags: [go, cpp, architecture, design-philosophy]
curated: 2026-06-14
curated_by: config-scout
---

# logicalclocks/rondb — claude-md

**Why it's worth keeping:** Includes a 'Design Philosophy' section that instructs the agent on how to write code (e.g., 'Fail loud with context'), which is a rare but essential pattern for maintaining project standards.

**Summary:** Provides comprehensive build and testing instructions for both a Go CLI and a C++ core engine. It includes high-value architectural maps and command flow descriptions.

**Source credibility:** Highly credible; part of a high-star, actively maintained professional database repository.

**Recency:** Current; uses modern build toolchains and provides specific instructions highly useful for current agentic workflows.

**Source:** [logicalclocks/rondb/CLAUDE.md](https://github.com/logicalclocks/rondb/blob/f136cc623b7bf7bf09a0f457282027ea0fe8c251/CLAUDE.md) · 710★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

RonDB is a distribution of NDB Cluster (MySQL's distributed key-value store with SQL capabilities). This repository contains:
1. **RonDB Core** - C++ codebase (MySQL/NDB Cluster fork)
2. **rondb-cli** - Go CLI tool at `/tools/rondb-cli/` for unified Rondis + SQL access

The unique value proposition: Write data with Rondis (Redis protocol), query it with SQL, same data store.

## Build Commands

### rondb-cli (Go tool)
```bash
cd tools/rondb-cli
go build -o rondb .
```

### RonDB Core (C++ - requires CMake)
```bash
cmake -DWITH_NDB=1 -DWITH_RDRS=1 -DWITH_NDB_TEST=1 -DWITH_UNIT_TESTS=1 \
      -DWITH_SSL=$OPENSSL_ROOT -DWITH_ROUTER=0 .
make -j$(nproc)
```

Key CMake flags:
- `-DWITH_NDB=1` - NDB storage engine
- `-DWITH_RDRS=1` - REST server + Rondis support
- `-DWITH_NDB_TEST=1` - NDB test suite

## Testing

### MySQL Test Suite
```bash
cd mysql-test
./mysql-test-run.pl [test_name]       # Run specific test
./mysql-test-run.pl --record test     # Record new baseline
./mysql-test-run.pl ndb_*             # NDB-specific tests
./mysql-test-run --exte
```

</details>
