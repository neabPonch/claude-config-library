---
name: receptron__mulmocast-cli
source: https://github.com/receptron/mulmocast-cli/blob/3918c7694332200bef752610e890fcfa9d750612/CLAUDE.md
repo: receptron/mulmocast-cli
kind: claude-md
stars: 460
last_pushed: 2026-06-12T21:09:47Z
license: unknown
score: 9
domains: [cli-tools, ai-agents, media-processing]
tags: [typescript, architecture-patterns, workflow-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# receptron/mulmocast-cli — claude-md

**Why it's worth keeping:** The 'Methods Pattern' instruction prevents logic duplication by telling the AI exactly how to extend schema-specific functions, while the requirement for 'Implementation Plans' ensures complex changes are premeditated.

**Summary:** Provides deep architectural context including a strict 'Methods Pattern' for data processing and mandatory implementation plan workflows. It covers everything from specialized CLI commands to high-stakes publishing instructions.

**Source credibility:** High; a popular repository (460 stars) with very recent maintenance activity.

**Recency:** Current; highly compatible with Claude Code's ability to follow structured architectural patterns and tool-use workflows.

**Source:** [receptron/mulmocast-cli/CLAUDE.md](https://github.com/receptron/mulmocast-cli/blob/3918c7694332200bef752610e890fcfa9d750612/CLAUDE.md) · 460★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MulmoCast is an AI-native multi-modal presentation platform that transforms content into videos, podcasts, PDFs, and other formats. The core workflow involves creating MulmoScript (JSON-based content descriptions) and using GraphAI to orchestrate various AI agents for content generation.

## Development Commands

### Build & Development
```bash
yarn build                    # Compile TypeScript to lib/ directory
yarn build_test              # Build and checkout lib/ files to prevent accidental commits
yarn lint                    # Run ESLint on src/ and test/
yarn format                  # Format code with Prettier
yarn ci_test                 # Run Node.js native test runner
```

### Core CLI Commands
```bash
yarn cli                     # Run the CLI directly with npx tsx
yarn test                    # Run end-to-end test (generates test files)

# Content generation shortcuts
yarn audio <script>          # Generate audio from MulmoScript
yarn images <script>         # Generate images from MulmoScript  
yarn movie <script>          # Generate c
```

</details>
