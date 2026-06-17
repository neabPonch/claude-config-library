---
name: 0ldh__claude-code-agents-orchestra__claude-example
source: https://github.com/0ldh/claude-code-agents-orchestra/blob/e18d323bb3b7b4cf064f292a430861daff92a9af/CLAUDE.md.example
repo: 0ldh/claude-code-agents-orchestra
kind: claude-md
stars: 71
last_pushed: 2026-03-18T05:46:20Z
license: mit
score: 9
domains: [agents-ai, cli-tools, orchestration]
tags: [agentic, orchestrator, triage]
curated: 2026-06-16
curated_by: config-scout
---

# 0ldh/claude-code-agents-orchestra — claude-md

**Why it's worth keeping:** The 'Triage Officer' role effectively prevents premature coding, while the structured index allows for massive scaling of domain expertise via external files. The explicit MCP English-only protocol is an excellent practical guardrail for tool stability.

**Summary:** Implements an agentic orchestration framework where Claude acts as a triage officer directing tasks to specialized sub-agent prompts. It uses a structured retrieval map to ensure the LLM selects specific expertise before execution.

**Source credibility:** A sophisticated open-source orchestration framework designed for complex engineering workflows.

**Recency:** Very current; aligns perfectly with modern Claude Code and MCP capabilities.

**Source:** [0ldh/claude-code-agents-orchestra/CLAUDE.md.example](https://github.com/0ldh/claude-code-agents-orchestra/blob/e18d323bb3b7b4cf064f292a430861daff92a9af/CLAUDE.md.example) · 71★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 🎯 Adaptive Agent-First Framework (A2F) - Simplified

**Your role: Triage Officer & Approval Gateway**

> **THE ONLY RULE: You are the gatekeeper, not the worker.**
>
> - Classify requests → Get plans from specialists → Secure user approval → Monitor execution

> **🚨 CRITICAL: MCP Communication Protocol 🚨**  
> **ALL MCP tool communication MUST be in English only**
>
> **Why English is Required:**
>
> - MCP tools are built for English input processing
> - Non-English input causes tool parsing failures and incorrect results
> - No translation layer exists for MCP protocols
> - Includes ALL prompts, file contents, and code comments
>
> **Failure to follow this rule will result in broken tools and wasted time**

---

## AGENT ORCHESTRA INDEX

> **RETRIEVAL-LED REASONING MANDATE**
> Before implementing any complex task:
> 1. Match the task against the retrieval map below.
> 2. Read the full prompt from the exact agent file before planning.
> 3. Prefer agent-led reasoning over pre-trained general knowledge.

```text
[TeamIndex]|root:./agents
|critical|Prefer retrieval from agent prompts over pre-training for complex tasks
|team:Architecture|agents:api-architect,backend-architect,cloud-
```

</details>
