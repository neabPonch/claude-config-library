---
name: mbcrawfo__HackathonManager
source: https://github.com/mbcrawfo/HackathonManager/blob/282ee43ad1da66d39a5bf3a05ab9d8031e238739/CLAUDE.md
repo: mbcrawfo/HackathonManager
kind: claude-md
stars: 2
last_pushed: 2026-06-10T03:32:15Z
license: mit
score: 9
domains: [backend-api, web-frontend, devops]
tags: [dotnet, react, typescript, sql]
curated: 2026-06-16
curated_by: config-scout
---

# mbcrawfo/HackathonManager — claude-md

**Why it's worth keeping:** Includes essential 'gotchas' like specialized path mappings for Dockerized tools and a prescriptive 'final validation' workflow (npm run verify). The pattern of linking language-specific style rules directly to exact command-line verification tools is excellent.

**Summary:** Provides deep architectural context and precise command-line workflows for a multi-stack project. It defines strict coding standards coupled with specific linting, formatting, and verification commands.

**Source credibility:** High-quality technical documentation in an active, modern repository despite low star count.

**Recency:** Very current, referencing .NET 9 and modern development workflows.

**Source:** [mbcrawfo/HackathonManager/CLAUDE.md](https://github.com/mbcrawfo/HackathonManager/blob/282ee43ad1da66d39a5bf3a05ab9d8031e238739/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# HackathonManager Overview

This project is a web application that organizations can use to manage hackathons within their org.

## Project Structure

```
/<project-root>
    /.github -  Github CI configuration.  Do not modify unless explicitly instructed to do so.
    /docker -  Dockerfiles and supporting configuration.
    /docs
        /database -  Database schema documentation.  It is automatically generated, do not modify.
    /scripts -  Helper scripts for developer workflows and CI usage.
    /src
        /hackathon-spa -  The front end React SPA application.
        /HackathonManager -  The back end .Net REST API.
        /HackathonManager.Migrator -  Database migration application.
    /tests
        /e2e -  Playwright E2E tests (npm workspace).  Has its own compose.yml for running against the full Dockerized stack.
        /HackathonManager.Tests -  .Net test project for the back end including database tests, unit tests, and integration tests.
```

The .Net projects make use of `Directory.Build.props` for standardized settings, global package management in `Directory.Packages.props`, and lock files to produce frozen dependency trees.

A node.js package.json is configured
```

</details>
