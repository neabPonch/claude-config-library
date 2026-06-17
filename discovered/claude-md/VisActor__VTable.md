---
name: VisActor__VTable
source: https://github.com/VisActor/VTable/blob/dbb2ba6e465579b8c2e88012fcb5fb0f5133b866/CLAUDE.md
repo: VisActor/VTable
kind: claude-md
stars: 3594
last_pushed: 2026-06-16T12:34:03Z
license: mit
score: 8
domains: [web-frontend, data-visualization, monorepo]
tags: [typescript, canvas, architecture, rush-monorepo]
curated: 2026-06-16
curated_by: config-scout
---

# VisActor/VTable — claude-md

**Why it's worth keeping:** It goes beyond 'how to run' by providing the 'how it works' through rendering pipeline explanations and specific class-level implementation details which guide AI reasoning.

**Summary:** Provides comprehensive context for a complex Rush monorepo, covering command workflows, package dependencies, and deep architectural mental models.

**Source credibility:** High; comes from a highly starred (3.5k+) active data visualization library.

**Recency:** Very recent; includes current development branch specifics and modern Node versions.

**Source:** [VisActor/VTable/CLAUDE.md](https://github.com/VisActor/VTable/blob/dbb2ba6e465579b8c2e88012fcb5fb0f5133b866/CLAUDE.md) · 3594★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

VTable is a high-performance multidimensional data analysis table component built on the VRender canvas engine. This is a Rush monorepo containing the core VTable library and related packages.

## Essential Commands

### Development Setup
```bash
# Install dependencies (required first time and after package.json changes)
rush update

# Build all packages
rush build

# Start development server for core vtable package
cd packages/vtable && rushx demo

# Start documentation site
rush docs

# Run tests
rush test

# Run linting
rush eslint

# Fix dependency issues
rush purge && rush update
```

### Working with Individual Packages
```bash
# Build specific package
cd packages/[package-name] && rushx build

# Run tests for specific package
cd packages/[package-name] && rushx test

# Start demo for specific package
cd packages/[package-name] && rushx demo
```

### Git Workflow
```bash
# After making changes, update changelogs before committing
rush change-all

# Commit with conventional message format
git commit -m "type: description"
```

## Architectur
```

</details>
