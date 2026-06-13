# Workflows

Workflow practices describe *how* to work with Claude Code effectively — beyond individual CLAUDE.md settings or skills. These are patterns for getting consistent, high-quality results across a project.

## Structure

```
workflows/
├── practices/     # General practices applicable across most projects
├── patterns/      # Recurring patterns for specific scenarios
└── integrations/  # How Claude Code works with external tools (CI, GitHub, Linear, etc.)
```

## Categories

### Practices (`practices/`)

High-level approaches to common software tasks:

| File | What it covers |
|------|---------------|
| `code-review.md` | How to use Claude for PR review effectively |
| `tdd.md` | Test-driven development with Claude in the loop |
| `debugging.md` | Systematic debugging workflows |
| `refactoring.md` | Safe, incremental refactoring with Claude |
| `onboarding.md` | Using Claude to onboard new devs to a codebase |
| `documentation.md` | Keeping docs in sync with code changes |
| `incident-response.md` | Using Claude during production incidents |

### Patterns (`patterns/`)

Repeatable solutions to specific scenarios:

| File | What it covers |
|------|---------------|
| `migration.md` | Database and API migrations |
| `feature-flag.md` | Rolling out features safely |
| `dependency-upgrade.md` | Upgrading major dependencies |
| `performance-investigation.md` | Profiling and optimization workflow |
| `security-audit.md` | Pre-release security sweep |

### Integrations (`integrations/`)

How to wire Claude Code into your toolchain:

| File | What it covers |
|------|---------------|
| `github-actions.md` | Triggering Claude Code from CI |
| `linear.md` | Linking Claude work to Linear tickets |
| `slack.md` | Claude Code notifications and summaries |
| `vercel.md` | Deploy preview review workflow |

## Format

Each workflow file follows this structure:

```markdown
---
name: workflow-slug
description: one-line description
category: [practice, pattern, integration]
tags: [review, test, debug, deploy, document]
---

# Workflow: [Name]

## When to use this

[Describe the situation or trigger]

## Steps

1. ...
2. ...

## Claude prompts to use

[Specific prompts or skill invocations that work well here]

## Pitfalls

[Common mistakes or anti-patterns]
```
