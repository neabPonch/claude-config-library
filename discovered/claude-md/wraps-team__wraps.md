---
name: wraps-team__wraps
source: https://github.com/wraps-team/wraps/blob/da260aa2c6cb585e9fbe844204658db6237a75f5/CLAUDE.md
repo: wraps-team/wraps
kind: claude-md
stars: 46
last_pushed: 2026-06-14T12:38:19Z
license: other
score: 9
domains: [fullstack, infrastructure-as-code, security, frontend, cli-tools]
tags: [monorepo, typescript, aws, design-system, security-focused]
curated: 2026-06-15
curated_by: config-scout
---

# wraps-team/wraps — claude-md

**Why it's worth keeping:** The 'Banned Dependencies' and 'Security Patterns' sections provide high-signal guardrails that prevent common LLM errors. The use of 'Critical Design Principles' ensures architectural consistency across a complex monorepo.

**Summary:** A highly detailed project context that defines strict technical boundaries, security patterns, and a specific brand design language. It provides actionable constraints for an AI to follow during complex multi-step operations.

**Source credibility:** Highly credible; originates from an active, well-structured AWS infrastructure project.

**Recency:** Extremely current; uses cutting-edge technologies like React 19 and Tailwind 4.

**Source:** [wraps-team/wraps/CLAUDE.md](https://github.com/wraps-team/wraps/blob/da260aa2c6cb585e9fbe844204658db6237a75f5/CLAUDE.md) · 46★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Wraps Project Context

## Workflow

Before modifying any code, read all relevant files and understand the full execution flow first. Do not start making changes while still exploring the codebase. If the task is complex, use a Task agent to explore the codebase before writing any code.

## Error Handling

When implementing new features that involve external API calls (e.g., AWS SDK, Vercel API), always wrap each API call with specific error handling that distinguishes between different error types (e.g., NotFound vs CredentialsError vs PermissionDenied). Never use generic catch-all error messages.

When implementing multi-step features (e.g., create resource -> save state -> use resource), ensure each step's side effects are persisted before proceeding to the next step. Specifically: save all critical state (IDs, external references) immediately after creation, before any subsequent operations that might fail.

## Project Overview

**Wraps** is a CLI tool, web platform, and TypeScript SDK that deploys communication infrastructure (email via AWS SES, SMS via AWS End User Messaging, CDN via S3+CloudFront) to users' AWS accounts with zero stored credentials, beautiful de
```

</details>
