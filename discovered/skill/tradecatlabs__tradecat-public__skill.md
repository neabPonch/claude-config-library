---
name: tradecatlabs__tradecat-public__skill
source: https://github.com/tradecatlabs/tradecat-public/blob/a9194d4d3d14bb803337ff4c90594846d801efb9/skills/tradecat-public/SKILL.md
repo: tradecatlabs/tradecat-public
kind: skill
stars: 957
last_pushed: 2026-06-03T18:57:01Z
license: mit
score: 9
domains: [agents-ai, cli-tools, fintech, trading]
tags: [paper-trading, market-data, safety-boundaries, api-interfacing]
curated: 2026-06-15
curated_by: config-scout
---

# tradecatlabs/tradecat-public — skill

**Why it's worth keeping:** Uses highly effective 'When to Use' vs 'Not For/Boundaries' sections to enforce strict safety guardrails; provides structured command sequences and validation workflows rather than just single commands.

**Summary:** A high-precision skill definition for an agent-driven paper trading runtime that includes market context auditing and signal analysis.

**Source credibility:** High credibility with 957 stars and active, recent maintenance.

**Recency:** 

**Source:** [tradecatlabs/tradecat-public/skills/tradecat-public/SKILL.md](https://github.com/tradecatlabs/tradecat-public/blob/a9194d4d3d14bb803337ff4c90594846d801efb9/skills/tradecat-public/SKILL.md) · 957★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tradecat-public
description: "TradeCat public Hermes skill: Agent/Hermes paper-trading runtime using public online sheet signals, bundled Binance public-readonly resources, schema-audited context, and local paper/watch execution."
---

# tradecat-public Skill

Use this skill when Hermes/Agent needs to operate TradeCat from the embedded Skill package at `skills/tradecat-public/`. The Python project root is the repository root two levels above this Skill directory; the Skill package provides activation rules, Agent role profiles, references, and the canonical manifest.

## When to Use This Skill

- The task mentions TradeCat public sheet signals, `signal_flow`, `anomaly_panel`, Agent trading loops, paper/watch, paper ledger, replay/backtest, health/daily/alert reports, or autonomous paper ops.
- The task mentions Binance public/read-only Agent market context, K lines, order book, funding, open interest, long/short ratio, context audit, or trade thesis.
- The task needs the Agent machine contract, role profile, safety boundary, Hermes/OpenAI adapter config, or Skill/package governance.

## Not For / Boundaries

- Do not read Binance keys, secrets, listen keys, account state,
```

</details>
