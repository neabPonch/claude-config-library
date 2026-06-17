---
name: brs077__3dp-mcp-server
source: https://github.com/brs077/3dp-mcp-server/blob/960e8de46fc52b82939bc43619cb16a7d4897374/CLAUDE.MD
repo: brs077/3dp-mcp-server
kind: claude-md
stars: 6
last_pushed: 2026-03-18T18:08:23Z
license: other
score: 9
domains: [mcp-servers, cad-engineering, python, cli-tools]
tags: [build123d, 3d-printing, mcp, engineering]
curated: 2026-06-16
curated_by: config-scout
---

# brs077/3dp-mcp-server — claude-md

**Why it's worth keeping:** It provides essential syntax examples for the underlying library (build123d) and crucial manufacturing heuristics (wall thickness, tolerances) that prevent the AI from generating invalid 3D models.

**Summary:** A highly detailed technical specification that covers project structure, development workflows, and deep domain-specific coding patterns.

**Source credibility:** A specialized engineering tool with active recent maintenance.

**Recency:** Very recent; reflects modern MCP and build123d development standards.

**Source:** [brs077/3dp-mcp-server/CLAUDE.MD](https://github.com/brs077/3dp-mcp-server/blob/960e8de46fc52b82939bc43619cb16a7d4897374/CLAUDE.MD) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 3DP MCP Server

MCP server for 3D-printable CAD modeling with build123d, targeting STL export for Bambu Lab X1C 3D printing.

## Project Structure

```
src/threedp_mcp/
├── server.py       # Thin entrypoint — FastMCP init, tool registration, main()
├── constants.py    # MATERIAL_PROPERTIES, ISO_THREAD_TABLE
├── helpers.py      # shape_to_model_entry, run_build123d_code, select_face, compute_overhangs, ensure_exported
└── tools/
    ├── __init__.py     # register_all_tools(mcp, models, output_dir)
    ├── core.py         # create_model, export_model, measure_model, analyze_printability, list_models, get_model_code
    ├── transform.py    # transform_model, combine_models, import_model
    ├── modification.py # shell_model, split_model, add_text, create_threaded_hole
    ├── analysis.py     # estimate_print, analyze_overhangs, suggest_orientation, section_view, export_drawing, split_model_by_color
    ├── utility.py      # shrinkage_compensation, pack_models, convert_format
    ├── components.py   # create_enclosure, create_gear, create_snap_fit, create_hinge, create_dovetail, generate_label
    ├── mechanical.py   # create_thread, create_fastener, create_bearing, create_sprocket,
```

</details>
