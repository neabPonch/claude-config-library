---
name: daohainam__emulator-8086-js
source: https://github.com/daohainam/emulator-8086-js/blob/181314f229f3047164e0c99e9da178f6883174a3/CLAUDE.md
repo: daohainam/emulator-8086-js
kind: claude-md
stars: 2
last_pushed: 2026-05-28T22:03:43Z
license: unknown
score: 9
domains: [low-level, web-frontend, emulator]
tags: [architecture-specification, state-management, hardware-simulation]
curated: 2026-06-15
curated_by: config-scout
---

# daohainam/emulator-8086-js — claude-md

**Why it's worth keeping:** Uses highly structured tables to map functions/components to purposes and provides exact details on the custom state management pattern used to bypass React's overhead.

**Summary:** Acts as a technical specification detailing how low-level hardware emulation logic interacts with the React UI layer.

**Source credibility:** Niche hobbyist project; high density of technical detail despite low star count.

**Recency:** Very current; includes modern stack details like React 19/Vite.

**Source:** [daohainam/emulator-8086-js/CLAUDE.md](https://github.com/daohainam/emulator-8086-js/blob/181314f229f3047164e0c99e9da178f6883174a3/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Commands

```bash
npm run dev        # Start Vite dev server with HMR
npm run build      # Production build (output to dist/)
npm run lint       # Run ESLint
npm run preview    # Preview production build locally
```

No test suite is configured.

## Architecture

This is an Intel 8086 processor emulator with a web-based IDE and debugger, built with React 19 + Vite + Tailwind CSS.

**The emulator is split across three source files:**
- `src/App.jsx` — all UI components, state management, and the main application shell
- `src/CPU8086.js` — the 8086 CPU emulation core: binary decoder engine, memory manager, flags, BIOS interrupt handlers (INT 10h/13h/16h), and the `executeStep` function
- `src/Assembler8086.js` — standalone two-pass NASM-compatible x86 assembler that compiles source text to a `Uint8Array` of machine code

`App.jsx` is structured in three sections marked by comments: constants/utilities, UI sub-components, and the main app + CPU core logic.

### CPU State Model

All CPU state lives in a single `useRef` object (`eng`):
- **Registers:** `reg` — AX, BX,
```

</details>
