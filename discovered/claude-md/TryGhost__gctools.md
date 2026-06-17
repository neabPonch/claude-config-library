---
name: TryGhost__gctools
source: https://github.com/TryGhost/gctools/blob/e5e5df7bad0272d7fcdca74064fcaa08ff07627d/CLAUDE.md
repo: TryGhost/gctools
kind: claude-md
stars: 50
last_pushed: 2026-06-15T03:34:38Z
license: mit
score: 9
domains: [cli-tools, backend-api, node.js]
tags: [architectural-patterns, extension-guide, ghost-cms]
curated: 2026-06-15
curated_by: config-scout
---

# TryGhost/gctools — claude-md

**Why it's worth keeping:** Includes high-quality boilerplate and pattern examples for API interactions and task orchestration that ensure structural consistency when adding new features.

**Summary:** Provides a rigorous architectural framework for extending the CLI tool via specific layers: business logic (tasks), command definitions, and interactive prompts.

**Source credibility:** Moderate star count for a niche utility; maintenance is very recent and active.

**Recency:** Uses modern ESM syntax and async/await patterns consistent with current Node.js standards.

**Source:** [TryGhost/gctools/CLAUDE.md](https://github.com/TryGhost/gctools/blob/e5e5df7bad0272d7fcdca74064fcaa08ff07627d/CLAUDE.md) · 50★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# gctools - Ghost Content Tools

CLI utilities for working with Ghost CMS content via the Admin API.

**Use `yarn` (not npm) for running scripts and installing dependencies.**

## Architecture Overview

```
gctools/
├── bin/cli.js          # Entry point - registers all commands with prettyCLI
├── commands/           # CLI command definitions (flags, options, run function)
├── tasks/              # Core business logic (API calls, data processing)
├── prompts/            # Interactive mode definitions (inquirer prompts)
├── lib/                # Shared utilities
└── test/               # Jest tests
```

## Adding a New Feature

To add a new command, create/modify these files:

### 1. `tasks/<feature>.js` - Business Logic

```javascript
import GhostAdminAPI from '@tryghost/admin-api';
import {makeTaskRunner} from '@tryghost/listr-smart-renderer';
import {discover} from '../lib/batch-ghost-discover.js';

const initialise = (options) => ({
    title: 'Initialising API connection',
    task: (ctx, task) => {
        ctx.api = new GhostAdminAPI({
            url: options.apiURL.replace('localhost', '127.0.0.1'),
            key: options.adminAPIKey,
            version: 'v5.0'
        });
```

</details>
