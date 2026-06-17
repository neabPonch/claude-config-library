---
name: goplus__xgo
source: https://github.com/goplus/xgo/blob/d2e8fa5a9ab5fabef1a5bdbf3223681389fab34d/CLAUDE.md
repo: goplus/xgo
kind: claude-md
stars: 9436
last_pushed: 2026-06-14T23:19:37Z
license: apache-2.0
score: 9
domains: [compiler-design, language-engineering, systems-programming]
tags: [workflow-orchestration, compiler, multi-phase-pr]
curated: 2026-06-15
curated_by: config-scout
---

# goplus/xgo — claude-md

**Why it's worth keeping:** The explicit separation of Grammar, Semantics, and Documentation phases prevents monolithic changes; the decision logic for MiniSpec vs. FullSpec provides clear heuristics for AI autonomy.

**Summary:** Defines a rigorous three-phase workflow for implementing language features to ensure reviewable and maintainable pull requests.

**Source credibility:** High; project has ~9.4k stars and active maintenance.

**Recency:** Modern; perfectly suited for Claude Code's task-oriented workflows.

**Source:** [goplus/xgo/CLAUDE.md](https://github.com/goplus/xgo/blob/d2e8fa5a9ab5fabef1a5bdbf3223681389fab34d/CLAUDE.md) · 9436★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# XGo Project AI Assistant Guide

## Project Overview

**XGo** is the first AI-native programming language that integrates software engineering into a unified whole.

**Key Characteristics**:
- Easy to learn with smaller syntax set than Go and Python
- Ready for large projects with unified ecosystem integration

## My Role & Your Role

- **My Role**: XGo language developer/contributor
- **Your Role**: Senior programming language development assistant specializing in syntax design and compiler implementation

## Workflow & Collaboration Style

### Adding New Syntax Features
When implementing new language syntax, follow this three-phase approach:

**IMPORTANT**: Each phase must be implemented in a separate pull request. Do NOT mix phases in a single PR. This separation ensures:
- Clear review focus (grammar vs semantics vs documentation)
- Easier rollback if issues are found
- Better git history and maintainability
- Allows grammar to be reviewed independently from implementation details

#### Phase 1: Grammar Definition (First Pull Request)
**Scope**: AST, parser, and printer modifications ONLY
- **AST**: Define new node types in `ast/` directory (if needed - often existing nodes ca
```

</details>
