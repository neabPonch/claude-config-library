---
name: revokslab__ShipFree
source: https://github.com/revokslab/ShipFree/blob/8d69f955656433997f863fada876286e0e984cf3/CLAUDE.md
repo: revokslab/ShipFree
kind: claude-md
stars: 1666
last_pushed: 2026-05-25T19:13:09Z
license: mit
score: 9
domains: [web-frontend, fullstack-saas]
tags: [nextjs, bun, drizzle, boilerplate]
curated: 2026-06-15
curated_by: config-scout
---

# revokslab/ShipFree — claude-md

**Why it's worth keeping:** The 'Common Tasks' section offers exact operational procedures, while the 'Important Notes' provide essential guardrails to prevent the agent from breaking core architectural patterns.

**Summary:** This guide provides a deep architectural overview and actionable procedural steps for common development workflows like database migrations and page creation.

**Source credibility:** Highly credible; a popular open-source SaaS boilerplate with recent commits.

**Recency:** Very current, utilizing modern technologies like Bun and TailwindCSS 4.

**Source:** [revokslab/ShipFree/CLAUDE.md](https://github.com/revokslab/ShipFree/blob/8d69f955656433997f863fada876286e0e984cf3/CLAUDE.md) · 1666★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ShipFree - AI Agent Onboarding Guide

## Overview

ShipFree is a production-ready Next.js boilerplate designed to help developers ship startups quickly. It's a free, open-source alternative to ShipFast, built with modern web technologies and best practices.

### Key Characteristics
- **Framework**: Next.js  with App Router
- **Runtime**: Bun (package manager and runtime)
- **Database**: PostgreSQL with Drizzle ORM
- **Authentication**: Better-Auth with multiple OAuth providers
- **Payments**: Multi-provider support (Stripe, Polar, Lemon Squeezy)
- **Email**: Multi-provider support (Resend, Postmark, Plunk, Nodemailer)
- **UI**: TailwindCSS 4, BaseUI components, Shadcn-style patterns
- **Internationalization**: next-intl (i18n) with support for en, es, fr
- **Monitoring**: Sentry integration
- **Storage**: Cloudflare R2 support

## Architecture

### Project Structure

Application code lives under `src/`. The path alias `@/*` maps to `src/*` (e.g. `@/lib/auth` is `src/lib/auth`).

```
ShipFree/
├── src/                    # Application source
│   ├── app/                # Next.js App Router pages and routes
│   │   ├── [locale]/       # Internationalized routes
│   │   │   ├── (aut
```

</details>
