---
name: Significant-Gravitas__AutoGPT__claude
source: https://github.com/Significant-Gravitas/AutoGPT/blob/ba178a734f47ab85e42da8a76b755ca8cc611665/classic/forge/CLAUDE.md
repo: Significant-Gravitas/AutoGPT
kind: claude-md
stars: 184945
last_pushed: 2026-06-15T05:40:10Z
license: other
score: 9
domains: [agents-ai, backend-api, python]
tags: [architecture, agentic-framework, protocols, composition]
curated: 2026-06-15
curated_by: config-scout
---

# Significant-Gravitas/AutoGPT — claude-md

**Why it's worth keeping:** It uses 'Must Override' sections to define class contracts and detail specific protocols/logic (like topological sorting) that prevent AI from hallucinating component interactions.

**Summary:** This file serves as a high-level architectural blueprint that explains not just how to run the code, but how the internal object models interact.

**Source credibility:** Extremely high; AutoGPT is a leading-edge, highly-starred repository in the AI agent space.

**Recency:** Very current; uses modern Python type hinting and reflects contemporary LLM integration patterns.

**Source:** [Significant-Gravitas/AutoGPT/classic/forge/CLAUDE.md](https://github.com/Significant-Gravitas/AutoGPT/blob/ba178a734f47ab85e42da8a76b755ca8cc611665/classic/forge/CLAUDE.md) · 184945★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Quick Reference

All commands run from the `classic/` directory (parent of this directory):

```bash
# Run forge agent server (port 8000)
poetry run python -m forge

# Run forge tests
poetry run pytest forge/tests/
poetry run pytest forge/tests/ --cov=forge
poetry run pytest -k test_name
```

## Entry Point

`__main__.py` → loads `.env` → configures logging → starts Uvicorn with hot-reload on port 8000

The app is created in `app.py`:
```python
agent = ForgeAgent(database=database, workspace=workspace)
app = agent.get_agent_app()
```

## Directory Structure

```
forge/
├── __main__.py               # Entry: uvicorn server startup
├── app.py                    # FastAPI app creation
├── agent/                    # Core agent framework
│   ├── base.py               # BaseAgent abstract class
│   ├── forge_agent.py        # Reference implementation
│   ├── components.py         # AgentComponent base classes
│   └── protocols.py          # Protocol interfaces
├── agent_protocol/           # Agent Protocol standard
│   ├── agent.py              # ProtocolAgent mixin
│
```

</details>
