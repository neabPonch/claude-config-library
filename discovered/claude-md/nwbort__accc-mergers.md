---
name: nwbort__accc-mergers
source: https://github.com/nwbort/accc-mergers/blob/56e06cb0a76fdbc666233cec18cb8defdf0ae355/claude.md
repo: nwbort/accc-mergers
kind: claude-md
stars: 1
last_pushed: 2026-06-13T23:42:16Z
license: mit
score: 9
domains: [web-frontend, data-pipeline, devops]
tags: [react, python, scraping, static-site]
curated: 2026-06-14
curated_by: config-scout
---

# nwbort/accc-mergers — claude-md

**Why it's worth keeping:** The explicit 'Key Data Flow' and specific command suites for different sub-systems provide the exact context an agent needs to understand side effects in complex pipelines.

**Summary:** A highly detailed technical breakdown of a multi-stage data pipeline integrated with a React frontend.

**Source credibility:** High; active repository with recent maintenance.

**Recency:** 

**Source:** [nwbort/accc-mergers/claude.md](https://github.com/nwbort/accc-mergers/blob/56e06cb0a76fdbc666233cec18cb8defdf0ae355/claude.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# ACCC Merger Tracker

A public-facing web application for tracking Australian Competition and Consumer Commission (ACCC) merger reviews. Live at https://mergers.fyi.

## Architecture

Fully static — no backend server. Cloudflare Pages serves the React SPA plus generated JSON data files. Data is refreshed via GitHub Actions (hourly scrapes, daily extraction) which commit updated JSON files, triggering auto-deploy.

### Frontend (`merger-tracker/frontend/`)

- **React 19** SPA with **React Router 7** for client-side routing
- **Vite 7** build tool, **Tailwind CSS 3** for styling
- **Chart.js 4** for data visualizations
- **date-fns 4** for date manipulation
- Static JSON files in `public/data/` serve as the "API"

### Data Pipeline (`scripts/`)

- **Python 3.10** scripts for scraping, extracting, and generating data
- `scrape.sh` → `extract_mergers.py` → `generate_static_data.py`
- Dependencies: beautifulsoup4, requests, pdfplumber, markdownify

### Cloudflare Worker (`cloudflare-worker/`)

- Handles digest email signup form submissions
- Validates Cloudflare Turnstile tokens
- Deployed separately via wrangler

## Project Structure

```
merger-tracker/frontend/src/
├── main.jsx
```

</details>
