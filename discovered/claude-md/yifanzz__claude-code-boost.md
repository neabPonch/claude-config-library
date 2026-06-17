---
name: yifanzz__claude-code-boost
source: https://github.com/yifanzz/claude-code-boost/blob/0cf9a5ebc3eb065e6c03475160aedc1f138e1e45/CLAUDE.md
repo: yifanzz/claude-code-boost
kind: claude-md
stars: 165
last_pushed: 2026-03-21T15:51:55Z
license: mit
score: 9
domains: [cli-tools, agents-ai, typescript]
tags: [cli, automation, development-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# yifanzz/claude-code-boost — claude-md

**Why it's worth keeping:** It demonstrates how to organize exhaustive command lists for all lifecycle stages (build, test, release) and provides deep technical context on security philosophy and logic flow.

**Summary:** A highly structured documentation file that outlines the architecture, development workflows, and configuration of a CLI tool designed to enhance Claude Code.

**Source credibility:** High; the project has significant community interest with 165 stars and recent activity.

**Recency:** Very current, updated within the last few months to reflect modern workflows.

**Source:** [yifanzz/claude-code-boost/CLAUDE.md](https://github.com/yifanzz/claude-code-boost/blob/0cf9a5ebc3eb065e6c03475160aedc1f138e1e45/CLAUDE.md) · 165★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Claude Code Boost is a TypeScript-based CLI tool that provides intelligent auto-approval hooks for Claude Code. It enhances developer productivity by automatically approving safe development operations while blocking genuinely destructive commands.

## Architecture

The project follows a simple CLI architecture:

- **Entry Point**: `src/index.ts` - Uses Commander.js for CLI structure
- **Main Command**: `src/commands/auto-approve-tools.ts` - Core logic for tool approval decisions
- **Hook Integration**: Processes Claude Code PreToolUse hooks via stdin/stdout JSON communication  
- **AI-Powered Decisions**: Falls back to Claude API for complex approval decisions
- **Type Safety**: `src/types/hook-schemas.ts` - Zod schemas for input/output validation
- **Security Model**: Two-tier approval system:
  - Fast approval for unambiguously safe tools (Read, LS, Glob, etc.)
  - AI-powered analysis for complex operations using `prompts/system-prompt.md`

## Development Commands

### Build and Test
```bash
npm run build          # TypeScript compilation to d
```

</details>
