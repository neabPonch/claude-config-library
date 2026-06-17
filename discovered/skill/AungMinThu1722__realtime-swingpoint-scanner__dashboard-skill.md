---
name: AungMinThu1722__realtime-swingpoint-scanner__dashboard-skill
source: https://github.com/AungMinThu1722/realtime-swingpoint-scanner/blob/88802bb9ff393bf3dc3f1985f70f034f6e52f3d1/DASHBOARD_SKILL.md
repo: AungMinThu1722/realtime-swingpoint-scanner
kind: skill
stars: 0
last_pushed: 2026-06-01T12:44:17Z
license: unknown
score: 7
domains: [automation, cli-tools, devops]
tags: [dashboard, syncing, operational-procedures]
curated: 2026-06-16
curated_by: config-scout
---

# AungMinThu1722/realtime-swingpoint-scanner — skill

**Why it's worth keeping:** It defines exact command-line patterns (including PYTHONPATH requirements) and troubleshooting steps that allow an agent to perform manual system maintenance when automation fails.

**Summary:** Provides operational procedures for manual overrides and synchronization of a trading dashboard using specific CLI commands.

**Source credibility:** Low; the source is a personal project with zero social proof/stars.

**Recency:** Current; utilizes modern GitHub Actions and Vercel workflows.

**Source:** [AungMinThu1722/realtime-swingpoint-scanner/DASHBOARD_SKILL.md](https://github.com/AungMinThu1722/realtime-swingpoint-scanner/blob/88802bb9ff393bf3dc3f1985f70f034f6e52f3d1/DASHBOARD_SKILL.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: realtime-dashboard-automation
description: Maintain and operate the MMXM Alpha Dashboard (Vercel) and its automated GitHub Action sync to GitHub Gist.
---

# MMXM Dashboard & Automation Skill

This skill is for managing the **Live Trading Dashboard** and its **Automated Daily Scanner**.

## Architecture
- **Frontend:** `index.html` (Vercel-ready, Tailwind CSS, Glassmorphism).
- **Automation:** GitHub Action `.github/workflows/scan.yml` (Runs every 15 min).
- **Database:** GitHub Gist (Synced via `sync_to_jsonbin.py` → GitHub Gist API).
- **Logic:** Ported from `forex-chart-scan/` ICT rules.

## Key Operations

### 1. Manual Dashboard Update
Run this to force an update of the Vercel/Gist dashboard:
```bash
export PYTHONPATH=./forex-chart-scan
python3 forex-chart-scan/scripts/sync_to_jsonbin.py
```

### 2. Manual Notion Sync
Run this to push active signals to your Notion database:
```bash
export PYTHONPATH=./forex-chart-scan
python3 forex-chart-scan/scripts/sync_to_notion.py --timeframe 1D
```

### 3. Verify GitHub Actions
Check the **Actions** tab in the `realtime-swingpoint-scanner` repository.
- **Workflow Name:** `Daily MMXM Scan`
- **Schedule:** Every 15 minutes.
- **M
```

</details>
