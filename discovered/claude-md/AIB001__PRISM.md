---
name: AIB001__PRISM
source: https://github.com/AIB001/PRISM/blob/d9eeb90aed279c5310c74392f7f6034595533b58/CLAUDE.md
repo: AIB001/PRISM
kind: claude-md
stars: 25
last_pushed: 2026-04-10T06:48:40Z
license: unknown
score: 9
domains: [scientific-computing, cli-tools, bioinformatics]
tags: [molecular-dynamics, strict-conventions, resource-management]
curated: 2026-06-15
curated_by: config-scout
---

# AIB001/PRISM — claude-md

**Why it's worth keeping:** Uses 'Correct vs Wrong' examples to enforce non-obvious architectural rules; includes specific machine-level constraints (CPU core counts) critical for scientific computing; leverages MCP tool selection guidance.

**Summary:** A highly detailed technical guide that provides specific instructions on tool usage, strict naming conventions, and hardware resource constraints for molecular dynamics automation.

**Source credibility:** Scientific research repository with moderate social proof and recent maintenance.

**Recency:** Very current; specifically references modern MCP LSP tools used in Claude Code environments.

**Source:** [AIB001/PRISM/CLAUDE.md](https://github.com/AIB001/PRISM/blob/d9eeb90aed279c5310c74392f7f6034595533b58/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

PRISM (Protein Receptor Interaction Simulation Modeler) is a comprehensive Python tool for building protein-ligand systems for molecular dynamics simulations in GROMACS. It supports multiple force fields including GAFF (via AmberTools) and OpenFF (Open Force Field).

**Documentation Repository**: `/home/gxf1212/data/work/PRISM-Tutorial` - Official documentation and tutorials for PRISM

## Code Search and Navigation

**📝 LSP Tools Preferred**: For code navigation, use LSP tools over grep when available:
- **LSP tools** (`mcp__cclsp__` series): Semantic understanding, direct symbol location
  - `mcp__cclsp__find_definition` - Find symbol definitions accurately
  - `mcp__cclsp__find_references` - Find all symbol references
  - `mcp__cclsp__find_workspace_symbols` - Search workspace symbols
  - Benefits: More accurate, skips comments/strings, reduces token usage
- **Grep**: Text search requiring human interpretation
- **Availability**: LSP tools available in Claude Code tool context only
- **Fallback**: Use `Grep` tool when LSP tools are unavailable
```

</details>
