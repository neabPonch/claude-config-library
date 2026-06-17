---
name: anthropics__claude-code-action__claude
source: https://github.com/anthropics/claude-code-action/blob/3d9f0dc7dc27995e8d9ae6ec22f9fe72f3e5ab12/base-action/CLAUDE.md
repo: anthropics/claude-code-action
kind: claude-md
stars: 8011
last_pushed: 2026-06-14T05:49:35Z
license: mit
score: 7
domains: [cli-tools, github-actions, typescript]
tags: [bun, automation, github-action]
curated: 2026-06-15
curated_by: config-scout
---

# anthropics/claude-code-action — claude-md

**Why it's worth keeping:** Clearly maps specific build/test command patterns and explains provider authentication logic to prevent agent hallucination during task execution.

**Summary:** Provides essential development commands, architecture overview, and authentication patterns for a Bun-based GitHub Action.

**Source credibility:** High; from a highly-starred, actively maintained repository associated with the Claude ecosystem.

**Recency:** Current, utilizing modern runtimes like Bun.

**Source:** [anthropics/claude-code-action/base-action/CLAUDE.md](https://github.com/anthropics/claude-code-action/blob/3d9f0dc7dc27995e8d9ae6ec22f9fe72f3e5ab12/base-action/CLAUDE.md) · 8011★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Common Commands

### Development Commands

- Build/Type check: `bun run typecheck`
- Format code: `bun run format`
- Check formatting: `bun run format:check`
- Run tests: `bun test`
- Install dependencies: `bun install`

### Action Testing

- Test action locally: `./test-local.sh`
- Test specific file: `bun test test/prepare-prompt.test.ts`

## Architecture Overview

This is a GitHub Action that allows running Claude Code within GitHub workflows. The action consists of:

### Core Components

1. **Action Definition** (`action.yml`): Defines inputs, outputs, and the composite action steps
2. **Prompt Preparation** (`src/index.ts`): Runs Claude Code with specified arguments

### Key Design Patterns

- Uses Bun runtime for development and execution
- JSON streaming output format for execution logs
- Composite action pattern to orchestrate multiple steps
- Provider-agnostic design supporting Anthropic API, AWS Bedrock, and Google Vertex AI

## Provider Authentication

1. **Anthropic API** (default): Requires API key via `anthropic_api_key` input
2. **AWS Bedrock**: Uses OIDC authentication when `use_bedrock: true`
3. **Google Vertex AI**: Uses OIDC authentication when `u
```

</details>
