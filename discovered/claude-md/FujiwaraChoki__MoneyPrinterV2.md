---
name: FujiwaraChoki__MoneyPrinterV2
source: https://github.com/FujiwaraChoki/MoneyPrinterV2/blob/5192af8eca97759f941834b947e3ceb209da0649/CLAUDE.md
repo: FujiwaraChoki/MoneyPrinterV2
kind: claude-md
stars: 30928
last_pushed: 2026-06-14T08:36:16Z
license: agpl-3.0
score: 9
domains: [cli-tools, automation, python]
tags: [python-cli, architecture-deep-dive, path-context]
curated: 2026-06-15
curated_by: config-scout
---

# FujiwaraChoki/MoneyPrinterV2 — claude-md

**Why it's worth keeping:** It explicitly explains the `sys.path` manipulation logic to prevent import errors and detailes a clear provider pattern for service dispatching.

**Summary:** A highly detailed project guide that provides architectural context and critical execution-environment nuances.

**Source credibility:** High; from a very popular repository (30k+ stars) with recent activity.

**Recency:** Very current, utilizing Python 3.12 and modern LLM/automation stacks.

**Source:** [FujiwaraChoki/MoneyPrinterV2/CLAUDE.md](https://github.com/FujiwaraChoki/MoneyPrinterV2/blob/5192af8eca97759f941834b947e3ceb209da0649/CLAUDE.md) · 30928★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

MoneyPrinterV2 (MPV2) is a Python 3.12 CLI tool that automates four online workflows:
1. **YouTube Shorts** — generate video (LLM script → TTS → images → MoviePy composite) and upload via Selenium
2. **Twitter/X Bot** — generate and post tweets via Selenium
3. **Affiliate Marketing** — scrape Amazon product info, generate pitch, share on Twitter
4. **Local Business Outreach** — scrape Google Maps (Go binary), extract emails, send cold outreach via SMTP

There is no web UI, no REST API, no test suite, no CI, and no linting config.

## Running the Application

```bash
# First-time setup
cp config.example.json config.json   # then fill in values
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt

# macOS quick setup (auto-configures Ollama, ImageMagick, Firefox profile)
bash scripts/setup_local.sh

# Preflight check (validates services are reachable)
python scripts/preflight_local.py

# Run
python src/main.py
```

The app **must** be run from the project root. `python src/main.py` adds `src/` to `sys.path`, so all import
```

</details>
