---
name: stellar__stellar-core__skill
source: https://github.com/stellar/stellar-core/blob/ff61f2e6d639fc6b7906f3c30fa3ca1ffa412a87/.claude/skills/subsystem-summary-of-overlay/SKILL.md
repo: stellar/stellar-core
kind: skill
stars: 3290
last_pushed: 2026-06-13T07:24:50Z
license: other
score: 9
domains: [blockchain, networking, systems-programming]
tags: [architecture-map, system-overview, context-injection]
curated: 2026-06-15
curated_by: config-scout
---

# stellar/stellar-core — skill

**Why it's worth keeping:** It acts as a 'system map' that prevents an agent from wasting tokens on recursive file-crawling by providing high-level structural context upfront.

**Summary:** Provides a dense, hierarchical architectural blueprint of the networking subsystem, mapping files to specific responsibilities and class behaviors.

**Source credibility:** Extremely high; stellar-core is a production-grade, highly-starred blockchain implementation.

**Recency:** Very current, based on recent repository activity.

**Source:** [stellar/stellar-core/.claude/skills/subsystem-summary-of-overlay/SKILL.md](https://github.com/stellar/stellar-core/blob/ff61f2e6d639fc6b7906f3c30fa3ca1ffa412a87/.claude/skills/subsystem-summary-of-overlay/SKILL.md) · 3290★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: subsystem-summary-of-overlay
description: "read this skill for a token-efficient summary of the overlay subsystem"
---

# Overlay Subsystem — Technical Summary

## Overview

The overlay subsystem implements stellar-core's peer-to-peer network layer. It manages TCP connections to other nodes, authenticates peers via ECDH+HMAC, floods broadcast messages (transactions, SCP messages) across the network, fetches missing data (tx sets, quorum sets) via anycast requests, and performs network surveys. The subsystem supports optional background thread processing for I/O-heavy operations (reads/writes on TCP sockets) to keep the main thread responsive.

## Key Files

- **OverlayManager.h / OverlayManagerImpl.h/.cpp** — Central manager; owns peer lists, Floodgate, TxDemandsManager, SurveyManager, PeerManager, PeerAuth, PeerDoor.
- **Peer.h / Peer.cpp** — Abstract base class for a connected peer; handles message dispatch, HMAC auth, flow control, pull-mode adverts.
- **TCPPeer.h / TCPPeer.cpp** — Concrete `Peer` subclass; async TCP read/write via Asio, framing with RFC5531 record marking.
- **FlowControl.h / FlowControl.cpp** — Per-peer flow control for flood traffic; outbound queuin
```

</details>
