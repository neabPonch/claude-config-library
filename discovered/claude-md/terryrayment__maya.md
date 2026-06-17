---
name: terryrayment__maya
source: https://github.com/terryrayment/maya/blob/2775291807802357030a375c583e0de735a55b93/CLAUDE.md
repo: terryrayment/maya
kind: claude-md
stars: 0
last_pushed: 2026-06-10T19:57:48Z
license: unknown
score: 9
domains: [ecommerce, fullstack-deployment, system-architecture]
tags: [shopify, vercel, nextjs, integration]
curated: 2026-06-16
curated_by: config-scout
---

# terryrayment/maya — claude-md

**Why it's worth keeping:** It includes high-value 'known gotchas' regarding payload requirements and theme synchronization that are critical for system integrity. The inclusion of exact CLI deployment commands makes the instructions highly actionable for an agent.

**Summary:** This configuration maps out a complex split-system architecture between Shopify and Vercel. It clearly defines API boundaries to prevent common integration errors.

**Source credibility:** The extreme specificity of IDs, URLs, and business logic suggests this is a genuine, functioning production file.

**Recency:** Current; utilizes modern Shopify CLI workflows and Next.js patterns.

**Source:** [terryrayment/maya/CLAUDE.md](https://github.com/terryrayment/maya/blob/2775291807802357030a375c583e0de735a55b93/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
@AGENTS.md

---

## MAYA — Architecture & Agent Orientation

### Two separate systems

| System | Domain | What it does |
|---|---|---|
| Shopify storefront | `officeofmaya.com` | All customer-facing pages, cart, checkout, product pages |
| Next.js app (Vercel) | `maya-azure-pi.vercel.app` | API routes only (`/api/quiz-submit`, etc.) |

⚠️ **`officeofmaya.com` is Shopify.** It does NOT serve Next.js routes. Any `fetch()` from the Shopify quiz that targets `officeofmaya.com/api/...` will 404 silently.

The correct API base is: **`https://maya-azure-pi.vercel.app`**

---

### Quiz flow

```
officeofmaya.com/pages/quiz   (Shopify Liquid — shopify-theme/templates/page.quiz.liquid)
  └─ POST /api/quiz-submit    (Vercel Next.js — src/app/api/quiz-submit/route.ts)
       └─ MailerLite API      subscribe with status="active" → group "MAYA Quiz Leads"
            └─ Automation     "MAYA - Quiz Welcome + 10% Off" (ID 185490353957111620)
                 └─ Email 1   "Your dog's MAYA formula — plus 10% off inside" (immediate)
                 └─ Email 2–5 Follow-up sequence over 14 days
```

Critical: `status: "active"` MUST be in the MailerLite POST body. Without it, subscribers land as Unco
```

</details>
