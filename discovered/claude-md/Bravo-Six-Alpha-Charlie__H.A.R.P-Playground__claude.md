---
name: Bravo-Six-Alpha-Charlie__H.A.R.P-Playground__claude
source: https://github.com/Bravo-Six-Alpha-Charlie/H.A.R.P-Playground/blob/3ee5d70587a29c415bf069814fe6727525b27314/tasks/alex/Claude.md
repo: Bravo-Six-Alpha-Charlie/H.A.R.P-Playground
kind: claude-md
stars: 1
last_pushed: 2026-03-07T23:27:54Z
license: unknown
score: 9
domains: [signal-processing, machine-learning, geospatial]
tags: [RF-classification, trilateration, real-time-tracking]
curated: 2026-06-15
curated_by: config-scout
---

# Bravo-Six-Alpha-Charlie/H.A.R.P-Playground — claude-md

**Why it's worth keeping:** Includes exact feature engineering math, JSON schemas, and geometric algorithms (trilateration) that prevent AI hallucination in complex domain tasks.

**Summary:** A high-density technical specification for a signal processing and geolocation pipeline. It provides the mathematical foundation, data schemas, and algorithmic logic required to build the system.

**Source credibility:** High technical density suggests a specialized engineer/researcher, though social proof is low due to hackathon origin.

**Recency:** Very current; written for a 2026 event context and uses modern Pythonic implementations.

**Source:** [Bravo-Six-Alpha-Charlie/H.A.R.P-Playground/tasks/alex/Claude.md](https://github.com/Bravo-Six-Alpha-Charlie/H.A.R.P-Playground/blob/3ee5d70587a29c415bf069814fe6727525b27314/tasks/alex/Claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Find My Force — Claude Code Instructions

## Project Overview

RF Classification, Geolocation & Tactical Awareness system for a hackathon (March 7, 2026).
Build a pipeline that classifies RF emitters, geolocates them from multi-receiver observations,
and displays the tactical picture on a Common Operating Picture (COP).

**Event:** 8:30 AM – 7:30 PM | Build time: 9:55 AM – 4:00 PM

---

## Architecture

```
Training IQ Data + Live Simulation Feed + Receiver Config
        ↓
Signal Classifier (ML)        ← classify each IQ snapshot
        ↓
Observation Association       ← group observations from same emitter
        ↓
Geolocation Engine            ← trilaterate position from RSSI/TDoA
        ↓
Track Manager                 ← persist + update emitter tracks over time
        ↓
Common Operating Picture      ← interactive map (Leaflet/Mapbox)
```

---

## Data Formats

### IQ Snapshot (256-element float32 vector)
- Elements 0–127: I (in-phase) components
- Elements 128–255: Q (quadrature) components
- Sample rate: 10 MS/s → 12.8 µs snapshot
- SNR range: -20 dB to +18 dB

### Simulation Feed Observation (JSON)
```json
{
  "observation_id": "string",
  "timestamp": "ISO 8601",
  "rec
```

</details>
