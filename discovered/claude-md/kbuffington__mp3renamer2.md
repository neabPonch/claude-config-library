---
name: kbuffington__mp3renamer2
source: https://github.com/kbuffington/mp3renamer2/blob/c196165abfa0e9247759a7450573854f3f74311e/claude.md
repo: kbuffington/mp3renamer2
kind: claude-md
stars: 1
last_pushed: 2026-06-15T23:33:39Z
license: mit
score: 9
domains: [web-frontend, desktop-app, electron]
tags: [angular, electron, typescript, testing]
curated: 2026-06-16
curated_by: config-scout
---

# kbuffington/mp3renamer2 — claude-md

**Why it's worth keeping:** Includes exceptional 'how-to' guides for extending system features and highly detailed testing protocols that explain complex async behaviors.

**Summary:** A high-density technical guide covering architectural patterns, file structure, and specific workflow extension procedures for an Angular/Electron app.

**Source credibility:** High-quality documentation despite low star count; appears professionally maintained.

**Recency:** Very current, referencing Angular 19 and modern TypeScript/Electron versions.

**Source:** [kbuffington/mp3renamer2/claude.md](https://github.com/kbuffington/mp3renamer2/blob/c196165abfa0e9247759a7450573854f3f74311e/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MP3 Renamer2

Electron + Angular desktop app for MP3 file renaming, ID3 tagging, MusicBrainz metadata retrieval, and album artwork downloading. Rewrite of an older LabWindows/CVI tool, tailored to foobar2000 conventions.

## Tech Stack

- **Frontend:** Angular 19 with TypeScript 5.3
- **Desktop:** Electron 40 (main process in `main.js`)
- **UI:** Clarity Design System (clr/cds) v17
- **State:** RxJS BehaviorSubjects in services (no NgRx)
- **ID3:** node-id3tag for MP3 metadata I/O
- **Build:** Angular CLI, electron-packager

## Commands

- `npm start` - Angular dev server (localhost:4200)
- `npm run start-id3` - Compile node-id3 module + launch Electron
- `npm run build` - Build Angular app to dist/
- `npm run build:win` - Build + package for Windows (win32-x64)
- `npm run build:osx` - Build + package for macOS (darwin-x64)
- `npm test` - Run unit tests (Karma + Jasmine)
- `ng lint` - ESLint

## Project Structure

```
src/app/
  classes/        # Data models (Track, MetadataObj, MusicBrainz types)
  components/     # Angular components (main, left-panel, right-panel, renamer-grid, etc.)
  services/       # Business logic & state (TrackService, MusicbrainzService, ConfigService, e
```

</details>
