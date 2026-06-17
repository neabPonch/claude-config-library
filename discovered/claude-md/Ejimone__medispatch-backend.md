---
name: Ejimone__medispatch-backend
source: https://github.com/Ejimone/medispatch-backend/blob/861115c845c0df5db11dbc06a9aba0a5a140c2a5/Claude.md
repo: Ejimone/medispatch-backend
kind: claude-md
stars: 0
last_pushed: 2026-03-10T04:13:49Z
license: unknown
score: 9
domains: [backend-api, security, django]
tags: [multi-tenancy, state-machine, django-rest-framework]
curated: 2026-06-16
curated_by: config-scout
---

# Ejimone/medispatch-backend — claude-md

**Why it's worth keeping:** Includes critical 'Never' rules for security (UUIDs, hospital_id scoping) and defines an explicit state machine for visit transitions to prevent logic errors.

**Summary:** A highly prescriptive set of guardrails for a multi-tenant Django backend that focuses on security boundaries and business logic integrity.

**Source credibility:** Single developer project; value lies in the highly detailed technical constraints rather than social proof.

**Recency:** Highly current; utilizes modern patterns optimized for AI agent-driven development.

**Source:** [Ejimone/medispatch-backend/Claude.md](https://github.com/Ejimone/medispatch-backend/blob/861115c845c0df5db11dbc06a9aba0a5a140c2a5/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MedDispatch — Claude Code Instructions

> This file is the single source of truth for Claude Code working on the MedDispatch backend.
> Read this fully before writing any code. Re-read ARCHITECTURE.md and SKILLS.md as needed.
> Follow STAGES.md for sequenced build order. Never skip a stage.

---

## What Is MedDispatch?

MedDispatch is a three-sided home healthcare dispatch platform.

- **Hospitals** sign up and manage their nurses and patients via a dashboard
- **Nurses** (hospital-assigned only) receive visit assignments pushed to them
- **Patients** request home medical visits, track their nurse, and pay for the service

The flow: Patient requests visit → Hospital coordinator assigns a nurse manually → Nurse executes visit → Patient pays via Paystack or cash → Visit closed.

---

## Project Stack

| Layer | Technology |
|-------|-----------|
| Language | Python 3.11+ |
| Framework | Django 5.x + Django REST Framework |
| Database | PostgreSQL (ONLY — no MongoDB, no SQLite in any env) |
| Auth | JWT via djangorestframework-simplejwt (custom multi-role backend) |
| Push Notifications | Firebase Admin SDK (FCM) |
| Payments | Paystack API + webhooks |
| File Storage | AWS S3 via
```

</details>
