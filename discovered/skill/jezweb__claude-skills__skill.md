---
name: jezweb__claude-skills__skill
source: https://github.com/jezweb/claude-skills/blob/0aa0f4437e0e70dda1e4e62df3a9d9cb8170f8ba/plugins/integrations/skills/stripe-payments/SKILL.md
repo: jezweb/claude-skills
kind: skill
stars: 858
last_pushed: 2026-06-11T13:18:31Z
license: mit
score: 9
domains: [backend-api, payments, fullstack]
tags: [stripe, webhooks, subscriptions, cloudflare]
curated: 2026-06-15
curated_by: config-scout
---

# jezweb/claude-skills — skill

**Why it's worth keeping:** Includes a strategic API decision matrix and addresses environment-specific pitfalls like Cloudflare Workers' requirement for constructEventAsync.

**Summary:** A comprehensive technical blueprint for integrating Stripe payments, covering one-time payments, subscriptions, and webhook verification.

**Source credibility:** High; part of a highly starred, frequently updated repository specifically designed for Claude Code skills.

**Recency:** Highly current, including modern deployment patterns for Cloudflare/Wrangler and Tailwind v4 context.

**Source:** [jezweb/claude-skills/plugins/integrations/skills/stripe-payments/SKILL.md](https://github.com/jezweb/claude-skills/blob/0aa0f4437e0e70dda1e4e62df3a9d9cb8170f8ba/plugins/integrations/skills/stripe-payments/SKILL.md) · 858★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: stripe-payments
description: "Add Stripe payments to a web app — Checkout Sessions, Payment Intents, subscriptions, webhooks, customer portal, and pricing pages. Covers the decision of which Stripe API to use, produces working integration code, and handles webhook verification. No MCP server needed — uses Stripe npm package directly. Triggers: 'add payments', 'stripe', 'checkout', 'subscription', 'payment form', 'pricing page', 'billing', 'accept payments', 'stripe webhook', 'customer portal'."
compatibility: claude-code-only
allowed-tools:
  - Read
  - Write
  - Edit
  - Bash
  - Glob
  - Grep
---

# Stripe Payments

Add Stripe payments to a web app. Covers the common patterns — one-time payments, subscriptions, webhooks, customer portal — with working code. No MCP server needed.

## Which Stripe API Do I Need?

| You want to... | Use | Complexity |
|----------------|-----|-----------|
| Accept a one-time payment | Checkout Sessions | Low — Stripe hosts the payment page |
| Embed a payment form in your UI | Payment Element + Payment Intents | Medium — you build the form, Stripe handles the card |
| Recurring billing / subscriptions | Checkout Sessions (subscription mode)
```

</details>
