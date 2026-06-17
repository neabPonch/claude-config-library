---
name: swagger-api__swagger-js
source: https://github.com/swagger-api/swagger-js/blob/df27b424b0aa86c1638a9ca0c286aadd2c1061ad/CLAUDE.md
repo: swagger-api/swagger-js
kind: claude-md
stars: 2691
last_pushed: 2026-06-10T06:00:40Z
license: apache-2.0
score: 9
domains: [javascript, api-tools, open-api]
tags: [build-system, testing-strategy, git-conventions, directory-map]
curated: 2026-06-15
curated_by: config-scout
---

# swagger-api/swagger-js — claude-md

**Why it's worth keeping:** The explicit mapping of functional logic to the repository tree and the specific documentation of multi-target build configurations (UMD/CJS/ESM) are exceptionally useful for AI agents.

**Summary:** A highly detailed guide that maps complex architecture to directory structure and provides strict workflow rules for building, testing, and committing code.

**Source credibility:** High; belongs to a mature, widely used open-source project with recent maintenance.

**Recency:** Current; references modern Node.js versions and contemporary development workflows.

**Source:** [swagger-api/swagger-js/CLAUDE.md](https://github.com/swagger-api/swagger-js/blob/df27b424b0aa86c1638a9ca0c286aadd2c1061ad/CLAUDE.md) · 2691★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - AI Assistant Guide for swagger-js

This document provides comprehensive guidance for AI assistants working on the swagger-js (swagger-client) codebase.

## Project Overview

**swagger-js** (npm package: `swagger-client`) is a JavaScript module that allows you to fetch, resolve, and interact with Swagger/OpenAPI documents. It supports:
- OpenAPI 3.2.0 (latest)
- OpenAPI 3.1.0
- OpenAPI 3.0.x (3.0.0 through 3.0.4)
- Swagger/OpenAPI 2.0
- Legacy Swagger 1.x (via version 2.x branch)

**Current Version**: 3.36.0

The library is used by Swagger-UI and other tools in the OpenAPI ecosystem to parse, resolve references, and execute operations defined in OpenAPI specifications.

## Repository Structure

```
swagger-js/
├── src/                    # Source code (ES6+ modules)
│   ├── execute/           # Request execution logic for OAS operations
│   │   ├── oas3/         # OpenAPI 3.x execution
│   │   └── swagger2/     # Swagger 2.0 execution
│   ├── helpers/          # Utility functions and helpers
│   ├── http/             # HTTP client implementation
│   │   └── serializers/  # Request/response serialization
│   ├── resolver/         # Spec resolution and $ref handling
│
```

</details>
