---
name: valeriiSkliar__currency-converter-app
source: https://github.com/valeriiSkliar/currency-converter-app/blob/221495d24ca941e33666aace9fe42bb48c9b897a/claude.md
repo: valeriiSkliar/currency-converter-app
kind: claude-md
stars: 1
last_pushed: 2026-06-09T08:33:45Z
license: mit
score: 9
domains: [mobile-development, frontend]
tags: [react-native, expo, architecture, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# valeriiSkliar/currency-converter-app — claude-md

**Why it's worth keeping:** The explicit 'Smart vs. Dumb' component separation rules prevent AI from mixing business logic with UI; the inclusion of hard constraints like function line limits and specific import patterns is excellent.

**Summary:** A high-density instruction set for a React Native/Expo project that enforces strict architectural boundaries between UI and logic. It provides clear guardrails for state management, theming, and component responsibilities.

**Source credibility:** Low social proof (1 star), but highly professional-grade technical documentation typical of production templates.

**Recency:** Very current, referencing modern Expo SDK 54 and recent React Native versions.

**Source:** [valeriiSkliar/currency-converter-app/claude.md](https://github.com/valeriiSkliar/currency-converter-app/blob/221495d24ca941e33666aace9fe42bb48c9b897a/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
> This project was generated from the [Obytes React Native Template](https://github.com/obytes/react-native-template-obytes), a production-ready React Native starter with modern tooling and best practices.

## What: Technology Stack

- **Expo SDK 54** with React Native 0.81.5 - Managed React Native development
- **TypeScript** - Strict type safety throughout
- **Expo Router 6** - File-based routing (like Next.js)
- **TailwindCSS** via Uniwind/Nativewind - Utility-first styling for React Native
- **Zustand** - Lightweight global state management
- **React Query** - Server state and data fetching
- **TanStack Form + Zod** - Type-safe form handling and validation
- **MMKV** - Encrypted local storage
- **Jest + React Testing Library** - Unit testing

## What: Project Structure

```
src/
├── app/              # Expo Router file-based routes (add new routes here)
├── features/         # Feature modules - auth, feed, settings are EXAMPLES
├── components/ui/    # Pre-built UI components (button, input, modal, etc.)
├── lib/              # Pre-configured utilities (api, auth, i18n, storage)
├── translations/     # i18n files (en.json, ar.json - add more languages)
└── global.css        # Ta
```

</details>
