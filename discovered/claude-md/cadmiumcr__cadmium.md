---
name: cadmiumcr__cadmium
source: https://github.com/cadmiumcr/cadmium/blob/94e3be502c9464e93559adef2aad2fc9131d6756/CLAUDE.md
repo: cadmiumcr/cadmium
kind: claude-md
stars: 211
last_pushed: 2026-01-05T05:58:29Z
license: mit
score: 9
domains: [cli-tools, nlp, monorepo]
tags: [git-submodules, crystal-lang, justfile, dependency-management]
curated: 2026-06-15
curated_by: config-scout
---

# cadmiumcr/cadmium — claude-md

**Why it's worth keeping:** It includes high-value technical 'gotchas' like required environment variable overrides and an explicit internal dependency graph to prevent breaking changes across shards.

**Summary:** Provides detailed operational intelligence for managing a complex Crystal monorepo using git submodules and the 'just' command runner.

**Source credibility:** The repository is active with a respectable star count, indicating it is a real-world project rather than a placeholder.

**Recency:** 

**Source:** [cadmiumcr/cadmium/CLAUDE.md](https://github.com/cadmiumcr/cadmium/blob/94e3be502c9464e93559adef2aad2fc9131d6756/CLAUDE.md) · 211★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Cadmium** is a Natural Language Processing (NLP) library for Crystal, organized as a monorepo using git submodules. Each NLP component is a separate shard with its own git repository, versioning, and release cycle.

## Development Setup

### Initial Setup
```bash
git clone --recursive git@github.com:cadmiumcr/cadmium.git
cd cadmium
SHARDS_OVERRIDE=shard.dev.yml shards install
```

**Critical:** Always use `SHARDS_OVERRIDE=shard.dev.yml` when running `shards install` for development. This uses local path dependencies instead of GitHub dependencies.

### If Already Cloned Without --recursive
```bash
git submodule update --init --recursive
SHARDS_OVERRIDE=shard.dev.yml shards install
```

## Common Commands (via justfile)

Install [just](https://github.com/casey/just) if needed. Run `just` to see all commands.

### Development
```bash
just install              # Install dependencies (uses shard.dev.yml)
just update-submodules    # Update all submodules to latest
just submodule-status     # Check submodule status
```

### Testing
```bash
just test
```

</details>
