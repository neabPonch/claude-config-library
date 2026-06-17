---
name: trou__rsbkb
source: https://github.com/trou/rsbkb/blob/8f44ce05f0d5389173789bd35bcc29d56d5934c1/SKILL.md
repo: trou/rsbkb
kind: skill
stars: 150
last_pushed: 2026-04-22T19:34:21Z
license: gpl-3.0
score: 9
domains: [security, cli-tools, reverse-engineering]
tags: [binary, data-manipulation, ctf]
curated: 2026-06-15
curated_by: config-scout
---

# trou/rsbkb — skill

**Why it's worth keeping:** The 'Input Model' classification (Stdin vs. File vs. Value) is an elite pattern for preventing agent errors regarding how to pass data to CLI tools.

**Summary:** A highly structured specification for a collection of binary manipulation applets, categorized by their specific input interaction models.

**Source credibility:** Stable project with reasonable star count and recent maintenance.

**Recency:** Very current; highly relevant to modern terminal-centric agent workflows.

**Source:** [trou/rsbkb/SKILL.md](https://github.com/trou/rsbkb/blob/8f44ce05f0d5389173789bd35bcc29d56d5934c1/SKILL.md) · 150★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rsbkb (Rust BlackBag)

description: "Use rsbkb for binary data manipulation, CLI tools: hex unhex urlenc urldec crc16 crc32 crc b64 d64 bofpattoff bofpatt xor entropy slice bgrep findso tsdec tsenc deflate inflate base escape unescape"
---

## Overview
rsbkb is a versatile collection of command-line tools (applets) designed for rapid data transformation and analysis. It functions similarly to `busybox`, where a single binary provides multiple utilities that can be chained together via pipes to perform complex operations, effectively serving as a high-performance CLI alternative to CyberChef.

## Key Capabilities

### Encoding & Decoding
- **Hex**: `hex` (encode), `unhex` (flexible decoding of hex strings and mixed data).
- **Base64**: `b64` (encode), `d64` (decode), with URL-safe support via `-u`.
- **URL**: `urlenc` (encode), `urldec` (decode) with advanced escaping options.

### Binary Analysis & Hacking
- **Search**: `bgrep` for binary pattern matching using hex or regex.
- **Entropy**: `entropy` to calculate Shannon entropy for identifying packed or encrypted data.
- **Exploitation**: `bofpatt` and `bofpattoff` for cyclic pattern generation and offset calculation.
- *
```

</details>
