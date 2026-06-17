---
name: mondoohq__cnspec__skill
source: https://github.com/mondoohq/cnspec/blob/c0162642772df07282372eb804db08bd4b9d0dfb/skills/mql/SKILL.md
repo: mondoohq/cnspec
kind: skill
stars: 429
last_pushed: 2026-06-15T13:31:18Z
license: other
score: 9
domains: [security, cli-tools, devops]
tags: [mql, schema-discovery, query-language]
curated: 2026-06-15
curated_by: config-scout
---

# mondoohq/cnspec — skill

**Why it's worth keeping:** It includes a 'Schema Discovery' workflow that teaches the agent exactly which CLI commands to run to find fields/resources, preventing hallucinations of schema details.

**Summary:** Provides highly structured instructions for writing, validating, and exploring MQL queries using the cnspec CLI or MCP tools.

**Source credibility:** High; comes from an established security platform (Mondoo) with active maintenance.

**Recency:** Very current; utilizes modern MCP tool-calling patterns and command-line validation techniques.

**Source:** [mondoohq/cnspec/skills/mql/SKILL.md](https://github.com/mondoohq/cnspec/blob/c0162642772df07282372eb804db08bd4b9d0dfb/skills/mql/SKILL.md) · 429★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: mql
description: Use when writing MQL (Mondoo Query Language) queries, working with Mondoo MCP tools, or developing security policies
---

# MQL Development Skill

## Overview

This skill provides guidance for writing MQL (Mondoo Query Language) queries and validating them using either the cnspec CLI or Mondoo's MCP tools.

**Two-tier knowledge system:**
- **Reference Files** (static): MQL syntax docs, platform-specific examples
- **Schema Tools** (live): Real-time schema lookup and query validation via cnspec CLI or MCP

## When to Use

- Writing MQL queries or policies
- Validating MQL syntax before deployment
- Exploring available MQL resources and fields
- Platform-specific query development (AWS, Azure, Linux, Windows, Microsoft 365)

## Reference Materials

Located within this skill directory:

| File | Purpose |
|------|---------|
| [mql-reference.md](mql-reference.md) | Complete MQL syntax and patterns |
| [samples/general.md](samples/general.md) | General MQL patterns |
| [samples/aws.md](samples/aws.md) | AWS resource patterns |
| [samples/azure.md](samples/azure.md) | Azure resource patterns |
| [samples/linux.md](samples/linux.md) | Linux system patterns |
| [
```

</details>
