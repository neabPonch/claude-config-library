---
name: pactflow__pactflow-agent-skills__pactflow-skill
source: https://github.com/pactflow/pactflow-agent-skills/blob/a023485752f1978ccc26fd366b868ba33325f886/docs/ai-tools/pactflow-skill.md
repo: pactflow/pactflow-agent-skills
kind: skill
stars: 3
last_pushed: 2026-06-15T04:28:51Z
license: mit
score: 8
domains: [api-testing, devops, contract-testing, agent-orchestration]
tags: [mcp, cli-tools, tiered-capability, pactflow]
curated: 2026-06-16
curated_by: config-scout
---

# pactflow/pactflow-agent-skills — skill

**Why it's worth keeping:** It utilizes a sophisticated 'Capability Tiering' pattern (Knowledge → Shell/CLI → MCP), which provides a template for teaching agents to recognize their own tool limitations based on the environment.

**Summary:** A blueprint for tiered agentic capabilities that scales from pure domain knowledge to CLI execution and full MCP integration.

**Source credibility:** High; authored by PactFlow, an industry-standard specialist in contract testing.

**Recency:** Highly current; leverages modern agentic standards like MCP and CLI-tool orchestration.

**Source:** [pactflow/pactflow-agent-skills/docs/ai-tools/pactflow-skill.md](https://github.com/pactflow/pactflow-agent-skills/blob/a023485752f1978ccc26fd366b868ba33325f886/docs/ai-tools/pactflow-skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PactFlow AI Assistant Skill

The **PactFlow skill** turns your AI coding assistant into a Pact and PactFlow contract testing expert. It provides deep knowledge of consumer test patterns, provider verification configuration, can-i-deploy diagnostics, and full workspace management — surfaced directly in your editor without leaving your flow.

It ships as part of the [`swagger-contract-testing`](https://github.com/pactflow/pactflow-agent-skills) plugin alongside two companion skills:

- **Drift** ☁ (Spec-based API conformance testing tool, PactFlow Cloud only — [docs](https://pactflow.github.io/drift-docs/))
- **OpenAPI Parser** (spec analysis).

:::tip Works with open-source Pact Broker and PactFlow Cloud
The skill and MCP server work with both the open-source Pact Broker and PactFlow Cloud. Features marked ☁ require a PactFlow Cloud account. All other capabilities work with Pact and any Pact Broker.
PactFlow-specific capabilities include: Drift testing, AI test generation and review, bi-directional contract testing, team metrics, the audit log, and all administration tools.
:::

---

## Skill vs Pact CLI vs Full Plugin

There are three levels of capability depending on what is ins
```

</details>
