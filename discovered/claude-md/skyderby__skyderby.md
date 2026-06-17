---
name: skyderby__skyderby
source: https://github.com/skyderby/skyderby/blob/4c38150fb9620b7396279499eee431f69e5169e3/CLAUDE.md
repo: skyderby/skyderby
kind: claude-md
stars: 83
last_pushed: 2026-06-09T18:37:43Z
license: other
score: 8
domains: [web-application, ruby-on-rails]
tags: [rails, localization, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# skyderby/skyderby — claude-md

**Why it's worth keeping:** The specific translation pathing instructions prevent locale-file sprawl, while the 'no service objects' rule prevents an AI from introducing modern technical debt into an existing codebase.

**Summary:** Enforces strict architectural constraints (no service objects), CSS migration rules, and a highly granular localization file hierarchy.

**Source credibility:** Niche project with consistent recent activity.

**Recency:** Current; explicitly optimized for Claude Code usage.

**Source:** [skyderby/skyderby/CLAUDE.md](https://github.com/skyderby/skyderby/blob/4c38150fb9620b7396279499eee431f69e5169e3/CLAUDE.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

Skyderby is a web application that provides gps tracks analysys, online ranknig and competition scoring
for skydivers and base jumpers.

## Style Guidelines
- You must not write comments in the code unless explicitly requested

### Ruby
- Verify code style with Rubocop and run corresponding test if it exists
- Prefer using fixtures and manually creating records instead of factories
- Do not create service objects unless explicitly requested, either use a model method, concern or place the code in the controller
- Check with rubocop for style issues

### Frontend
- For new styles use CSS, if you need to touch SCSS - rewrite it to CSS
- Use shared styles as if you are creating a design system instead of writing page specific styles.
  Write utility styles.
- Use what Hotwire offers - Stimulus, Turbo Streams and Turbo Frames
- Pass urls as data-attribute using route helpers, do not hardcode urls in JS
- Verify JS code style with `yarn lint`, if there is corresponding test to file - run test too

### Translations
- Application is translated to English, Russian, German, I
```

</details>
