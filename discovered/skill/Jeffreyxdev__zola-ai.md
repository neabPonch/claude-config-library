---
name: Jeffreyxdev__zola-ai
source: https://github.com/Jeffreyxdev/zola-ai/blob/de06c7b74491a9d21a9ae5e0ea278ab007f106f3/SKILL.MD
repo: Jeffreyxdev/zola-ai
kind: skill
stars: 3
last_pushed: 2026-03-12T21:02:32Z
license: unknown
score: 8
domains: [agents-ai, security, blockchain, backend]
tags: [solana, tool-calling, encryption, autonomous-agent]
curated: 2026-06-14
curated_by: config-scout
---

# Jeffreyxdev/zola-ai — skill

**Why it's worth keeping:** Provides highly specific patterns for 'Zero AI Exposure' (passing transaction results instead of keys to the LLM) and context injection of environment state into agent loops.

**Summary:** A technical architecture document for an autonomous Solana agent using Gemini 2.0 with native tool calling and secure, non-custodial key handling.

**Source credibility:** Hackathon project with 3 stars; demonstrates real-world implementation complexity.

**Recency:** Current; written within the last 3 months using modern LLM tool-calling logic.

**Source:** [Jeffreyxdev/zola-ai/SKILL.MD](https://github.com/Jeffreyxdev/zola-ai/blob/de06c7b74491a9d21a9ae5e0ea278ab007f106f3/SKILL.MD) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Zola AI — Technical Skills & Architecture

> **Hackathon Judges**: This document covers Zola AI's core technical achievements, architecture decisions, and the cluster-switching system. Live demo: [use-zola.vercel.app/](https://use-zola.vercel.app/)

---

##  Hackathon Focus: Telegram vs. Twitter

While Zola is designed as a multi-platform autonomous DeFi agent, **our primary focus for this hackathon was the Telegram integration**.

- **Telegram (`telegram_bot.py`)**: Fully implemented, rigorously tested, and serves as our primary interactive interface. Features secure deep-linking, a `/connect` flow that auto-deletes sensitive messages, and full agentic execution.
- **Twitter (`twitter_bot.py`)**: Fully functional in code. Uses a robust Tweepy v2 polling engine and shares the *exact same* Gemini agentic execution pipeline as Telegram. Currently untested live due to pending Twitter Developer API credits — the architecture guarantees identical behaviour to Telegram once credits are applied.

the core ai engine has 2 main agents one for security and the other for onchain executions what work hand in hand simultaneously
---

##  1. Agentic AI Integration (Gemini 2.0 Flash Lite)

We m
```

</details>
