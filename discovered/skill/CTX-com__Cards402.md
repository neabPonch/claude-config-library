---
name: CTX-com__Cards402
source: https://github.com/CTX-com/Cards402/blob/6dcc31ff98dc59cde5a3ea79829d6125ca13b87a/skill.md
repo: CTX-com/Cards402
kind: skill
stars: 5
last_pushed: 2026-06-02T13:52:43Z
license: unknown
score: 8
domains: [finance, cli-tools, agents-ai, blockchain]
tags: [virtual-cards, stellar, crypto-payments]
curated: 2026-06-14
curated_by: config-scout
---

# CTX-com/Cards402 — skill

**Why it's worth keeping:** It includes highly specific troubleshooting logic—like the USDC trustline requirement—that prevents common failures in agentic financial transactions.

**Summary:** Provides an end-to-end operational workflow for agents to manage a Stellar wallet and purchase virtual Visa cards via a CLI.

**Source credibility:** A niche, specialized fintech tool with very recent maintenance activity.

**Recency:** Highly current; uses modern CLI patterns and `npx` execution styles ideal for Claude Code.

**Source:** [CTX-com/Cards402/skill.md](https://github.com/CTX-com/Cards402/blob/6dcc31ff98dc59cde5a3ea79829d6125ca13b87a/skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# cards402 — Virtual Visa Cards for AI Agents

Purchase prepaid Visa virtual cards by paying with XLM or USDC on Stellar.
Cards are delivered in 30–60 seconds.

## What your operator gives you

A single one-shot command — nothing else. It looks like this:

```
Read https://cards402.com/skill.md
and set up this agent by running:

  npx cards402 onboard --claim c402_<48_hex_chars>
```

**No raw API key in the paste.** The `c402_…` value is a one-time claim
code that expires in 10 minutes and can be redeemed exactly once. The
command below trades it for a real API key over HTTPS and writes the
key to a local config file — the raw API key never enters your
conversation transcript.

## Setup — one command

```bash
npx cards402 onboard --claim <code>
```

That's it. Behind the scenes the CLI:

1. `POST`s the claim code to `https://api.cards402.com/v1/agent/claim`.
   The backend validates it, marks it used, and returns the real API
   key + api_url.
2. Writes `~/.cards402/config.json` (chmod 0600) with the API key,
   api_url, and your wallet name. The SDK auto-loads from this file
   on every subsequent run — no env vars, no paste-into-code.
3. Creates (or fetches) an encrypted OWS Stel
```

</details>
