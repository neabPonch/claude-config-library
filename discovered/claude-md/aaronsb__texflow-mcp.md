---
name: aaronsb__texflow-mcp
source: https://github.com/aaronsb/texflow-mcp/blob/ff6ebb69471008d9f4fcf55587bd7fab74aec3ff/CLAUDE.md
repo: aaronsb/texflow-mcp
kind: claude-md
stars: 22
last_pushed: 2026-03-05T05:14:50Z
license: mit
score: 8
domains: [mcp, cli-tools, python]
tags: [mcp, latex, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# aaronsb/texflow-mcp — claude-md

**Why it's worth keeping:** The 'Key Design Decisions' section provides essential behavioral constraints (e.g., treating the Document model as the source of truth) which prevents AI-driven state corruption. The inclusion of a clear architectural tree and tool definitions enables highly reliable navigation for an agent.

**Summary:** Defines a LaTeX compiler that uses an intermediate structured model rather than direct TeX manipulation to handle document construction.

**Source credibility:** Recent, niche project with active maintenance.

**Recency:** Current; uses modern Python tooling like uv.

**Source:** [aaronsb/texflow-mcp/CLAUDE.md](https://github.com/aaronsb/texflow-mcp/blob/ff6ebb69471008d9f4fcf55587bd7fab74aec3ff/CLAUDE.md) · 22★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TeXFlow MCP Server

## Project Overview

TeXFlow is a LaTeX document compiler with an MCP interface. The AI operates on a structured document model (sections, paragraphs, figures, tables) and the server handles all LaTeX mechanics — packages, preamble, compilation.

**Two entry flows:**
1. **Scaffold**: `document(action="create")` → empty document skeleton → AI builds content via `edit` tool
2. **Markdown ingest**: `document(action="ingest", source="file.md")` → populated model → AI refines layout

Both converge on an in-memory `Document` model that auto-saves to disk. LaTeX is only ever an output artifact.

## Architecture

```
server.py                          # FastMCP entry point, 5 tool registrations
texflow/
  model.py                         # Document model dataclasses
  serializer.py                    # Model → .tex generation
  ingestion.py                     # Markdown → model (mistune AST)
  compiler.py                      # .tex → PDF (xelatex subprocess)
  tools/
    state.py                       # Shared session state, auto-save
    document.py                    # create, ingest, outline, read
    layout.py                      # configure typesetting
    edi
```

</details>
