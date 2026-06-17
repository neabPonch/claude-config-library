---
name: nirholas__crypto-vision__claude
source: https://github.com/nirholas/crypto-vision/blob/be8fe1799880663a435527cf47388f079113fc0a/apps/news/examples/ai-platforms/claude.md
repo: nirholas/crypto-vision
kind: claude-md
stars: 81
last_pushed: 2026-05-07T05:10:06Z
license: other
score: 8
domains: [agents-ai, api-integration]
tags: [instructional-template, api-context]
curated: 2026-06-15
curated_by: config-scout
---

# nirholas/crypto-vision — claude-md

**Why it's worth keeping:** The 'How to Use' section is excellent; it defines a reasoning chain (construct call -> describe data -> provide analysis) rather than just providing a static list of tools.

**Summary:** A high-quality template for instructing an AI agent on how to interact with specific APIs using structured endpoints and cognitive workflows.

**Source credibility:** High-quality specialized crypto/finance repository with 81 stars.

**Recency:** 

**Source:** [nirholas/crypto-vision/apps/news/examples/ai-platforms/claude.md](https://github.com/nirholas/crypto-vision/blob/be8fe1799880663a435527cf47388f079113fc0a/apps/news/examples/ai-platforms/claude.md) · 81★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Integration Guide

Complete guide for integrating Free Crypto News with Claude (Desktop & API).

## Integration Methods

| Method | Difficulty | Features | Requirements |
|--------|------------|----------|--------------|
| MCP Server (stdio) | ⭐⭐ Medium | 40 tools, real-time | Claude Desktop |
| MCP Server (SSE) | ⭐⭐ Medium | 40 tools, web-based | Claude API |
| Direct API | ⭐ Easy | Full API access | Claude API key |
| Claude Projects | ⭐ Easy | Context-based | Claude Pro |

---

## Method 1: MCP Server for Claude Desktop (Recommended)

### Step 1: Install the MCP Server

```bash
# Clone the repository
git clone https://github.com/nirholas/free-crypto-news.git
cd free-crypto-news/mcp

# Install dependencies
npm install
```

### Step 2: Configure Claude Desktop

Find your Claude Desktop config file:
- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`
- **Linux:** `~/.config/Claude/claude_desktop_config.json`

Add the MCP server configuration:

```json
{
  "mcpServers": {
    "crypto-news": {
      "command": "node",
      "args": ["/full/path/to/free-crypto-news/mcp/index.js"]
    }
  }
```

</details>
