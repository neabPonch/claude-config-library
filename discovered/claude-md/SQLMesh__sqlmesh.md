---
name: SQLMesh__sqlmesh
source: https://github.com/SQLMesh/sqlmesh/blob/b44fdf65be66b207186e779df278f7113d480270/CLAUDE.md
repo: SQLMesh/sqlmesh
kind: claude-md
stars: 3139
last_pushed: 2026-06-13T18:48:31Z
license: apache-2.0
score: 9
domains: [data-engineering, cli-tools, ai-agents]
tags: [multi-agent-workflow, test-optimization, architectural-mapping]
curated: 2026-06-15
curated_by: config-scout
---

# SQLMesh/sqlmesh — claude-md

**Why it's worth keeping:** The mandatory developer-reviewer cycle enforces higher code quality; the differentiation between 'fast' and 'slow' test commands optimizes agent efficiency.

**Summary:** Establishes a formal multi-agent workflow (developer, reviewer, writer) and provides a comprehensive command catalog categorized by task type.

**Source credibility:** Highly credible source with 3k+ stars and active maintenance.

**Recency:** Extremely current, specifically optimized for agentic tool-use workflows like Claude Code.

**Source:** [SQLMesh/sqlmesh/CLAUDE.md](https://github.com/SQLMesh/sqlmesh/blob/b44fdf65be66b207186e779df278f7113d480270/CLAUDE.md) · 3139★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Agent-Based Development Workflow

Every time the user requests a feature or bug fix, you MUST follow the process below:

### Development Process

1. **Understanding The Task**: Use the `developer` agent to understand what the user is asking for and to read GitHub issues
2. **Feature Development & Bug Fixes**: Use the `developer` agent for implementing features and fixing bugs. IMPORTANT: Always begin by writing a failing test (or tests) that reflects the expected behavior
3. **Code Review**: After development work, invoke the `code-reviewer` agent to review the implementation
4. **Iteration**: Use the `developer` agent again to address feedback from the code reviewer
5. **Repeat**: Continue the developer → code-reviewer cycle until no more feedback remains
6. **Documentation**: If the feature or bug fix requires documentation updates, invoke the `technical-writer` agent

IMPORTANT: Make sure to share the project overview, architecture overview, and other concepts outlined below with the agent when it is invoked.

### Agent Responsibilities

**Developer Agent**:
-
```

</details>
