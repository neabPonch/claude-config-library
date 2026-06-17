---
name: thepictishbeast__PlausiDen-Firewall
source: https://github.com/thepictishbeast/PlausiDen-Firewall/blob/02fa86b06e66db0c56b333a00147e0c18230b890/CLAUDE.md
repo: thepictishbeast/PlausiDen-Firewall
kind: claude-md
stars: 1
last_pushed: 2026-05-17T04:29:05Z
license: other
score: 9
domains: [security, systems-programming, rust]
tags: [architecture-mapping, context-optimization, workflow-enforcement]
curated: 2026-06-15
curated_by: config-scout
---

# thepictishbeast/PlausiDen-Firewall — claude-md

**Why it's worth keeping:** The IMPLEMENTED/SCAFFOLD status tracking is an elite technique to prevent Claude from hallucinating missing logic, while the context-compaction warning optimizes long-running sessions.

**Summary:** Provides a detailed architectural map distinguishing between implemented modules and scaffolds, alongside strict Rust development workflows.

**Source credibility:** Low star count but high technical density indicates a specialized security tool rather than a generic repo.

**Recency:** Highly current; explicitly references Rust 2024 edition and modern development standards.

**Source:** [thepictishbeast/PlausiDen-Firewall/CLAUDE.md](https://github.com/thepictishbeast/PlausiDen-Firewall/blob/02fa86b06e66db0c56b333a00147e0c18230b890/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Instructions for Claude Code

## IMPORTANT: If this is the first message in a session or context was recently compacted, read this entire file before doing anything else. Do not rely on conversation history.

## Project: plausiden-firewall
Application-aware firewall with deep packet inspection, egress filtering, and DNS sinkholing. Designed for state-level adversary threat models.

## Part of the PlausiDen Ecosystem
This repo is part of PlausiDen (PLAUSIbly DENiable) protection suite — AI-powered tools that generate forensically indistinguishable synthetic data, defeating surveillance and forensic overreach. All repos share the same standards.

## Architecture
Single crate with the following modules:
- `rules` — Firewall rule engine with priority ordering and default-deny (IMPLEMENTED)
- `dns_sinkhole` — DNS sinkhole with wildcard support, default blocklist, DoH bypass detection, TLD blocking, punycode/IDN homograph detection (IMPLEMENTED)
- `doh_monitor` — DNS-over-HTTPS connection monitor with browser/non-browser classification (IMPLEMENTED)
- `egress` — Per-application egress filtering with default-deny (IMPLEMENTED)
- `conntrack` — Stateful connection tracking wit
```

</details>
