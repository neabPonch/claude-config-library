---
name: kosukesaigusa__geoflutterfire_plus
source: https://github.com/kosukesaigusa/geoflutterfire_plus/blob/f8bb6b8435fda88ff8a8076ee5454a1183448b4d/CLAUDE.md
repo: kosukesaigusa/geoflutterfire_plus
kind: claude-md
stars: 65
last_pushed: 2026-03-06T19:34:28Z
license: mit
score: 8
domains: [mobile-development, flutter, database]
tags: [dart, firestore, geospatial]
curated: 2026-06-15
curated_by: config-scout
---

# kosukesaigusa/geoflutterfire_plus — claude-md

**Why it's worth keeping:** The 'Common Operations' section provides high-value, actionable code snippets that teach the AI how to use the core API correctly. The explicit directory tree is essential for efficient file navigation without constant searching.

**Summary:** Provides a comprehensive technical map of the project including directory structure, dependencies, and actual code implementation patterns.

**Source credibility:** High; it is a well-maintained, specialized Flutter package with a clear purpose and active history.

**Recency:** Current; updated within the last few months.

**Source:** [kosukesaigusa/geoflutterfire_plus/CLAUDE.md](https://github.com/kosukesaigusa/geoflutterfire_plus/blob/f8bb6b8435fda88ff8a8076ee5454a1183448b4d/CLAUDE.md) · 65★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# geoflutterfire_plus Project Guide

## Project Overview

This is **geoflutterfire_plus**, a Flutter package that enables geographic queries on Cloud Firestore documents. It's a redesigned fork of GeoFlutterFire with modern Flutter/Dart support and additional features.

### Key Information

- **Package**: geoflutterfire_plus
- **Language**: Dart/Flutter
- **Purpose**: Geographic data storage and querying for Cloud Firestore
- **Repository**: <https://github.com/KosukeSaigusa/geoflutterfire_plus>
- **License**: MIT

## Technical Stack

### Dependencies

- **cloud_firestore** (Core Firestore integration)
- **rxdart** (Reactive programming)
- **flutter** (UI framework - SDK)

### Development Dependencies

- **build_runner** (Code generation)
- **mockito** (Testing mocks)
- **flutter_test** (Testing framework - SDK)

### SDK Requirements

- **Dart**: >=2.17.0 <4.0.0
- **Flutter**: >=2.10.0

## Project Structure

```bash
lib/
├── geoflutterfire_plus.dart          # Main library export
└── src/
    ├── geo_collection_reference.dart  # Collection reference with geo queries
    ├── geo_fire_point.dart           # Geographic point representation
    ├── math.dart                     # Mathe
```

</details>
