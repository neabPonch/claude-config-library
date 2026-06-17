---
name: ktheory__dalli-elasticache
source: https://github.com/ktheory/dalli-elasticache/blob/e6ce2fe95422aadab901c187c89ef40f77df7f05/CLAUDE.md
repo: ktheory/dalli-elasticache
kind: claude-md
stars: 128
last_pushed: 2026-02-27T22:00:48Z
license: mit
score: 9
domains: [backend, ruby, infrastructure]
tags: [architecture-flow, technical-nuance]
curated: 2026-06-15
curated_by: config-scout
---

# ktheory/dalli-elasticache — claude-md

**Why it's worth keeping:** It includes vital warnings about name-shadowing (e.g., the need for ::Socket) and explains the exact step-by-step logic of network operations.

**Summary:** Provides a detailed technical map of discovery flows, module hierarchies, and critical implementation nuances.

**Source credibility:** Solid; a specialized niche gem with recent maintenance activity.

**Recency:** Very current, targeting Ruby 3.3.

**Source:** [ktheory/dalli-elasticache/CLAUDE.md](https://github.com/ktheory/dalli-elasticache/blob/e6ce2fe95422aadab901c187c89ef40f77df7f05/CLAUDE.md) · 128★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
bundle exec rake          # Run all tests (default task)
bundle exec rspec         # Run all specs
bundle exec rspec spec/config_response_spec.rb  # Run a single spec file
bundle exec rubocop       # Lint
bundle exec rubocop -a    # Lint with auto-fix
```

## Architecture

This gem connects [Dalli](https://github.com/petergoldstein/dalli) (a Ruby memcached client) to AWS ElastiCache / Google Cloud MemoryStore auto-discovery endpoints. Given a cluster configuration endpoint, it queries that endpoint over TCP to discover all cache nodes, then provides server addresses to Dalli.

### Module structure

All classes live under `Dalli::Elasticache::AutoDiscovery` (note: `Elasticache` module uses lowercase 'c', while the top-level `ElastiCache` class uses uppercase 'C').

**Entry point:** `Dalli::ElastiCache` (`lib/dalli/elasticache.rb`) — accepts a config endpoint + Dalli options + optional `timeout:`, delegates to `Endpoint` for discovery, and exposes `#client`, `#servers`, `#version`, `#engine_version`, `#refresh`.

**Discovery flow:**
1. `Endpoint` p
```

</details>
