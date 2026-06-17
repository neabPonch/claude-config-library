---
name: DevOpsAIguru123__claude-skills__code-documentation-skill
source: https://github.com/DevOpsAIguru123/claude-skills/blob/1449eae15d729b85192c230d1b9ee2959d73653d/code-documentation-skill.md
repo: DevOpsAIguru123/claude-skills
kind: skill
stars: 6
last_pushed: 2026-04-11T19:37:03Z
license: unknown
score: 7
domains: [documentation, software-architecture]
tags: [readme, api, adr, best-practices]
curated: 2026-06-16
curated_by: config-scout
---

# DevOpsAIguru123/claude-skills — skill

**Why it's worth keeping:** The distinction between 'Why vs What' in comments and the inclusion of ADR (Architecture Decision Record) formats offers high-value pattern guidance for an agent.

**Summary:** Provides comprehensive structural templates for READMEs, API documentation (JSDoc/OpenAPI), and architecture records.

**Source credibility:** Moderate; based on a small, organized repository.

**Recency:** Current; documentation standards are evergreen and highly stable.

**Source:** [DevOpsAIguru123/claude-skills/code-documentation-skill.md](https://github.com/DevOpsAIguru123/claude-skills/blob/1449eae15d729b85192c230d1b9ee2959d73653d/code-documentation-skill.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-documentation
description: Writing effective code documentation - API docs, README files, inline comments, and technical guides. Use for documenting codebases, APIs, or writing developer guides.
source: wshobson/agents
license: MIT
version: 4.1.0
---

# Code Documentation

## README Structure

### Standard README Template
```markdown
# Project Name

Brief description of what this project does.

## Quick Start

\`\`\`bash
npm install
npm run dev
\`\`\`

## Installation

Detailed installation instructions...

## Usage

\`\`\`typescript
import { something } from 'project';

// Example usage
const result = something.doThing();
\`\`\`

## API Reference

### `functionName(param: Type): ReturnType`

Description of what the function does.

**Parameters:**
- `param` - Description of parameter

**Returns:** Description of return value

**Example:**
\`\`\`typescript
const result = functionName('value');
\`\`\`

## Configuration

| Option | Type | Default | Description |
|--------|------|---------|-------------|
| `option1` | `string` | `'default'` | What it does |

## Contributing

How to contribute...

## License

MIT
```

## API Documentation

### JSDoc/TSDoc Style
```typescr
```

</details>
