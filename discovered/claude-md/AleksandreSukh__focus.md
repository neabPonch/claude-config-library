---
name: AleksandreSukh__focus
source: https://github.com/AleksandreSukh/focus/blob/8fc30a1c5b7db29aa810dd054455b5b8c3820e7c/CLAUDE.md
repo: AleksandreSukh/focus
kind: claude-md
stars: 2
last_pushed: 2026-06-12T18:39:53Z
license: gpl-3.0
score: 9
domains: [cross-platform, cli-tools]
tags: [modular-context, negative-constraints, multi-client]
curated: 2026-06-16
curated_by: config-scout
---

# AleksandreSukh/focus — claude-md

**Why it's worth keeping:** Uses a modular 'skill-based' context pattern to avoid token bloat and includes explicit negative constraints to prevent searching build artifacts.

**Summary:** Provides high-level architecture and cross-client sync rules while directing the LLM to specialized 'skill' files for specific domain deep-dives.

**Source credibility:** Low star count, but the documentation structure demonstrates high professional maturity.

**Recency:** Highly current; utilizes cutting-edge development environments (JDK 26).

**Source:** [AleksandreSukh/focus/CLAUDE.md](https://github.com/AleksandreSukh/focus/blob/8fc30a1c5b7db29aa810dd054455b5b8c3820e7c/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Focus — guidance for Claude Code

Mind-map/task app with three clients editing the same `FocusMaps/*.json` files: .NET 8 console app (`Focus/`), static PWA (`pwa/`), Android Kotlin/Compose client (`android/`).

**Before exploring the repo, read the matching project skill — they replace broad scans:**

- `focus-architecture` — repo map, which client owns what, shared concepts. Start here.
- `focus-map-schema` — map JSON schema, mutation/merge/CAS sync rules, llm-interop format.
- `focus-console-dev` — console app layout, command catalogs, dotnet build/test, E2E pipe harness.
- `focus-pwa-dev` — PWA modules, main.js patterns, offline queue, service-worker cache bump rule, `node --test` invocation.
- `focus-android-dev` — Android packages, ViewModel/sync coordinator, gradlew commands (needs JAVA_HOME to JDK 26).

Cross-client rule: domain/sync behavior changes usually must be mirrored in all three clients (PWA is the reference implementation; Android ports from it).

Never search generated dirs: `.artifacts/`, `.dotnet/`, `.vs/`, `**/bin/`, `**/obj/`, `pwa/dist/`, `Focus/Focus/publish/`, `Releases/`. Root `*.log` files are stale build output.

Quick commands:

```powershell
dotnet b
```

</details>
