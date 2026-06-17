---
name: vantage-sh__ec2instances.info
source: https://github.com/vantage-sh/ec2instances.info/blob/c3da5af1a8f1e7417764c42b52e532f2da36808e/CLAUDE.md
repo: vantage-sh/ec2instances.info
kind: claude-md
stars: 5725
last_pushed: 2026-06-03T19:27:28Z
license: mit
score: 9
domains: [web-frontend, data-pipeline]
tags: [nextjs, go, vitest, scraper]
curated: 2026-06-15
curated_by: config-scout
---

# vantage-sh/ec2instances.info — claude-md

**Why it's worth keeping:** Excellent prescriptive testing rules that prevent common library misuse and clear documentation of the complex data flow between Go and TypeScript.

**Summary:** Provides comprehensive context for a multi-language project involving Go scrapers and a Next.js frontend.

**Source credibility:** High; well-starred repository with very recent commits.

**Recency:** Very current, referencing cutting-edge versions like React 19 and Tailwind CSS 4.

**Source:** [vantage-sh/ec2instances.info/CLAUDE.md](https://github.com/vantage-sh/ec2instances.info/blob/c3da5af1a8f1e7417764c42b52e532f2da36808e/CLAUDE.md) · 5725★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

EC2Instances.info is a cloud instance comparison website supporting AWS (EC2, RDS, ElastiCache, Redshift, OpenSearch), Azure VMs, and GCP instances. The project consists of:

- **next/**: Next.js 16 frontend (React 19, Tailwind CSS 4, TypeScript)
- **scraper/**: Go-based data scraper for AWS, Azure, and GCP APIs
- **imagegen/**: Go-based OG image generator (outputs to `www/`)
- **www/**: Static output data (instances.json, OG images, compressed variants)

## Common Commands

### Frontend Development (run from `next/` directory)

```bash
nvm use                    # Use correct Node version (.nvmrc specifies v22)
npm ci                     # Install dependencies
npm run init               # Compress data (required before first dev run)
npm run dev                # Start dev server with Turbopack
npm run check-types        # TypeScript type checking
npm run test               # Run Vitest tests
npm run build              # Full build (init + llms + next build)
```

### Formatting (run from root)

```bash
make format                # Run gofmt and p
```

</details>
