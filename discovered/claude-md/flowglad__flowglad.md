---
name: flowglad__flowglad
source: https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/claude.md
repo: flowglad/flowglad
kind: claude-md
stars: 1716
last_pushed: 2026-05-17T18:12:00Z
license: other
score: 9
domains: [fullstack, backend-api, devops]
tags: [bun, drizzle-orm, testing-patterns, ast-grep, operational-rules]
curated: 2026-06-15
curated_by: config-scout
---

# flowglad/flowglad — claude-md

**Why it's worth keeping:** Provides exact code patterns for tool usage (Bun Shell API), leverages semantic search instructions via ast-grep, and includes a sophisticated testing doctrine that prevents race conditions/mocking errors.

**Summary:** A highly opinionated instruction set that defines strict operational boundaries for package management, database migrations, and testing protocols. It uses specific 'negative constraints' to prevent AI-driven errors like manual migration creation or incorrect search methods.

**Source credibility:** High; comes from a popular, actively maintained open-source project with over 1.7k stars.

**Recency:** Very current; utilizes modern toolchains like Bun, Drizzle ORM, and ast-grep.

**Source:** [flowglad/flowglad/claude.md](https://github.com/flowglad/flowglad/blob/aad66f18960bab4ca5f9f261ce26cd50b023283f/claude.md) · 1716★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Package Manager
**IMPORTANT**: This project uses `bun` as its package manager. ALWAYS use `bun` for all package management operations. Never use `npm` or `yarn`.

Examples:
- Install dependencies: `bun install`
- Add a package: `bun add <package-name>`
- Run scripts: `bun run <script-name>`
- Build: `bun run build`

## Related Files

- `AGENTS.md` - High-level overview and code quality standards
- `.cursor/rules/` - File-specific patterns for AI assistance
- `platform/flowglad-next/llm-prompts/` - Reusable prompt templates for common workflows
- `.agents/` - AI context (gameplans, research, troubleshooting guides)

## Init
Run the following command EVERY TIME you are in a new context:
```bash
bun run init:flowglad-next
```

**Note:** This requires two environment variables to be set:
- `FLOWGLAD_VERCEL_PROJECT_ID` - The Vercel project ID
- `FLOWGLAD_VERCEL_ORG_ID` - The Vercel organization ID
- `FLOWGLAD_LOCAL_USER` - Your local username for env var prefixing (e.g., BROOKS)

## Resources

### ast-grep

You run in an environment where `ast-grep` is available; whenever a search requires syntax-aware or structural matching, default to `ast-grep --lang <language> -p '<pattern>'` (e.
```

</details>
