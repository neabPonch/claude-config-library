---
name: magic-spells__dialog-panel
source: https://github.com/magic-spells/dialog-panel/blob/b4dc16d5f05c07a06c91bf51500e97df83ea5eed/claude.md
repo: magic-spells/dialog-panel
kind: claude-md
stars: 0
last_pushed: 2026-05-11T04:24:09Z
license: mit
score: 9
domains: [web-frontend, design-systems]
tags: [web-components, state-machine, accessibility]
curated: 2026-06-16
curated_by: config-scout
---

# magic-spells/dialog-panel — claude-md

**Why it's worth keeping:** Includes a visual state machine diagram and 'Key Design Decisions' which provide the AI with the rationale behind non-obvious code patterns.

**Summary:** Provides high-density technical context by documenting component architecture, state machine flows, and specific implementation nuances.

**Source credibility:** Low star count but reflects high-quality technical writing and professional engineering standards.

**Recency:** Very recent; updated within the last month.

**Source:** [magic-spells/dialog-panel/claude.md](https://github.com/magic-spells/dialog-panel/blob/b4dc16d5f05c07a06c91bf51500e97df83ea5eed/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Dialog Panel - AI Context

## Overview

`@magic-spells/dialog-panel` is a lightweight web component that wraps native `<dialog>` elements with state-driven animations. It leverages browser-native features for accessibility (focus trapping, escape key handling) while providing a clean API for animations and event handling.

## Architecture

### Components

1. **DialogPanel** (`<dialog-panel>`) - Main wrapper component
   - Manages state machine: `hidden` → `showing` → `shown` → `hiding`
   - Handles show/hide animations via CSS transitions
   - Emits lifecycle events: `beforeShow`, `shown`, `beforeHide`, `hidden`
   - Auto-creates `<dialog-backdrop>` if not present

2. **DialogBackdrop** (`<dialog-backdrop>`) - Visual backdrop element
   - Provides cross-browser animated backdrop (Firefox doesn't animate native `::backdrop`)
   - Uses oversized dimensions (`200vw` × `200dvh`) to work inside transformed parents
   - Click-to-close functionality

### State Machine

```
hidden ──show()──> showing ──RAF──> shown
                                      │
                                   hide()
                                      │
                                      v
hidden <──clo
```

</details>
