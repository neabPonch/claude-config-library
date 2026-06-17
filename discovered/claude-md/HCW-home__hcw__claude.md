---
name: HCW-home__hcw__claude
source: https://github.com/HCW-home/hcw/blob/505b86d6bc4a6a73237097a7ad4e1dccf2d097ea/practitioner/CLAUDE.md
repo: HCW-home/hcw
kind: claude-md
stars: 7
last_pushed: 2026-06-09T10:38:55Z
license: gpl-3.0
score: 9
domains: [web-frontend, mobile-app, backend-api, fullstack]
tags: [angular, django, ui-library, multi-service]
curated: 2026-06-15
curated_by: config-scout
---

# HCW-home/hcw — claude-md

**Why it's worth keeping:** The 'UI Component Library' section provides strict directives to use existing components over creating new ones; it also includes highly specific CLI commands with necessary flags for all sub-services.

**Summary:** A comprehensive multi-service guide covering Angular frontend, Ionic mobile app, and Django backend workflows.

**Source credibility:** Low star count but the structure indicates a real-world professional healthcare application.

**Recency:** Very current, mentioning modern Angular standalone component patterns and Django 5.x.

**Source:** [HCW-home/hcw/practitioner/CLAUDE.md](https://github.com/HCW-home/hcw/blob/505b86d6bc4a6a73237097a7ad4e1dccf2d097ea/practitioner/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a healthcare consultation web application with a **multi-service architecture**:

- **practitioner/**: Angular 20 frontend for healthcare practitioners
- **patient/**: Ionic Angular mobile app for patients  
- **backend/**: Django REST API with WebRTC, real-time messaging, and async task processing
- **Root-level Makefile**: Coordinates building across all services

## Development Commands

### Practitioner Frontend (Angular 20)
Navigate to `practitioner/` directory:
- **Start development server**: `ng serve` (serves at http://localhost:4200)
- **Build application**: `ng build` (outputs to dist/)
- **Build for production**: `ng build --configuration production`
- **Run tests**: `ng test` (uses Karma + Jasmine)
- **Lint code**: `ng lint` (uses Angular ESLint with TypeScript and template rules)
- **Generate components**: `ng generate component component-name`
- **Watch build**: `ng build --watch --configuration development`
- **Extract i18n**: `ng extract-i18n`

### Patient Mobile App (Ionic Angular)
Navigate to `patient/` directory:
- **St
```

</details>
