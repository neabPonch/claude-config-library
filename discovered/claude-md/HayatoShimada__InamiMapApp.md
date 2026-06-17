---
name: HayatoShimada__InamiMapApp
source: https://github.com/HayatoShimada/InamiMapApp/blob/5efe547998aee608e7444d9ea1c7f66c4414dcc4/CLAUDE.md
repo: HayatoShimada/InamiMapApp
kind: claude-md
stars: 0
last_pushed: 2025-11-24T08:06:58Z
license: unknown
score: 8
domains: [full-stack, mobile-app, web-admin, firebase]
tags: [firebase, flutter, react, workflow-driven]
curated: 2026-06-15
curated_by: config-scout
---

# HayatoShimada/InamiMapApp — claude-md

**Why it's worth keeping:** The 'Key Development Workflows' section is exceptional; it explains essential state machine transitions (e.g., approval processes) that prevent the AI from breaking business rules. It also uses high-quality, directory-specific command blocks.

**Summary:** A multi-component guide for a Firebase-backed mobile and web ecosystem. It includes categorized development commands and critical business logic workflows.

**Source credibility:** Low star count/maintenance indicates a small or personal project, but the documentation quality is high.

**Recency:** Current; utilizes modern stacks like React 18 and Flutter 3+.

**Source:** [HayatoShimada/InamiMapApp/CLAUDE.md](https://github.com/HayatoShimada/InamiMapApp/blob/5efe547998aee608e7444d9ea1c7f66c4414dcc4/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

InamiMapApp is a Firebase-based mapping platform for Inami town (南砺市井波) featuring shop discovery and event management. The application has two main components: a Flutter mobile app for users to discover shops and events, and a web admin panel for shop owners to manage their information and submit events for approval.

## Project Structure

```
InamiMapApp/
├── web/              # Shop owner admin panel (React/Vite/TypeScript)
│   ├── src/          # React components and pages
│   ├── public/       # Static assets
│   ├── package.json  
│   └── README.md
├── mobile/           # User-facing Flutter app 
│   ├── lib/          # Dart source code
│   ├── android/      # Android platform files
│   ├── ios/          # iOS platform files
│   ├── pubspec.yaml  # Flutter dependencies
│   └── README.md
├── backend/          # Legacy Node.js backend (migrating to Firebase)
├── shared/           # Shared TypeScript types and utilities
├── firebase/         # Firebase configuration and rules
├── DESIGN.md         # Detailed development plan and specifications
```

</details>
