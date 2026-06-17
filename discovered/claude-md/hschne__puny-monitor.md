---
name: hschne__puny-monitor
source: https://github.com/hschne/puny-monitor/blob/626049d81396da315397fb786bf2dcf83a7a0eac/CLAUDE.md
repo: hschne/puny-monitor
kind: claude-md
stars: 102
last_pushed: 2025-10-17T08:44:41Z
license: mit
score: 8
domains: [backend, devops, monitoring]
tags: [ruby, sinatra, architecture-focused]
curated: 2026-06-14
curated_by: config-scout
---

# hschne/puny-monitor — claude-md

**Why it's worth keeping:** The Architecture section links components (Scheduler, SystemUtils) to high-level design patterns, which helps the AI understand system side effects. It also explicitly documents critical environment variable dependencies for Dockerized execution.

**Summary:** Provides a deep architectural mental model alongside specific development and deployment workflows.

**Source credibility:** Solid reputation for a niche utility with 102 stars.

**Recency:** Highly relevant; follows modern containerized development standards.

**Source:** [hschne/puny-monitor/CLAUDE.md](https://github.com/hschne/puny-monitor/blob/626049d81396da315397fb786bf2dcf83a7a0eac/CLAUDE.md) · 102★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Puny Monitor is a batteries-included monitoring tool for single hosts, designed specifically for Kamal deployments and containerized setups. It's a Ruby gem built with Sinatra that provides system monitoring through a web interface.

## Development Commands

### Setup
```bash
bin/setup              # Install dependencies
```

### Testing & Quality
```bash
rake test              # Run all tests with Minitest
rake standard          # Run StandardRB linter
rake default           # Run both tests and linter
```

### Development Server
```bash
bundle exec rackup     # Start development server (default port 9292)
puny-monitor           # Start the server on port 4567
bin/console            # Interactive Ruby console
```

### Docker Development
```bash
rake docker:build     # Build Docker image
rake docker:run       # Run container locally
rake docker:shell     # Interactive shell in container
```

### Assets
```bash
rake assets           # Copy Chartkick JavaScript assets to public/
```

## Architecture

### Core Components

**Sinatra App** (`app/puny_
```

</details>
