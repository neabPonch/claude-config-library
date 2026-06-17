---
name: codelynx__SwiftOpenUI
source: https://github.com/codelynx/SwiftOpenUI/blob/6150b964a7cb1cf3a961770f6947ed55c1a31433/CLAUDE.md
repo: codelynx/SwiftOpenUI
kind: claude-md
stars: 21
last_pushed: 2026-04-29T05:20:46Z
license: mit
score: 9
domains: [cross-platform, systems-programming, swift]
tags: [architecture-rules, git-protocol, api-catalog]
curated: 2026-06-15
curated_by: config-scout
---

# codelynx/SwiftOpenUI — claude-md

**Why it's worth keeping:** The 'Multi-Platform Branch Protocol' and 'Key Design Decisions' sections provide high-stakes instructions that prevent the AI from breaking cross-platform separation or introducing stale merges.

**Summary:** This file defines a rigorous multi-platform development workflow, including strict git branch protocols and architectural constraints to maintain platform independence.

**Source credibility:** High; the documentation is exceptionally professional, detailed, and follows industry-standard architectural patterns.

**Recency:** Current; includes modern Swift toolchain and Wasm considerations.

**Source:** [codelynx/SwiftOpenUI/CLAUDE.md](https://github.com/codelynx/SwiftOpenUI/blob/6150b964a7cb1cf3a961770f6947ed55c1a31433/CLAUDE.md) · 21★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SwiftOpenUI

Cross-platform SwiftUI framework — write SwiftUI, run anywhere.

## Project Structure

- `Sources/SwiftOpenUI/` — Core platform-independent library (Views, State, Layout, Modifiers, Environment, Backend protocol)
- `Sources/Backend/GTK4/` — Linux backend (GTK4): CGTK system module, CGTKBridge interop, Rendering
- `Sources/Backend/Win32/` — Windows backend (Win32): CWin32, CWin32Bridge, Rendering + LayoutEngine
- `Sources/Backend/Web/` — Web/Wasm backend (experimental): DOM rendering via JavaScriptKit
- `Examples/Showcase/` — Polished demo apps (HelloWorld, Stopwatch, ColorMixer, Calculator, SimplePaint, LayoutStress)
- `Examples/Parity/` — Matrix-backed coverage examples (11 parity targets)
- `Tests/SwiftOpenUITests/` — Core tests (platform-independent)
- `Tests/BackendTests/` — Platform-specific backend tests
- `docs/` — Architecture, API reference, porting guides, mission
- `configure` — Setup script: installs swiftly, open-source Swift toolchain, Wasm SDK

## Branches

- `main` — clean until v1.0, do not merge to main without explicit instruction
- `develop` — active development, all work happens here
- `experimental/*` — experimental features (e.g. `experimental/
```

</details>
