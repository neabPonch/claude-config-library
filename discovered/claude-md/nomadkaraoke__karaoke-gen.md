---
name: nomadkaraoke__karaoke-gen
source: https://github.com/nomadkaraoke/karaoke-gen/blob/654e331dd425ace5c780d2c1bafb1050e4ce2147/CLAUDE.md
repo: nomadkaraoke/karaoke-gen
kind: claude-md
stars: 144
last_pushed: 2026-06-16T04:27:19Z
license: mit
score: 9
domains: [cloud-infrastructure, devops, web-service, api-integration]
tags: [production-debugging, iac-pulumi, e2e-testing, i18n]
curated: 2026-06-16
curated_by: config-scout
---

# nomadkaraoke/karaoke-gen — claude-md

**Why it's worth keeping:** It includes 'What Doesn't Work' troubleshooting blocks, detailed i18n translation workflows, and exact command-line recipes for interacting with internal APIs and GCP resources.

**Summary:** A highly operational manual that goes beyond code instructions to provide specific shell commands for production debugging, database access, and infrastructure management.

**Source credibility:** High; a well-structured, active project with clear engineering discipline.

**Recency:** Very current; integrates modern AI/LLM workflows for translations and cloud automation.

**Source:** [nomadkaraoke/karaoke-gen/CLAUDE.md](https://github.com/nomadkaraoke/karaoke-gen/blob/654e331dd425ace5c780d2c1bafb1050e4ce2147/CLAUDE.md) · 144★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Karaoke-Gen AI Assistant Guidelines

## Project Overview

**Karaoke video generation platform** - CLI tool and web service that creates professional karaoke videos with synchronized lyrics.

- **Production**: <https://gen.nomadkaraoke.com> (frontend), <https://api.nomadkaraoke.com> (backend)
- **CLI**: `karaoke-gen` (local), `karaoke-gen-remote` (cloud)
- **Repo**: <https://github.com/nomadkaraoke/karaoke-gen>

## Quick Reference

| What | Where |
|------|-------|
| Product vision & goals | `docs/PRODUCT-VISION.md` |
| Current status | `docs/README.md` |
| Architecture | `docs/ARCHITECTURE.md` |
| Dev setup & testing | `docs/DEVELOPMENT.md` |
| **Testing & code quality** | `docs/TESTING.md` |
| API reference | `docs/API.md` |
| Past learnings | `docs/LESSONS-LEARNED.md` |
| **Operational runbooks** | `docs/TROUBLESHOOTING.md` |
| GDrive validator & gaps | `docs/GDRIVE-VALIDATOR.md` |
| **Product communication** | `docs/PRODUCT-COMMUNICATION-GUIDE.md` |
| Brand style guide | `docs/BRAND-STYLE-GUIDE.md` |

## Tech Stack

- **Backend**: FastAPI on Cloud Run, Firestore, GCS, Secret Manager
- **Frontend**: Next.js on Cloudflare Pages
- **Processing**: Cloud Run GPU (L4 audio separatio
```

</details>
