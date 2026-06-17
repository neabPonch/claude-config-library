---
name: yuandrk__actual-csv-transformer
source: https://github.com/yuandrk/actual-csv-transformer/blob/9a6fc96f22de87f45f1d8994c43fd75dc3f29e6f/claude.md
repo: yuandrk/actual-csv-transformer
kind: claude-md
stars: 0
last_pushed: 2026-02-08T16:41:46Z
license: mit
score: 9
domains: [backend-api, data-engineering, devops]
tags: [fastapi, etl, financial-logic, kubernetes]
curated: 2026-06-15
curated_by: config-scout
---

# yuandrk/actual-csv-transformer — claude-md

**Why it's worth keeping:** It explicitly highlights 'Critical Transformation Logic' (like sign flipping) which prevents AI from making common logical errors in financial data processing; it also maps key files to their specific functional roles.

**Summary:** A high-context instruction file for an ETL service that prioritizes critical domain-specific business rules over boilerplate.

**Source credibility:** Low GitHub social proof, but the technical depth and structure suggest a highly disciplined author.

**Recency:** Highly current, matching modern Python/FastAPI/K8s patterns.

**Source:** [yuandrk/actual-csv-transformer/claude.md](https://github.com/yuandrk/actual-csv-transformer/blob/9a6fc96f22de87f45f1d8994c43fd75dc3f29e6f/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Code Instructions - ActualBudget CSV Transformer

## Project Overview

This is a **production-ready, privacy-first FastAPI service** that transforms Nationwide UK CSV bank exports into ActualBudget's CSV import format. It's designed for self-hosted deployment on k3s Kubernetes clusters.

**Key Purpose:** Convert Nationwide UK bank statements to a format that ActualBudget can import, with automatic encoding detection, date conversion, amount sign flipping, payee normalization, category assignment, and duplicate detection.

## Tech Stack

- **Backend:** Python 3.11+ with FastAPI
- **Build System:** Hatchling (pyproject.toml)
- **Container:** Multi-stage Docker builds (distroless/slim base)
- **Orchestration:** Kubernetes (k3s optimized) with Helm charts
- **CI/CD:** GitHub Actions
- **GitOps:** FluxCD support
- **Database:** SQLite (default) or PostgreSQL for deduplication
- **Storage:** Local PersistentVolume or S3/MinIO

## Project Structure

```
.
├── app/                          # FastAPI application
│   ├── core/                     # Core modules
│   │   ├── config.py             # Pydantic settings (env vars)
│   │   ├── logging.py            # Structured JSON loggin
```

</details>
