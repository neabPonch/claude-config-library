---
name: eoko-dev__gideon
source: https://github.com/eoko-dev/gideon/blob/299535f123c6a31446e2f7061939ff96cc8c107f/CLAUDE.MD
repo: eoko-dev/gideon
kind: claude-md
stars: 27
last_pushed: 2026-05-25T20:09:43Z
license: mit
score: 8
domains: [agents-ai, discord-bots, backend]
tags: [architecture, state-management, database-schema]
curated: 2026-06-15
curated_by: config-scout
---

# eoko-dev/gideon — claude-md

**Why it's worth keeping:** The explicit breakdown of the BotStateManager and the hierarchical configuration (Global > Channel > Thread) provides essential logic context that prevents an agent from breaking override patterns. The Mermaid diagram and schema documentation allow for precise data-layer modifications without guesswork.

**Summary:** A high-density architectural blueprint detailing component relationships, complex state management hierarchies, and granular database schemas.

**Source credibility:** A niche but well-structured open-source project with recent activity.

**Recency:** Very current, referencing modern AI models (Sora 2 Pro, etc.) and up-to-date tech stacks.

**Source:** [eoko-dev/gideon/CLAUDE.MD](https://github.com/eoko-dev/gideon/blob/299535f123c6a31446e2f7061939ff96cc8c107f/CLAUDE.MD) · 27★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Gideon - AI Assistant for Discord

## Project Overview

Gideon is a sophisticated Discord bot that serves as an AI-powered assistant, providing intelligent conversations, image generation, video generation, trivia games, reminders, per-channel personas, and more. The bot integrates with multiple AI providers (OpenRouter, OpenAI, Anthropic Claude, Google Gemini), image generation services (AI Horde, Cloudflare Workers, DALL-E, ComfyUI, OpenRouter), and video generation via OpenRouter (Veo 3.1, Sora 2 Pro, Seedance, Wan, Kling, etc.).

**Tech Stack:**
- Python 3.8+
- Discord.py (Py-cord 2.4+)
- SQLite database
- Multiple AI provider APIs
- Docker support for deployment

## Architecture

### Architecture Diagram

```mermaid
graph TD
    A[Discord API] --> B(Bot Instance);
    B --> C(Event Handlers);
    B --> D(Command Dispatcher);
    D --> E(Cogs);
    E --> F(BotStateManager);
    F --> G(DatabaseManager);
    E --> H(API Clients);
    H --> I(External AI Services<br/>OpenRouter, OpenAI, AI Horde, Cloudflare);
    E --> J(Background Tasks<br/>Auto-save, Pruning);
    G --> K(SQLite Database);
    B --> L(Configuration<br/>.env, DB Config);
    L --> F;
    L --> H;
    E --> M(W
```

</details>
