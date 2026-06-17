---
name: lightdash__lightdash__claude
source: https://github.com/lightdash/lightdash/blob/a433067d14799b2c3229569ff7ed19f30321923f/packages/cli/src/handlers/CLAUDE.md
repo: lightdash/lightdash
kind: claude-md
stars: 5898
last_pushed: 2026-06-16T15:02:17Z
license: other
score: 9
domains: [cli-tools, typescript]
tags: [structured-instructions, semantic-tagging]
curated: 2026-06-16
curated_by: config-scout
---

# lightdash/lightdash — claude-md

**Why it's worth keeping:** Uses explicit step-by-step procedural workflows and 'importantToKnow' blocks to prevent agent hallucination regarding auth flows and project context.

**Summary:** Provides highly structured, semantic module documentation including execution patterns and critical business logic dependencies.

**Source credibility:** High: popular repository (5.8k stars) with very recent activity.

**Recency:** Current; maintains modern TypeScript and path alias conventions.

**Source:** [lightdash/lightdash/packages/cli/src/handlers/CLAUDE.md](https://github.com/lightdash/lightdash/blob/a433067d14799b2c3229569ff7ed19f30321923f/packages/cli/src/handlers/CLAUDE.md) · 5898★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLI Handlers Module

<summary>
Command handlers for the Lightdash CLI that execute core operations like authentication, compilation, deployment, and project management. Each handler implements the business logic for a specific CLI command and provides user feedback through the terminal interface.
</summary>

<howToUse>
Handlers are called by the main CLI framework (Commander.js) when users execute commands. Each handler follows a consistent pattern:

1. Parse and validate command options
2. Set up global state (verbose logging, analytics)
3. Execute the core operation
4. Provide user feedback and handle errors

Most handlers require authentication and project context. The compile/deploy workflow is the most common usage pattern.
</howToUse>

<codeExample>
```typescript
// Compile dbt models and validate explores
import { compile, CompileHandlerOptions } from './compile';

const options: CompileHandlerOptions = {
projectDir: './dbt-project',
profilesDir: './profiles',
target: 'dev',
verbose: true,
skipWarehouseCatalog: false
};

const explores = await compile(options);
console.info(`Compiled ${explores.length} explores`);

// Deploy to Lightdash instance
import { deployHandler } f
```

</details>
