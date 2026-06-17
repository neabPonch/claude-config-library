---
name: MrWillingten__house-of-paradise__claude-backup
source: https://github.com/MrWillingten/house-of-paradise/blob/a7928ef8a42174d75aecad0ffa484a03ac28b68c/CLAUDE.md.backup
repo: MrWillingten/house-of-paradise
kind: claude-md
stars: 0
last_pushed: 2025-12-19T11:09:38Z
license: unknown
score: 9
domains: [backend-api, microservices, devops, security]
tags: [polyglot, docker, kubernetes, api-gateway, spring-boot]
curated: 2026-06-16
curated_by: config-scout
---

# MrWillingten/house-of-paradise — claude-md

**Why it's worth keeping:** The specific ordering of security middleware and structured 'Common Development Scenarios' provide high-fidelity instructions that prevent an AI from breaking critical logic during refactoring.

**Summary:** A comprehensive architectural blueprint for a polyglot microservices system that includes orchestration, deployment, and operational commands.

**Source credibility:** Low social proof (0 stars), but the technical depth suggests a high-quality personal or educational project.

**Recency:** Recent enough (6 months) to be highly relevant to current Claude Code workflows.

**Source:** [MrWillingten/house-of-paradise/CLAUDE.md.backup](https://github.com/MrWillingten/house-of-paradise/blob/a7928ef8a42174d75aecad0ffa484a03ac28b68c/CLAUDE.md.backup) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a polyglot microservices-based travel booking platform with hotel, trip, payment, and authentication services, orchestrated using Docker Compose and Kubernetes. The system uses an API Gateway pattern with comprehensive security middleware.

## Architecture

### Service Layer (Polyglot Implementation)
- **API Gateway** (Node.js/Express, Port 8080): Unified entry point with extensive security middleware (DDoS protection, rate limiting, XSS/injection protection)
- **Hotel Service** (Node.js/Express, Port 3001): Hotel CRUD, booking management, real-time updates via Socket.IO, loyalty rewards, personalization
- **Trip Service** (Java Spring Boot, Port 3002): Trip/journey management using JPA with PostgreSQL
- **Payment Service** (Python FastAPI, Port 3003): Payment processing with SQLAlchemy
- **Auth Service** (Node.js/Express, Port 3004): JWT-based authentication with MFA support
- **Frontend** (React, Port 3000): SPA with React Router, proxies to API Gateway

### Data Layer
- **MongoDB** (Port 27017): Used by Hotel Service (`hoteldb`) and Au
```

</details>
