---
name: mvanhorn__printing-press-library__skill
source: https://github.com/mvanhorn/printing-press-library/blob/b8126509e276177906cdfe5f353081dbf4dc7d09/cli-skills/pp-instacart/SKILL.md
repo: mvanhorn/printing-press-library
kind: skill
stars: 1598
last_pushed: 2026-06-17T02:31:00Z
license: unknown
score: 9
domains: [e-commerce, cli-tools, agents-ai]
tags: [instacart, shopping, graphql, automation]
curated: 2026-06-17
curated_by: config-scout
---

# mvanhorn/printing-press-library — skill

**Why it's worth keeping:** It includes critical 'verification' steps for the agent and explains complex logic (like history-first vs. live search) so the agent understands its own reliability/latency profile.

**Summary:** A specialized CLI skill that enables agents to manage Instacart carts via GraphQL rather than brittle browser automation.

**Source credibility:** High; large star count (1.5k+) and active maintenance by a known contributor.

**Recency:** Very current, utilizing modern patterns like Chrome MCP for data extraction.

**Source:** [mvanhorn/printing-press-library/cli-skills/pp-instacart/SKILL.md](https://github.com/mvanhorn/printing-press-library/blob/b8126509e276177906cdfe5f353081dbf4dc7d09/cli-skills/pp-instacart/SKILL.md) · 1598★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pp-instacart
description: "Printing Press CLI for Instacart. Natural-language Instacart CLI that talks directly to the web GraphQL API. Add items to your cart, search products, and manage carts across retailers without browser automation. Also caches your purchase history locally so 'add' resolves items you have bought before instead of guessing from live search. Trigger phrases: 'install instacart', 'use instacart', 'run instacart', 'add X to my Safeway cart', 'what did I buy last time', 'order the usual', 'add my regulars to Costco', 'backfill my instacart history', 'sync my instacart orders', 'download my order history', 'save my instacart history locally'."
author: "Matt Van Horn"
license: "Apache-2.0"
argument-hint: "<command> [args] | install cli|mcp | backfill"
allowed-tools: "Read Bash WebFetch"
metadata:
  openclaw:
    requires:
      bins:
        - instacart-pp-cli
    install:
      - kind: go
        bins: [instacart-pp-cli]
        module: github.com/mvanhorn/printing-press-library/library/commerce/instacart/cmd/instacart-pp-cli
---
<!-- GENERATED FILE — DO NOT EDIT.
     This file is a verbatim mirror of library/commerce/instacart/SKILL.md,
     regenerate
```

</details>
