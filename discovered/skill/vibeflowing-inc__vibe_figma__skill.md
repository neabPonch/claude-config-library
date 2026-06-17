---
name: vibeflowing-inc__vibe_figma__skill
source: https://github.com/vibeflowing-inc/vibe_figma/blob/f250b8ad6946184b93b8029097a2be3051182cee/skills/vibefigma/SKILL.md
repo: vibeflowing-inc/vibe_figma
kind: skill
stars: 549
last_pushed: 2026-05-26T17:32:35Z
license: agpl-3.0
score: 8
domains: [web-frontend, cli-tools, design-to-code]
tags: [figma, react, tailwind, automation]
curated: 2026-06-16
curated_by: config-scout
---

# vibeflowing-inc/vibe_figma — skill

**Why it's worth keeping:** The 'Workflow' section provides excellent procedural logic for an agent, including how to handle file existence checks, overwrite confirmations, and specific error scenarios like missing tokens.

**Summary:** A specialized skill for converting Figma designs into production-ready React/Tailwind components via a CLI tool.

**Source credibility:** High; the repository has significant social proof with 549 stars and recent activity.

**Recency:** 

**Source:** [vibeflowing-inc/vibe_figma/skills/vibefigma/SKILL.md](https://github.com/vibeflowing-inc/vibe_figma/blob/f250b8ad6946184b93b8029097a2be3051182cee/skills/vibefigma/SKILL.md) · 549★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vibefigma
description: Convert Figma designs to production-ready React components with Tailwind CSS. Use when user provides a Figma URL, asks to convert Figma designs to React/code, wants to extract components from Figma, or mentions "vibefigma". Requires a Figma access token (via --token flag, FIGMA_TOKEN env var, or .env file).
---

# VibeFigma - Figma to React Converter

Convert Figma designs into React components with Tailwind CSS using the `vibefigma` CLI.

## Usage

### Interactive Mode (Recommended for first-time users)

```bash
npx vibefigma --interactive
```

Prompts for Figma URL, access token, and output paths.

### Direct Command

```bash
npx vibefigma "https://www.figma.com/design/FILE_ID?node-id=X-Y" --token FIGMA_TOKEN
```

### With Environment Variable

```bash
export FIGMA_TOKEN=your_token
npx vibefigma "https://www.figma.com/design/FILE_ID?node-id=X-Y"
```

### Using .env File

The user can add their Figma access token to a `.env` file in their project root:

```env
FIGMA_TOKEN=your_token_here
```

Then run:

```bash
npx vibefigma "https://www.figma.com/design/FILE_ID?node-id=X-Y"
```

Note: If the token is not configured, vibefigma will throw an error.
```

</details>
