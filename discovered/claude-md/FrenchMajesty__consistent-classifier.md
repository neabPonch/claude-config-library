---
name: FrenchMajesty__consistent-classifier
source: https://github.com/FrenchMajesty/consistent-classifier/blob/adcd2e406d645d1f18cec40b7ca4014e248f51e9/CLAUDE.md
repo: FrenchMajesty/consistent-classifier
kind: claude-md
stars: 64
last_pushed: 2025-11-01T18:51:04Z
license: mit
score: 9
domains: [backend, ai-infrastructure, cli-tools]
tags: [go, llm-orchestration, vector-search, concurrency]
curated: 2026-06-15
curated_by: config-scout
---

# FrenchMajesty/consistent-classifier — claude-md

**Why it's worth keeping:** Includes explicit file-and-line mappings to guide the agent through complex logic and documents critical concurrency/shutdown side effects.

**Summary:** Detailed documentation of the core classification data flow, specifically distinguishing between fast cache hits and slow miss paths.

**Source credibility:** High-quality technical documentation for a specialized Go package.

**Recency:** Extremely relevant; uses modern context-aware patterns helpful for agentic tools like Claude Code.

**Source:** [FrenchMajesty/consistent-classifier/CLAUDE.md](https://github.com/FrenchMajesty/consistent-classifier/blob/adcd2e406d645d1f18cec40b7ca4014e248f51e9/CLAUDE.md) · 64★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

`consistent-classifier` is a Go package for LLM-powered text classification with vector caching and label clustering. It uses:
- **Voyage AI** for text embeddings
- **Pinecone** for vector similarity search
- **OpenAI-compatible LLMs** for classification
- **Disjoint Set Union (DSU)** for clustering semantically similar labels

## Common Commands

### Testing
```bash
# Run all tests
go test ./...

# Run tests with coverage
go test -cover ./...

# Run specific package tests
go test ./adapters/...
go test ./internal/disjoint_set/...

# Generate coverage report
go test -coverprofile=coverage.out ./...
go tool cover -html=coverage.out
```

### Building
```bash
# Build the benchmark tool
go build -o consistent-classifier ./cmd/benchmark

# Run benchmark with LLM-only classification
./consistent-classifier --classify=llm --limit=100

# Run benchmark with vector caching + clustering
./consistent-classifier --classify=vectorize --limit=100

# Quick smoke test
./consistent-classifier --classify=vectorize --smoke-test
```

### Development
```bash
# Install depende
```

</details>
