---
name: pmndrs__xr__skill
source: https://github.com/pmndrs/xr/blob/8d2fda1ac27acb8959bd8055b8b3a1a7dcfb0611/.agents/skills/vitexec/SKILL.md
repo: pmndrs/xr
kind: skill
stars: 2595
last_pushed: 2026-05-29T01:42:32Z
license: other
score: 9
domains: [web-frontend, 3d-graphics, cli-tools]
tags: [vite, runtime-inspection, threejs, webxr]
curated: 2026-06-15
curated_by: config-scout
---

# pmndrs/xr — skill

**Why it's worth keeping:** It introduces the powerful technique of importing application stores directly into the execution snippet rather than relying on brittle DOM scraping.

**Summary:** Provides a specialized skill for agents to execute code within a running Vite browser session to inspect live state, DOM, and WebGL/WebXR contexts.

**Source credibility:** Highly credible; from the pmndrs organization, which is a leader in the React-Three-Fiber ecosystem.

**Recency:** Very current, updated within the last month.

**Source:** [pmndrs/xr/.agents/skills/vitexec/SKILL.md](https://github.com/pmndrs/xr/blob/8d2fda1ac27acb8959bd8055b8b3a1a7dcfb0611/.agents/skills/vitexec/SKILL.md) · 2595★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: vitexec
description: Use this skill when an AI agent needs to inspect, verify, or debug a live Vite app by running temporary snippets inside the browser page and reading browser logs. Use for client state after interactions, imported app modules, DOM state, human-like input, canvas/WebGL/Three.js state, screenshots, videos, WebXR/Three.js XR with IWER, and runtime-only behavior without editing app files.
---

# vitexec

Use `vitexec` when the truth lives in the running browser: client state, imported app modules, DOM, canvas/WebGL, screenshots, recordings, or browser-only errors.

Do not use it for questions static files, unit tests, or TypeScript can answer directly.

## References

- If `vitexec` or Playwright is missing, read [references/install.md](references/install.md).
- For mouse, keyboard, pointer lock, gamepad, or other input, read [references/inputs.md](references/inputs.md).
- For WebXR, read [references/webxr.md](references/webxr.md).

## Workflow

1. Identify the page path if it is not `/`.
2. Write the smallest snippet that performs the user-like action or reads the browser-only state.
3. Run `vitexec '<snippet>'`, adding `--path`, `--gpu`, `--screenshot`,
```

</details>
