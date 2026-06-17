---
name: nativewind__nativewind__skill
source: https://github.com/nativewind/nativewind/blob/d971e3770d60a4523987c0b6644e1c284b1258ee/.claude/skills/debug-nw/SKILL.md
repo: nativewind/nativewind
kind: skill
stars: 7939
last_pushed: 2026-06-11T23:33:20Z
license: mit
score: 8
domains: [mobile-development, react-native]
tags: [debugging, troubleshooting, config-verification]
curated: 2026-06-15
curated_by: config-scout
---

# nativewind/nativewind — skill

**Why it's worth keeping:** Uses specific code snippets as verification patterns and explicitly lists high-probability 'common mistakes' to guide the agent's reasoning.

**Summary:** Provides a systematic diagnostic checklist for debugging Nativewind v5 configuration issues across Metro, Babel, and PostCSS.

**Source credibility:** High; sourced from a widely used (7.9k stars) and actively maintained library.

**Recency:** Very current, specifically targeting modern Tailwind v4/Nativewind v5 requirements.

**Source:** [nativewind/nativewind/.claude/skills/debug-nw/SKILL.md](https://github.com/nativewind/nativewind/blob/d971e3770d60a4523987c0b6644e1c284b1258ee/.claude/skills/debug-nw/SKILL.md) · 7939★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: debug-nw
description: Debug a Nativewind v5 setup issue. Walks through common configuration problems with metro, babel, postcss, and dependencies.
allowed-tools: Read, Grep, Glob, Bash
---

You are helping debug a Nativewind v5 configuration issue. Walk through these checks systematically.

## 1. Version check

- Is `nativewind` at v5.x? (`package.json`)
- Is `react-native-css` installed as a peer dependency? Must be `^3.0.1`
- Is `tailwindcss` v4+? Must be `>4.1.11`
- Is `@tailwindcss/postcss` installed?

## 2. PostCSS config

Nativewind v5 uses Tailwind CSS v4's PostCSS plugin. Check for `postcss.config.mjs`:

```javascript
export default {
  plugins: {
    "@tailwindcss/postcss": {},
  },
};
```

**Common mistake**: Using Tailwind v3's `tailwindcss` PostCSS plugin instead of `@tailwindcss/postcss`.

## 3. CSS entry file

Check that the global CSS file imports the nativewind theme:

```css
@import "tailwindcss";
@import "nativewind/theme";
```

**Common mistake**: Missing `@import "nativewind/theme"` — this provides RN-specific utilities.

## 4. Metro config

Check `metro.config.js` for `withNativewind()`:

```javascript
const { withNativewind } = require("nativewind/me
```

</details>
