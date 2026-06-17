---
name: sztanko__madeira-pass
source: https://github.com/sztanko/madeira-pass/blob/efef8194849495211f28dc4f4e6c939d2ccc2444/CLAUDE.md
repo: sztanko/madeira-pass
kind: claude-md
stars: 0
last_pushed: 2026-06-14T04:37:57Z
license: unknown
score: 7
domains: [web-frontend, mobile-web]
tags: [product-spec, location-aware, map-integration]
curated: 2026-06-14
curated_by: config-scout
---

# sztanko/madeira-pass — claude-md

**Why it's worth keeping:** The 'User Flow' section provides highly granular state-transition logic, while the 'Routes pre-processing' section gives clear instructions for auxiliary automation tasks.

**Summary:** A detailed functional specification that combines product requirements with specific technical and data-processing instructions.

**Source credibility:** Low social proof; likely a personal project/prototype.

**Recency:** Current; uses modern tech stack like MapLibre and TypeScript.

**Source:** [sztanko/madeira-pass/CLAUDE.md](https://github.com/sztanko/madeira-pass/blob/efef8194849495211f28dc4f4e6c939d2ccc2444/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
## Intro
Madeira Pass is a micro web app that tracks your location and warns you if you need to buy a pass to walk on the root you are on. It is designed for mobile and is client-side only - there is no backend.


## Elements on the screen:
- Map normally covering 100% of the screen. It is a map of madeira island, with all the hiking routes that need payment for it. Normally, it should show the whole archipelago fitting the map. Map also has typical icons: +/- (for zooming in), 'Find my location' icon + An accordion menu icon - when clicked, it should show links to 'Main', 'List of routes', 'Madeira pass info' and 'About' pages. These pages should be shown on the info panel (see below)
- based on the user's location or user's action, screen can be split into two parts (upper abd lower) - upper wouls show the same map, lower would be an info/interactions panel. It is possible to close the panel, if it is open, but if necessary, it might re-appear if user location changes or user makes an interaction (presses a button, etc). Whenever info panel appears or hides, this should be done using a sleack css animation. 


## User Flow 
1. It requests your location and if within Madeira, will
```

</details>
