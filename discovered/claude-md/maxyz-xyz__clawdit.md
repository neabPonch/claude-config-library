---
name: maxyz-xyz__clawdit
source: https://github.com/maxyz-xyz/clawdit/blob/9d808e95096cfa319e64f21f72dbde3648cf252a/CLAUDE.md
repo: maxyz-xyz/clawdit
kind: claude-md
stars: 2
last_pushed: 2026-03-06T08:48:21Z
license: other
score: 8
domains: [security, agents-ai, smart-contracts]
tags: [mcp, context-management, agent-orchestration, solidity]
curated: 2026-06-16
curated_by: config-scout
---

# maxyz-xyz/clawdit — claude-md

**Why it's worth keeping:** The three-tier progressive disclosure architecture (Tier 0/1/2) is an elite technique for managing context window limits in complex, data-heavy tasks. It also provides a rigorous pattern for integrating specialized MCP servers into agent workflows.

**Summary:** Establishes a high-sophistication agent skill framework using structured MCP servers and multi-tiered knowledge retrieval.

**Source credibility:** Low star count but demonstrates high technical complexity specific to the Solidity security domain.

**Recency:** Highly current; aligned with contemporary Claude Code plugin and MCP capabilities.

**Source:** [maxyz-xyz/clawdit/CLAUDE.md](https://github.com/maxyz-xyz/clawdit/blob/9d808e95096cfa319e64f21f72dbde3648cf252a/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# clawdit

A Claude Code plugin for professional-grade Solidity smart contract security auditing.

## Specifications

- **Agent Skills spec**: https://agentskills.io/specification.md
- **Claude Code skills docs**: https://code.claude.com/docs/en/skills.md
- **Claude Code plugins docs**: https://code.claude.com/docs/en/plugins.md

## Plugin Structure

```
.claude-plugin/
  plugin.json
agents/                    # Agent definition files for parallel audit
skills/
  audit/
    SKILL.md               # Main orchestrator
    references/            # Three-tier reference architecture
mcp-servers/
  solodit/                 # Solodit search MCP server
  static-analysis/         # Slither + Aderyn MCP server
```

## Script Paths

All paths in SKILL.md and agent files must use `${CLAUDE_PLUGIN_ROOT}`:

```bash
node ${CLAUDE_PLUGIN_ROOT}/mcp-servers/solodit/dist/index.js
```

## Validation

```bash
uvx --from "git+https://github.com/agentskills/agentskills.git#subdirectory=skills-ref" skills-ref validate skills/clawdit
```

## Linting

```bash
npx prettier --write "**/*.md"
```

## Conventions

- Reference docs use three-tier progressive disclosure (Tier 0: always loaded, Tier 1: per-protoco
```

</details>
