---
name: thelegend1233__The-Best-Slot-Machine-
source: https://github.com/thelegend1233/The-Best-Slot-Machine-/blob/ded52a323e623161c37ae08ae13ed52a57524bc7/Claude.md
repo: thelegend1233/The-Best-Slot-Machine-
kind: claude-md
stars: 0
last_pushed: 2026-04-21T18:02:59Z
license: unknown
score: 9
domains: [web-frontend, game-dev]
tags: [vanilla-js, incremental-build, constraints-heavy]
curated: 2026-06-16
curated_by: config-scout
---

# thelegend1233/The-Best-Slot-Machine- — claude-md

**Why it's worth keeping:** The 'Build Order' provides an excellent roadmap for iterative development, while the 'What NOT to do' section effectively suppresses AI tendency toward over-engineering. The instruction to run a Monte Carlo test is a top-tier way to ensure mathematical correctness.

**Summary:** A highly prescriptive guide for building a vanilla JS game with strict architectural constraints. It uses incremental development stages and logic verification via Monte Carlo simulation.

**Source credibility:** Low popularity (0 stars), likely a personal learning repository.

**Recency:** Current; demonstrates advanced techniques like negative constraints and simulation-based verification highly relevant to modern AI coding agents.

**Source:** [thelegend1233/The-Best-Slot-Machine-/Claude.md](https://github.com/thelegend1233/The-Best-Slot-Machine-/blob/ded52a323e623161c37ae08ae13ed52a57524bc7/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Slot Machine Project

## What this is

A personal-learning browser slot machine. Generic nature/animal theme. Runs as a static site — open `index.html` in a browser and it works. No server, no build step, no deploy pipeline.

## Hard constraints

- **Vanilla HTML, CSS, and JavaScript only.** No React, Vue, Svelte, jQuery, TypeScript, bundlers, or package managers.
- **No build step.** If I can’t refresh the browser and see the change, it’s the wrong approach.
- **No external runtime dependencies** except Howler.js for audio (loaded from CDN, added only when audio is implemented).
- **Three files max for core:** `index.html`, `style.css`, `game.js`. Split `game.js` later only if it exceeds ~800 lines.
- **No localStorage wrappers, no state management libraries.** Plain `localStorage.getItem` / `setItem`.
- **Code must be readable by a non-developer.** Clear variable names, comments on non-obvious logic, no clever one-liners.

## Game specification

### Grid and reels

- 5 reels, 3 rows visible per reel (5x3 grid).
- Each reel is a strip of 30–40 symbols. Spinning picks a random offset and lands on it.
- Reel strips are weighted (more low-value symbols, fewer high-value) to hit ~95
```

</details>
