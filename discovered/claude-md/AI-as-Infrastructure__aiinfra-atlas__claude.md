---
name: AI-as-Infrastructure__aiinfra-atlas__claude
source: https://github.com/AI-as-Infrastructure/aiinfra-atlas/blob/85d78ad898bc96606b1208c3d208695c5a8cc208/.claude/CLAUDE.md
repo: AI-as-Infrastructure/aiinfra-atlas
kind: claude-md
stars: 6
last_pushed: 2026-06-11T23:18:02Z
license: other
score: 8
domains: [ai-research, rag-systems, backend-api]
tags: [spec-driven, troubleshooting-first, workflow-protocol]
curated: 2026-06-14
curated_by: config-scout
---

# AI-as-Infrastructure/aiinfra-atlas — claude-md

**Why it's worth keeping:** It includes high-value decision logic (when to propose vs. when to skip) and proactive debugging context for common infrastructure failures.

**Summary:** Establishes a formal 'OpenSpec' workflow for change management and provides detailed environmental troubleshooting guides.

**Source credibility:** Academic research project with consistent maintenance.

**Recency:** Highly current, featuring modern tech stacks and AI-driven development protocols.

**Source:** [AI-as-Infrastructure/aiinfra-atlas/.claude/CLAUDE.md](https://github.com/AI-as-Infrastructure/aiinfra-atlas/blob/85d78ad898bc96606b1208c3d208695c5a8cc208/.claude/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
> **Note**: This file provides project context, OpenSpec workflow, and setup information for Claude Code to help understand the ATLAS codebase, conventions, and common operations. This is the single source of truth for AI assistants working on this project.

# ATLAS - AI Infrastructure Research Platform

## OpenSpec Workflow

This project uses [OpenSpec](https://github.com/Fission-AI/OpenSpec) for spec-driven development. When planning significant changes:

### When to Create an OpenSpec Change Proposal

Create a proposal when you need to:
- Add features or functionality
- Make breaking changes (API, schema)
- Change architecture or patterns
- Optimize performance (changes behavior)
- Update security patterns

Skip proposals for:
- Bug fixes (restore intended behavior)
- Typos, formatting, comments
- Dependency updates (non-breaking)
- Configuration changes
- Tests for existing behavior

### Quick Workflow

1. **Search existing work**: `openspec list` and `openspec list --specs`
2. **Create proposal**: Choose unique `change-id` (kebab-case, verb-led: `add-`, `update-`, `remove-`)
3. **Scaffold**: Create `proposal.md`, `tasks.md`, and spec deltas under `openspec/changes/<id>/`
4. **
```

</details>
