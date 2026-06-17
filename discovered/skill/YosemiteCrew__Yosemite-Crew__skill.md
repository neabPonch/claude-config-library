---
name: YosemiteCrew__Yosemite-Crew__skill
source: https://github.com/YosemiteCrew/Yosemite-Crew/blob/c6719970a9bae76cbb58bd9369eb7fafa60bee24/.claude/skills/mobile-patterns/SKILL.md
repo: YosemiteCrew/Yosemite-Crew
kind: skill
stars: 2074
last_pushed: 2026-06-15T17:25:57Z
license: other
score: 9
domains: [mobile-development, react-native]
tags: [react-native, redux-toolkit, testing-automation, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# YosemiteCrew/Yosemite-Crew — skill

**Why it's worth keeping:** The extremely detailed 'Coverage Mandate' and the inclusion of precise command-line workflows for verifying coverage are elite agent instructions. It also provides highly actionable 'Gotchas' that address platform-specific pitfalls like file paths and permissions.

**Summary:** A highly rigorous skill file for a React Native mobile application that enforces architectural standards and testing protocols. It defines specific guardrails for state management, navigation, and internationalization.

**Source credibility:** High; a mature, highly starred open-source project with active maintenance.

**Recency:** Current; utilizes modern standards like React Navigation 7 and Redux Toolkit.

**Source:** [YosemiteCrew/Yosemite-Crew/.claude/skills/mobile-patterns/SKILL.md](https://github.com/YosemiteCrew/Yosemite-Crew/blob/c6719970a9bae76cbb58bd9369eb7fafa60bee24/.claude/skills/mobile-patterns/SKILL.md) · 2074★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Mobile App Patterns — Yosemite Crew

## Description

Use this skill when working on apps/mobileAppYC. Covers React Native architecture, navigation, Redux state management, and mobile-specific conventions.

TRIGGER: any task in apps/mobileAppYC — screens, components, navigation, state, or native integrations.

---

## Architecture

```
apps/mobileAppYC/
  src/
    screens/        ← Full-screen views
    components/     ← Reusable UI components
    navigation/     ← React Navigation config
    store/          ← Redux Toolkit slices
    services/       ← API calls (axios)
    hooks/          ← Custom React hooks
    utils/          ← Pure utility functions
    i18n/           ← Translation files (i18next)
    assets/         ← Images, fonts
```

---

## State Management

**Redux Toolkit** (not Zustand — that's frontend only). Redux Persist is enabled.

```ts
// Define a slice
import { createSlice } from '@reduxjs/toolkit';

const appointmentSlice = createSlice({
  name: 'appointments',
  initialState,
  reducers: { ... },
});
```

Never mix Redux and local `useState` for the same piece of data. Local state is for ephemeral UI state (modal open, input focus). Shared/persisted state g
```

</details>
