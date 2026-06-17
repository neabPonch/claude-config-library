---
name: Outlier1217__quilvion-multichain-testnet__ai-skill
source: https://github.com/Outlier1217/quilvion-multichain-testnet/blob/f80c90a0b2297f8f37e6a17631ac67754c47058e/AI-Skill.md
repo: Outlier1217/quilvion-multichain-testnet
kind: skill
stars: 5
last_pushed: 2026-06-08T04:39:34Z
license: apache-2.0
score: 8
domains: [agents-ai, backend-api, web3]
tags: [prompt-engineering, risk-management, agentic-orchestration]
curated: 2026-06-16
curated_by: config-scout
---

# Outlier1217/quilvion-multichain-testnet — skill

**Why it's worth keeping:** It provides highly specific system prompt constraints (sentence counts, tone, and output formatting) essential for predictable UI integration. The pattern of mapping raw data (XGBoost scores) to structured human explanations is an excellent template for agentic reasoning.

**Summary:** This document defines a dual-agent architecture separating high-speed ML risk scoring from LLM-driven natural language features for a Web3 marketplace.

**Source credibility:** High; documented as a functional part of an active, specialized Web3 project with 5 stars.

**Recency:** Current; utilizes modern models like LLaMA 3.3.

**Source:** [Outlier1217/quilvion-multichain-testnet/AI-Skill.md](https://github.com/Outlier1217/quilvion-multichain-testnet/blob/f80c90a0b2297f8f37e6a17631ac67754c47058e/AI-Skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AGENTS.md — Quilvion AI Agent System

This document describes the AI agents, models, and autonomous decision systems integrated into the Quilvion Web3 commerce platform. It is intended for developers, auditors, and investors who need to understand how AI is used across the stack.

---

## Overview

Quilvion uses two distinct AI systems that operate independently and serve different purposes:

| System | Model | Latency | Purpose |
|---|---|---|---|
| Fraud Detection | XGBoost (ML) | ~50ms | Risk scoring on every purchase |
| Language Model | Groq LLaMA 3.3 70B | ~1–2s | Explanations, chat, generation |

These systems are intentionally separated. The ML model produces a score in milliseconds before the LLM explanation loads — buyers see the risk level immediately without waiting for language generation.

---

## Agent 1 — Fraud Detection (XGBoost)

### What it does

Every time a buyer attempts a purchase, this agent runs before the wallet signs the transaction. It produces a risk score from 0 to 100 and triggers one of three automated actions based on the result.

### Inputs

```json
{
  "order_id": "string",
  "buyer_wallet": "0x...",
  "merchant_wallet": "0x...",
  "amount_usdc"
```

</details>
