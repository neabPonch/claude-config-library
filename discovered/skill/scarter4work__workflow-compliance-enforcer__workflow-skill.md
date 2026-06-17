---
name: scarter4work__workflow-compliance-enforcer__workflow-skill
source: https://github.com/scarter4work/workflow-compliance-enforcer/blob/1b3d410e433b7c59588c55e315e6cd011dc42323/WORKFLOW_SKILL.md
repo: scarter4work/workflow-compliance-enforcer
kind: skill
stars: 0
last_pushed: 2026-01-03T19:53:19Z
license: mit
score: 9
domains: [cli-tools, devops, workflow-automation]
tags: [mcp, state-machine, compliance, reliability]
curated: 2026-06-14
curated_by: config-scout
---

# scarter4work/workflow-compliance-enforcer — skill

**Why it's worth keeping:** Uses 'Scenario/Correct Response' blocks and 'Anti-Patterns' to prevent tool-bypassing; includes a clear State Machine reference for error recovery.

**Summary:** Provides highly structured instructions for an agent to follow a strictly enforced state-machine workflow using MCP tools.

**Source credibility:** Low social proof (0 stars), but the technical structure is professionally architected for agentic reliability.

**Recency:** Highly current; specifically leverages the MCP/Claude Code paradigm.

**Source:** [scarter4work/workflow-compliance-enforcer/WORKFLOW_SKILL.md](https://github.com/scarter4work/workflow-compliance-enforcer/blob/1b3d410e433b7c59588c55e315e6cd011dc42323/WORKFLOW_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Workflow Best Practices

## Overview
This skill provides context and examples for the enforced development workflow. 
The workflow is **physically enforced** by the `workflow-enforcer` MCP server.

## The Mandatory Workflow

You MUST follow this exact sequence:

1. **Start Issue** → `workflow_start_issue`
2. **Write Code** → Use normal file tools
3. **Run Tests** → `workflow_run_tests`
4. **Commit** → `workflow_commit` (only after tests pass)
5. **Deploy** → `workflow_deploy`
6. **Verify Production** → `workflow_verify_prod`
7. **Close Issue** → `workflow_close_issue`

## Why This Workflow Exists

### Why Start with an Issue?
- Ensures all work is tracked
- Provides context for code reviewers
- Links commits to requirements
- Enables better project management

### Why Run Tests Before Commit?
- Prevents broken code from entering the repository
- Catches regressions early
- Maintains code quality standards
- Saves time debugging later

### Why Verify in Production?
- Integration tests don't catch everything
- Real-world data behaves differently
- Network, latency, and scaling issues appear in prod
- Confirms the actual problem is solved

## Common Scenarios

### Scenario 1: Tests
```

</details>
