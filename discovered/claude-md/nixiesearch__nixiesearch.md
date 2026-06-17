---
name: nixiesearch__nixiesearch
source: https://github.com/nixiesearch/nixiesearch/blob/31bc0a853a3d5f8421861201af4118834a584a27/CLAUDE.md
repo: nixiesearch/nixiesearch
kind: claude-md
stars: 613
last_pushed: 2026-01-06T14:42:55Z
license: apache-2.0
score: 9
domains: [backend, search-engine, scala, distributed-systems]
tags: [sbt, lucene, architecture-patterns, scaling]
curated: 2026-06-16
curated_by: config-scout
---

# nixiesearch/nixiesearch — claude-md

**Why it's worth keeping:** Includes specific code patterns (Resource management and Error handling) and actionable 'Common Gotchas' that prevent domain-specific errors like Lucene concurrency issues.

**Summary:** Provides deep technical context for a Scala/Lucene search engine, covering build commands, application modes, and architectural principles.

**Source credibility:** Strong niche project with 600+ stars and high technical density.

**Recency:** Highly current; uses modern Scala 3 standards and contemporary deployment patterns.

**Source:** [nixiesearch/nixiesearch/CLAUDE.md](https://github.com/nixiesearch/nixiesearch/blob/31bc0a853a3d5f8421861201af4118834a584a27/CLAUDE.md) · 613★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Nixiesearch is a modern S3-based search engine built with Scala 3 and Apache Lucene. It provides hybrid search (lexical + semantic), AI-powered features (embeddings, LLM inference), and operates with stateless compute nodes backed by S3 storage.

## Build System & Commands

**Build Tool**: SBT with Scala 3.7.1

### Core Commands
```bash
# Run all tests
sbt test

# Build fat JAR
sbt assembly

# Build Docker images (with multi-arch support)
sbt dockerBuildAndPush

# Run specific test
sbt "testOnly *TestClassName*"

# Run tests by category
sbt "testOnly -- -n HttpTest"
sbt "testOnly -- -n SlowTest"
```

### Docker Development
```bash
# Build and run standalone mode
docker run -itp 8080:8080 -v .:/data nixiesearch/nixiesearch:latest standalone -c /data/config.yml

# GPU variant available
docker run nixiesearch/nixiesearch:latest-gpu
```

### Test Categories
Tests are tagged with ScalaTest categories:
- `HttpTest` - API integration tests
- `SlowTest` - Long-running tests
- Use these for selective test execution

## Architecture

### Core Design Princi
```

</details>
