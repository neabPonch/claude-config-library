---
name: m-deane__weather-forecast-alerts
source: https://github.com/m-deane/weather-forecast-alerts/blob/63ecc5e5f83d4f2febec51d757dfccc1f433510c/claude.md
repo: m-deane/weather-forecast-alerts
kind: claude-md
stars: 0
last_pushed: 2026-06-14T20:59:07Z
license: unknown
score: 9
domains: [full-stack, data-scraping, web-development]
tags: [fastapi, react, python, docker, scraper]
curated: 2026-06-16
curated_by: config-scout
---

# m-deane/weather-forecast-alerts — claude-md

**Why it's worth keeping:** Excellent use of data flow diagrams, detailed command hierarchies for different dev modes, and explicit inclusion of business logic (scoring algorithms) to provide semantic context.

**Summary:** Provides a comprehensive blueprint for a multi-service architecture including scraping, backend API, and frontend layers.

**Source credibility:** Low star count suggests a personal project, but the document structure is professionally engineered.

**Recency:** Highly current, utilizing modern stacks like Vite, React 18, and FastAPI.

**Source:** [m-deane/weather-forecast-alerts/claude.md](https://github.com/m-deane/weather-forecast-alerts/blob/63ecc5e5f83d4f2febec51d757dfccc1f433510c/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A full-stack Scottish Mountain Weather application that scrapes weather forecasts from mountain-forecast.com and OpenWeatherMap, calculates hiking suitability scores, and presents data through a React-based web interface.

**Architecture**: Full-stack web application with Python backend (FastAPI) and React/TypeScript frontend
**Primary Language**: Python (scraper/backend), TypeScript/React (frontend)

## Quick Development Commands

### Weather Scraper (Core functionality)
```bash
# Run the main weather scraper
python weather_scraper.py

# Check URL validity for mountain-forecast.com
python check_urls.py
```

### Backend API

**Simple Mock API** (for quick testing):
```bash
cd backend
python simple_api.py
# Runs on http://localhost:8000
```

**Full Production API** (requires database):
```bash
cd backend

# First-time setup
pip install -r requirements.txt

# Initialize database (requires Docker Compose services)
python -c "from database import startup_database; startup_database()"

# Run API
python main.py
```

### Frontend

```bash
cd frontend

#
```

</details>
