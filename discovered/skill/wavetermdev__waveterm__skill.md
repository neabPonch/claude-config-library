---
name: wavetermdev__waveterm__skill
source: https://github.com/wavetermdev/waveterm/blob/a5ac096233f825ad7b5776c4b14da5be0fd75b29/.kilocode/skills/electron-api/SKILL.md
repo: wavetermdev/waveterm
kind: skill
stars: 21266
last_pushed: 2026-06-10T17:41:17Z
license: apache-2.0
score: 9
domains: [electron, desktop-app, ipc]
tags: [electron, typescript, api-integration]
curated: 2026-06-15
curated_by: config-scout
---

# wavetermdev/waveterm — skill

**Why it's worth keeping:** It defines exact file sequences and communication patterns (sync/async/fire-and-forget) including critical warnings like the sync 'returnValue' requirement to prevent browser hangs.

**Summary:** Provides a rigorous structural workflow for adding new Electron-to-Frontend API methods via IPC.

**Source credibility:** High; based on a highly starred, actively maintained open-source terminal project.

**Recency:** Current; utilizes modern Electron IPC best practices (invoke/handle).

**Source:** [wavetermdev/waveterm/.kilocode/skills/electron-api/SKILL.md](https://github.com/wavetermdev/waveterm/blob/a5ac096233f825ad7b5776c4b14da5be0fd75b29/.kilocode/skills/electron-api/SKILL.md) · 21266★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: electron-api
description: Guide for adding new Electron APIs to Wave Terminal. Use when implementing new frontend-to-electron communications via preload/IPC.
---

# Adding Electron APIs

Electron APIs allow the frontend to call Electron main process functionality directly via IPC.

## Four Files to Edit

1. [`frontend/types/custom.d.ts`](frontend/types/custom.d.ts) - TypeScript [`ElectronApi`](frontend/types/custom.d.ts:82) type
2. [`emain/preload.ts`](emain/preload.ts) - Expose method via `contextBridge`
3. [`emain/emain-ipc.ts`](emain/emain-ipc.ts) - Implement IPC handler
4. [`frontend/preview/preview-electron-api.ts`](frontend/preview/preview-electron-api.ts) - Add a no-op stub to keep the `previewElectronApi` object in sync with the `ElectronApi` type

## Three Communication Patterns

1. **Sync** - `ipcRenderer.sendSync()` + `ipcMain.on()` + `event.returnValue = ...`
2. **Async** - `ipcRenderer.invoke()` + `ipcMain.handle()`
3. **Fire-and-forget** - `ipcRenderer.send()` + `ipcMain.on()`

## Example: Async Method

### 1. Define TypeScript Interface

In [`frontend/types/custom.d.ts`](frontend/types/custom.d.ts):

```typescript
type ElectronApi = {
    captureScreenshot:
```

</details>
