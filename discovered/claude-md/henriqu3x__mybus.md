---
name: henriqu3x__mybus
source: https://github.com/henriqu3x/mybus/blob/1ed0a602c149d9f7fe1cfcd53be29a241ecbbe82/CLAUDE.md
repo: henriqu3x/mybus
kind: claude-md
stars: 0
last_pushed: 2026-05-28T21:57:07Z
license: apache-2.0
score: 8
domains: [mobile-app, flutter-dart]
tags: [technical-debt, architectural-context, instructional-guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# henriqu3x/mybus — claude-md

**Why it's worth keeping:** It explicitly documents 'notable mismatches' and negative coding patterns (like silent error handling), which helps an AI avoid repeating existing technical debt.

**Summary:** Provides a high-context overview of a Flutter mobile app's tech stack, mission constraints, and architectural patterns.

**Source credibility:** Single-developer repository with structured, likely profile-generated documentation.

**Recency:** Highly current; updated within the last month.

**Source:** [henriqu3x/mybus/CLAUDE.md](https://github.com/henriqu3x/mybus/blob/1ed0a602c149d9f7fe1cfcd53be29a241ecbbe82/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!-- GSD:project-start source:PROJECT.md -->
## Project

**No Ponto**

No Ponto is a mobile urban mobility app focused on public bus transportation. It helps riders inspect nearby and citywide bus stops, see which lines serve each stop, check predicted arrivals, inspect full line itineraries, and plan trips between origin and destination using public transit.

The current product is already a functioning brownfield Flutter app with route planning, maps, notifications, and geolocation flows implemented. The immediate mission is not feature expansion, but making the existing app stable and trustworthy end to end for a first usable release.

**Core Value:** A rider can reliably understand where to board, when the bus should arrive, and how to complete a trip without the app hanging, misleading them, or failing silently.

### Constraints

- **Tech stack**: Flutter and Dart must remain the current implementation path — changing stack is out of scope for this milestone
- **Integrations**: The app depends on the current ETUFOR API and Nominatim-style geocoding — stability must improve without replacing these services wholesale
- **Architecture debt**: Existing flows already work partially
```

</details>
