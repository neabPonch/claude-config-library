---
name: snowplow__snowplow-lake-loader
source: https://github.com/snowplow/snowplow-lake-loader/blob/4aaab880a7a511473edcfe8a5e93fc476312f4c1/CLAUDE.md
repo: snowplow/snowplow-lake-loader
kind: claude-md
stars: 5
last_pushed: 2026-02-02T09:02:14Z
license: other
score: 8
domains: [data-engineering, backend]
tags: [scala, sbt, spark, multi-module]
curated: 2026-06-16
curated_by: config-scout
---

# snowplow/snowplow-lake-loader — claude-md

**Why it's worth keeping:** The architectural breakdown explains module boundaries and dependencies, while the specific SBT command sets enable precise tool usage for an AI agent.

**Summary:** Provides a comprehensive technical map of a complex multi-module Scala/Spark project including build, test, and deployment commands.

**Source credibility:** High; written by Snowplow, a reputable data engineering organization.

**Recency:** Very current; updated within the last 4 months.

**Source:** [snowplow/snowplow-lake-loader/CLAUDE.md](https://github.com/snowplow/snowplow-lake-loader/blob/4aaab880a7a511473edcfe8a5e93fc476312f4c1/CLAUDE.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Snowplow Lake Loader is a Scala application that loads Snowplow enriched events into open table formats (Delta, Iceberg) on cloud storage. It supports Azure (Event Hubs → ADLS Gen2), GCP (Pubsub → GCS), and AWS (Kinesis → S3) platforms.

## Common Commands

### Building and Testing
```bash
# Run tests
sbt test

# Check Scala formatting
sbt scalafmtCheckAll scalafmtSbtCheck

# Format Scala code
sbt scalafmtAll scalafmtSbt

# Compile all modules
sbt compile

# Run a specific test class
sbt "testOnly *ProcessingSpec"

# Run tests for specific module
sbt "project core" test
```

### Docker Operations
```bash
# Build Docker image for AWS
sbt "project aws" docker:publishLocal

# Build Docker image for Azure
sbt "project azure" docker:publishLocal

# Stage Docker build
sbt "project gcp" docker:stage
```

### Module-Specific Commands
```bash
# Work with specific cloud modules
sbt "project aws" <command>
sbt "project azure" <command>
sbt "project gcp" <command>
```

## Architecture

### Multi-Module Structure
- **Core Module** (`modules/core/`): Shared pr
```

</details>
