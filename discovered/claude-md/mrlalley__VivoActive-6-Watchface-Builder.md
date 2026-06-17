---
name: mrlalley__VivoActive-6-Watchface-Builder
source: https://github.com/mrlalley/VivoActive-6-Watchface-Builder/blob/eb5b12b2f705a73df31e99f98c159439690a56f2/Claude.md
repo: mrlalley/VivoActive-6-Watchface-Builder
kind: claude-md
stars: 0
last_pushed: 2026-06-01T18:07:53Z
license: unknown
score: 9
domains: [embedded-systems, desktop-app, build-engineering]
tags: [sdk-management, cache-protocol, environment-enforcement, logging-standards]
curated: 2026-06-16
curated_by: config-scout
---

# mrlalley/VivoActive-6-Watchface-Builder — claude-md

**Why it's worth keeping:** Provides explicit 'update protocols' for dependency synchronization and 'critical setup facts' that explain non-obvious execution orders and file system constraints.

**Summary:** A highly technical guide managing complex SDK versioning contracts, build-time code generation, and strict runtime environment requirements.

**Source credibility:** Low social proof (0 stars), but the depth of technical detail suggests a highly disciplined developer.

**Recency:** Extremely current, referencing Node.js 22 and modern toolchain requirements.

**Source:** [mrlalley/VivoActive-6-Watchface-Builder/Claude.md](https://github.com/mrlalley/VivoActive-6-Watchface-Builder/blob/eb5b12b2f705a73df31e99f98c159439690a56f2/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — WatchFace Builder

When working on this repository, read this file before making any changes.

---

## Repository purpose

A desktop Electron app that provides a GUI for designing Garmin Vivoactive 6 watch
faces. The user places elements on a 390x390 canvas; the app generates a Garmin
Connect IQ Monkey C project and compiles it to a `.prg` binary via the `monkeyc`
CLI. The app runs as either an Electron window or a standalone Express server.

---

## Template versioning contract

`garmin-project-template/VERSION` is the single source of truth for template-to-SDK compatibility. It must be updated every time the template is modified for a new SDK version.

### VERSION fields

| Field | Description | Must match |
|---|---|---|
| `templateVersion` | Semver for the template itself | — |
| `minSdkVersion` | Minimum Connect IQ SDK required to compile | `bin/version.txt` in installed SDK |
| `minApiLevel` | API level targeted by the template | `minSdkVersion` attribute in `manifest.xml` |
| `targetDeviceId` | Preferred build target | `<iq:product id="..."/>` in `manifest.xml` |
| `fallbackDeviceId` | Used if targetDeviceId absent from SDK | Documented in `notes` field |

`min
```

</details>
