---
name: robingtz__SprachPlan
source: https://github.com/robingtz/SprachPlan/blob/df0394570860ea2a3ee93d4297533e16c21debf6/Claude.md
repo: robingtz/SprachPlan
kind: claude-md
stars: 0
last_pushed: 2026-03-31T16:10:23Z
license: unknown
score: 7
domains: [web-frontend, backend-api, qa-testing]
tags: [negative-constraints, error-mapping, educational]
curated: 2026-06-16
curated_by: config-scout
---

# robingtz/SprachPlan — claude-md

**Why it's worth keeping:** The bug-to-file mapping table is an excellent way to provide context for specialized tasks like QA or testing. It also includes clear, multi-terminal startup instructions.

**Summary:** This file establishes strict 'negative constraints' preventing the AI from fixing intentional bugs while providing a structured map of known issues.

**Source credibility:** Low; it appears to be an educational/student project with no stars and unknown licensing.

**Recency:** 

**Source:** [robingtz/SprachPlan/Claude.md](https://github.com/robingtz/SprachPlan/blob/df0394570860ea2a3ee93d4297533e16c21debf6/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SprachPlan - Stundenplan-WebApp mit absichtlichen Bugs

## Projektzweck

SprachPlan ist eine **Lehr-WebApp** für den Berufsschulunterricht (Software-Testing / QA). Die App enthält **18 absichtlich eingebaute Fehler**, die Schülerinnen und Schüler finden und dokumentieren sollen.

**WICHTIG:** Bugs NICHT fixen, es sei denn explizit angefragt. Die Fehler sind das Feature.

## Tech-Stack

- **Frontend:** React + TypeScript + Tailwind CSS (Vite, Port 3000)
- **Backend:** Java Spring Boot 3.2.1 + H2-Datenbank (Maven, Port 8080)
- **Architektur:** Frontend → REST API → H2 (file-basiert, persistent)

## Starten

```bash
# Terminal 1: Backend
cd backend && ./mvnw spring-boot:run

# Terminal 2: Frontend
npm run dev
```

Login: `max.mustermann@email.com` / `test123`

## Projektstruktur (Kurzfassung)

```
sprachplan/
├── App.tsx                    # Hauptkomponente (Bugs: A-01, F-01)
├── constants.ts               # UI-Konstanten (Bug: A-02)
├── components/
│   ├── Login.tsx              # Login-Formular (Bugs: V-01, V-02)
│   ├── Schedule.tsx           # Stundenplan (Bugs: A-03, A-04, F-03, F-04, R-01, R-03)
│   ├── CourseDetailModal.tsx  # Detailansicht (Bugs: A-05, F-05, R-02)
│   └── Bu
```

</details>
