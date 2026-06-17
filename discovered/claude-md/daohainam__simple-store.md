---
name: daohainam__simple-store
source: https://github.com/daohainam/simple-store/blob/eaffa4f9196a3d390b38ce61e5a0e3862ff2b5b1/CLAUDE.md
repo: daohainam/simple-store
kind: claude-md
stars: 43
last_pushed: 2026-06-07T20:44:42Z
license: mit
score: 9
domains: [backend-api, microservices, distributed-systems, .net]
tags: [event-driven, saga-pattern, architecture-map, mass-transit]
curated: 2026-06-15
curated_by: config-scout
---

# daohainam/simple-store — claude-md

**Why it's worth keeping:** It excels at explaining cross-service side effects (Sagas/MassTransit) and how individual changes impact the entire event-driven flow. The inclusion of a migration changelog provides vital 'intent' context for architectural shifts.

**Summary:** A high-density architectural blueprint mapping a distributed microservices ecosystem including data ownership, event choreography, and security patterns.

**Source credibility:** Highly credible; maintained recently with highly specific, non-generic technical descriptions of a complex .NET stack.

**Recency:** Extremely current, referencing .NET 10 and recent rebranding (KurrentDB) from 2025.

**Source:** [daohainam/simple-store/CLAUDE.md](https://github.com/daohainam/simple-store/blob/eaffa4f9196a3d390b38ce61e5a0e3862ff2b5b1/CLAUDE.md) · 43★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

SimpleStore is a small e-commerce sample built on **.NET 10** and orchestrated with **.NET Aspire**. The monolith → microservices migration is now complete:

- **Catalog** is a standalone minimal-WebApi service (`SimpleStore.Catalog.API`) that owns `catalogdb` (Postgres). Storefront browsing is anonymous; admin write endpoints require a JWT with the `Admin` role.
- **Identity** (`SimpleStore.Identity.API`) owns `identitydb` (Postgres) and issues JWT bearer tokens (HS256) plus refresh tokens. Web and Admin call it over HTTP for register/login/passkey/profile.
- **Order** (`SimpleStore.Order.API`) owns `orderdb` (Postgres). Storefront endpoints (`/api/v1/order/orders`) require the caller's JWT; admin endpoints (`/api/v1/order/admin/...`) require the `Admin` role.
- **Cart** (`SimpleStore.Cart.API`) is backed by **Redis** (`cart-redis`). It is the first non-DB-backed microservice. Anonymous browsers identify a cart with the opaque `ss_cart` HttpOnly cookie issued by `SimpleStore.Web`, which it passes to Cart.API as the `X-Cart-Id` header; authenticated call
```

</details>
