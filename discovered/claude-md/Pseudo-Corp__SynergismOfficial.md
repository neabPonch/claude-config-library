---
name: Pseudo-Corp__SynergismOfficial
source: https://github.com/Pseudo-Corp/SynergismOfficial/blob/1f25d10780c5f341a54a0dde5c3f326c42eac854/claude.md
repo: Pseudo-Corp/SynergismOfficial
kind: claude-md
stars: 369
last_pushed: 2026-06-15T22:36:04Z
license: mit
score: 8
domains: [web-frontend, game-development, typescript]
tags: [state-management, performance-optimization, platform-gating]
curated: 2026-06-16
curated_by: config-scout
---

# Pseudo-Corp/SynergismOfficial — claude-md

**Why it's worth keeping:** Demonstrates how to use 'permission-based' instructions for high-risk state changes and provides exact code patterns for performance optimizations and environment branching.

**Summary:** Provides strict architectural guardrails for an idle game, specifically focusing on state mutation risks and platform-specific logic.

**Source credibility:** High; the repository is a well-starred, active project with highly specific technical requirements.

**Recency:** Current; utilizes modern TypeScript practices and agentic workflow instructions.

**Source:** [Pseudo-Corp/SynergismOfficial/claude.md](https://github.com/Pseudo-Corp/SynergismOfficial/blob/1f25d10780c5f341a54a0dde5c3f326c42eac854/claude.md) · 369★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Synergism Project Context for Claude

## Project Overview
- **Name**: Synergism (idle game)
- **Tech Stack**: TypeScript, HTML, CSS
- **URL**: https://synergism.cc
- **Repository**: Primarily for frontend features of Synergism
- **Backend**: Connected via `src/login.ts` with mocking in `src/mock/`

## Agent Role & Workflow
### Primary Tasks
- Implement frontend features
- Fix bugs and issues
- Architect new feature systems

### Required Actions
1. **Always ask permission** before adding variables to `player` object (affects savefile size)
2. **Check back with user** after writing significant code
3. **Ask questions** when task requirements are unclear

## File Structure Rules
```
src/                       # Core game logic
index.html
Synergism.css
translations/en.json       # Required for all new text strings
```

## Development Patterns

### String Internationalization
- i18next: Add all user-facing text to `translations/en.json`
- **Styling**: `<<color|{{text}}>>` for colored text

### Save System Variables
**CRITICAL**: Before adding to `player` object:
1. Get explicit permission from user
2. Add to `src/types/Synergism.ts`
3. Add to `src/saves/PlayerSchema.ts`
4. Variable lo
```

</details>
