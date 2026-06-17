---
name: imxv__Pretty-mermaid-skills
source: https://github.com/imxv/Pretty-mermaid-skills/blob/e33f086d3b5bcec9f28632e4bd9c348b02bb2278/SKILL.md
repo: imxv/Pretty-mermaid-skills
kind: skill
stars: 756
last_pushed: 2026-01-31T11:21:26Z
license: mit
score: 8
domains: [cli-tools, documentation, visualization]
tags: [mermaid, diagrams, svg, ascii, rendering]
curated: 2026-06-14
curated_by: config-scout
---

# imxv/Pretty-mermaid-skills — skill

**Why it's worth keeping:** The 'Workflow Decision Tree' is an excellent pattern for guiding agents through multi-step visual tasks, and the specific CLI templates make execution foolproof.

**Summary:** Enables an agent to transform Mermaid text into professional SVG diagrams or terminal-friendly ASCII art using a dedicated CLI toolset.

**Source credibility:** Strong; 756 stars indicates a highly-regarded utility in the developer community.

**Recency:** Current; updated within the last 4 months, aligning with modern tool-use patterns.

**Source:** [imxv/Pretty-mermaid-skills/SKILL.md](https://github.com/imxv/Pretty-mermaid-skills/blob/e33f086d3b5bcec9f28632e4bd9c348b02bb2278/SKILL.md) · 756★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pretty-mermaid
description: |
  Render beautiful Mermaid diagrams as SVG or ASCII art using the beautiful-mermaid library.
  Supports 15+ themes, 5 diagram types (flowchart, sequence, state, class, ER), and ultra-fast rendering.

  Use this skill when:
  1. User asks to "render a mermaid diagram" or provides .mmd files
  2. User requests "create a flowchart/sequence diagram/state diagram"
  3. User wants to "apply a theme" or "beautify a diagram"
  4. User needs to "batch process multiple diagrams"
  5. User mentions "ASCII diagram" or "terminal-friendly diagram"
  6. User wants to visualize architecture, workflows, or data models
---

# Pretty Mermaid

Render stunning, professionally-styled Mermaid diagrams with one command. Supports SVG for web/docs and ASCII for terminals.

## Quick Start

### Render a Single Diagram

**From a file:**
```bash
node scripts/render.mjs \
  --input diagram.mmd \
  --output diagram.svg \
  --format svg \
  --theme tokyo-night
```

**From user-provided Mermaid code:**
1. Save the code to a `.mmd` file
2. Run the render script with desired theme

### Batch Render Multiple Diagrams

```bash
node scripts/batch.mjs \
  --input-dir ./diagrams \
```

</details>
