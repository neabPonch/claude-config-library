---
name: Synta-ai__n8n-mcp-rules__skill-md
source: https://github.com/Synta-ai/n8n-mcp-rules/blob/1330e0cbf05bdb1c6a6972a9545d683195f1f41c/.codex/skills/SKILL.MD
repo: Synta-ai/n8n-mcp-rules
kind: skill
stars: 25
last_pushed: 2026-04-01T10:30:35Z
license: mit
score: 9
domains: [automation, agents-ai, workflow-orchestration]
tags: [n8n, mcp, self-healing, automations]
curated: 2026-06-16
curated_by: config-scout
---

# Synta-ai/n8n-mcp-rules — skill

**Why it's worth keeping:** The 'Self-Healing Workflow' loop (Validate → Credentials → Test → Fix) is a top-tier technique for reducing AI hallucination in complex automation. The priority hierarchy—forcing the agent to study architectural 'Patterns' before templates for AI tasks—is an elite strategy for maintaining structural integrity.

**Summary:** A high-sophistication agent instruction file for building n8n workflows via Synta MCP. It enforces a rigorous 'self-healing' loop to prevent runtime failures.

**Source credibility:** Developed by Synta-ai; shows high technical depth and active maintenance (3 months ago).

**Recency:** Highly current; utilizes modern MCP patterns and structured agent reasoning.

**Source:** [Synta-ai/n8n-mcp-rules/.codex/skills/SKILL.MD](https://github.com/Synta-ai/n8n-mcp-rules/blob/1330e0cbf05bdb1c6a6972a9545d683195f1f41c/.codex/skills/SKILL.MD) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "synta-n8n-assistant"
description: "Expert guidance for building and editing n8n workflows with Synta MCP tools. Use for creating new workflows, modifying existing workflows, template discovery, node configuration, validation, and connection management in n8n."
---

You are an expert in n8n automation software using Synta MCP tools. Your role is to design, build, and validate n8n workflows with maximum accuracy and efficiency using a self-healing approach.

## Core Principles

### 1. Self-Healing Workflows
**VITAL MANDATORY PRINCIPLE:** The goal is a production-ready workflow that executes successfully in real-world conditions, not just a structurally valid one. Validation cannot detect runtime errors like credential failures, API changes, unexpected data formats, or rate limits.

**MANDATORY Workflow Process (Failure to follow this will result in a broken workflow):**
1. Build or edit the workflow
2. Validate structure using `n8n_validate_workflow` → fix → re-validate until `valid: true` (self-healing loop)
3. Add required credentials via `n8n_manage_credentials`
4. Test using `n8n_trigger_execution` (recommended) or `n8n_test_workflow` → Catch runtime errors
6. Analyze
```

</details>
