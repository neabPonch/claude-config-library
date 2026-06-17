---
name: g41797__tofu__libevent-evaluation-claude
source: https://github.com/g41797/tofu/blob/0e61fdbb8f41b8e6a1666eea5de29692f78abf98/design/libevent-evaluation-claude.md
repo: g41797/tofu
kind: claude-md
stars: 28
last_pushed: 2026-06-07T11:14:38Z
license: mit
score: 9
domains: [systems-programming, networking, architecture]
tags: [contract-definition, invariants, backend-api]
curated: 2026-06-16
curated_by: config-scout
---

# g41797/tofu — claude-md

**Why it's worth keeping:** It provides exact function signatures, ASCII logic diagrams, and explicit memory stability requirements that prevent implementers from violating system-level constraints.

**Summary:** A technical specification defining the rigorous interface contract and runtime invariants required for an asynchronous networking backend.

**Source credibility:** High-density architectural analysis of a Zig/C systems project.

**Recency:** Current (2026 future-dated context).

**Source:** [g41797/tofu/design/libevent-evaluation-claude.md](https://github.com/g41797/tofu/blob/0e61fdbb8f41b8e6a1666eea5de29692f78abf98/design/libevent-evaluation-claude.md) · 28★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Evaluation: libevent as a Long-Term Networking Backend for tofu on Zig 0.16

**Date:** 2026-06-03
**Author:** Claude (Opus 4.7)
**Subject repos:**

* `tofu` — `/home/g41797/dev/root/github.com/g41797/tofu`
* `uSockets` fork — `/home/g41797/dev/root/github.com/g41797/uSockets`
* `libevent` — `/home/g41797/Downloads/libevent-master/`

**Scope:** architectural suitability, maintenance cost, feature coverage, implementation effort. **Not** a benchmark.

---

## 1. Executive Summary

libevent **can** implement the current tofu backend contract. The fit is good but
not perfect, and the migration cost is real because the impedance mismatch lives
not in *polling* (which is a clean swap) but in *socket-level wrappers*
(`bsd_send`/`bsd_recv`/`bsd_create_listen_socket`) that the posixnet backend
currently reuses from the uSockets fork.

### 1.1 Central fact: libevent is a polling library, not a sockets library

**libevent provides only event-loop and readiness-notification abstractions.**
It performs no socket I/O on the user's behalf. Every socket operation —
`create`, `bind`, `listen`, `accept`, `connect`, `send`, `recv`, `close`,
`setsockopt`, address parsing, DNS resolution, errno handl
```

</details>
