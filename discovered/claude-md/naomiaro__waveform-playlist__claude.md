---
name: naomiaro__waveform-playlist__claude
source: https://github.com/naomiaro/waveform-playlist/blob/6971ab6f2724efe622176b7577233a461d261f61/website/CLAUDE.md
repo: naomiaro/waveform-playlist
kind: claude-md
stars: 1649
last_pushed: 2026-06-12T01:52:02Z
license: mit
score: 9
domains: [web-frontend, audio-engineering]
tags: [css-pitfalls, ssr-patterns, design-system, web-audio]
curated: 2026-06-16
curated_by: config-scout
---

# naomiaro/waveform-playlist — claude-md

**Why it's worth keeping:** It focuses heavily on 'pitfalls' and 'gotchas'—essential for preventing an AI from introducing subtle bugs in CSS layout or Web Audio execution. It also provides strong aesthetic constraints to ensure generated UI matches the brand identity.

**Summary:** A high-density technical guide for a Docusaurus website that includes specific CSS failure modes, audio engine race conditions, and SSR patterns.

**Source credibility:** Highly credible; comes from a well-starred, actively maintained audio engineering project.

**Recency:** Current; addresses modern web concerns like SSR/SSG limitations and CSS container quirks.

**Source:** [naomiaro/waveform-playlist/website/CLAUDE.md](https://github.com/naomiaro/waveform-playlist/blob/6971ab6f2724efe622176b7577233a461d261f61/website/CLAUDE.md) · 1649★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Website Package (Docusaurus)

## Aesthetic: Berlin Underground

Industrial / electronic-music-culture aesthetic. When adding examples or UI:

- **Dark gradient backgrounds** with high-contrast text
- **Monospace fonts** (Courier New) for timestamps and technical elements
- **Grungy details** — `//` prefixes on timestamps, text shadows
- **Muted palette** with strategic accent colors
- **Minimal, utilitarian** — form follows function

**Dark-mode palette ("Ampelmännchen Traffic Light"** — DDR pedestrian-signal homage):
- 🟢 Green `#63C75F` — buttons / links
- 🟡 Amber `#c49a6c` — waveform bars, body text
- 🔴 Red `#d08070` — headings, accents

Reference: the Flexible API example showcases full customization (custom playheads, grungy timestamps, monospace clip headers).

## CSS Pitfalls

### `backdrop-filter` breaks `position: fixed` children

`backdrop-filter` on an ancestor creates a new containing block for `position: fixed` descendants. The mobile navbar sidebar (`position: fixed; top: 0; bottom: 0`) becomes constrained to the ancestor's height instead of the viewport.

**Fix:** Scope `backdrop-filter` with `:not(.navbar-sidebar--show)` so it only applies when the mobile sidebar i
```

</details>
