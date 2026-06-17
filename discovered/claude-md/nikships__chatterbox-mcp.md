---
name: nikships__chatterbox-mcp
source: https://github.com/nikships/chatterbox-mcp/blob/2a58413bb30d068fa90ada8eda9c9a7c403cd1f2/claude.md
repo: nikships/chatterbox-mcp
kind: claude-md
stars: 0
last_pushed: 2026-01-16T20:38:33Z
license: unknown
score: 9
domains: [ai-agents, backend-api, audio-processing, mcp-servers]
tags: [tts, mcp, python, voice-cloning]
curated: 2026-06-14
curated_by: config-scout
---

# nikships/chatterbox-mcp — claude-md

**Why it's worth keeping:** The 'Code Patterns' section provides exact templates for extending functionality, while 'Key Design Decisions' prevents the AI from introducing blocking I/O issues.

**Summary:** A highly specialized instruction set that includes domain-specific syntax (emotion markers) and architectural boilerplate.

**Source credibility:** Likely a specialized individual developer; low social proof on GitHub but high-quality technical depth.

**Recency:** Current; reflects modern async patterns and MCP tool development.

**Source:** [nikships/chatterbox-mcp/claude.md](https://github.com/nikships/chatterbox-mcp/blob/2a58413bb30d068fa90ada8eda9c9a7c403cd1f2/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Chatterbox TTS MCP Server

FastMCP server for text-to-speech generation with voice cloning.

## Project Structure

```
chatterbox-mcp/
├── server.py              # Entry point (run this)
├── chatterbox_server/     # Main package
│   ├── __init__.py
│   ├── config.py          # Configuration (paths, ports, URLs)
│   ├── models.py          # Model loading, caching, pool management
│   ├── audio.py           # Audio processing utilities
│   ├── tts.py             # Core TTS generation logic
│   ├── voices.py          # Voice management (list, save, delete, youtube, transcripts)
│   ├── mcp_tools.py       # MCP tool definitions
│   ├── api.py             # REST API endpoints
│   └── server.py          # Server setup and startup
├── ui/                    # Web interface
├── voices/                # Voice reference files + voice_transcripts.json
├── checkpoints/           # Fish Speech model checkpoint
└── output/                # Generated audio files
```

## Hardware

- **GPU**: NVIDIA RTX 5090 (32GB VRAM)
- Handles 3+ concurrent model instances (~2GB each)

## Models

- `standard` - English, CFG/exaggeration controls, 500M params (Chatterbox)
- `turbo` - English, fast generation, p
```

</details>
