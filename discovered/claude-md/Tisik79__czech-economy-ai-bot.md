---
name: Tisik79__czech-economy-ai-bot
source: https://github.com/Tisik79/czech-economy-ai-bot/blob/6b6904e9c54f0bc4cb6fb7d7d00a5bdf663263d3/Claude.md
repo: Tisik79/czech-economy-ai-bot
kind: claude-md
stars: 0
last_pushed: 2025-06-25T15:33:36Z
license: unknown
score: 8
domains: [agents-ai, content-automation, web-scraping]
tags: [agentic-workflow, structured-prompts, modular-design]
curated: 2026-06-14
curated_by: config-scout
---

# Tisik79/czech-economy-ai-bot — claude-md

**Why it's worth keeping:** It uses strict line-count constraints to enforce modularity and provides concrete, production-ready prompt engineering patterns for social media distribution.

**Summary:** A highly structured blueprint for an AI content agent that includes detailed module specs, scoring criteria, and platform-specific prompt templates.

**Source credibility:** Low (0 stars/unknown license), but the technical depth indicates a high-quality implementation plan.

**Recency:** 12 months old; the structural pattern remains highly effective for current agentic workflows.

**Source:** [Tisik79/czech-economy-ai-bot/Claude.md](https://github.com/Tisik79/czech-economy-ai-bot/blob/6b6904e9c54f0bc4cb6fb7d7d00a5bdf663263d3/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Czech Economy AI Bot - Claude Code Instructions

## Přehled projektu
AI aplikace pro automatické generování příspěvků o české ekonomice. Každé ráno v 9:00 projde zajímavé články o ekonomice ČR, vybere nejzajímavější a vytvoří z něj příspěvek na sociální síť.

## Architektura projektu
```
czech-economy-ai-bot/
├── src/
│   ├── scraper.py       # Web scraping logika (max 100 řádků)
│   ├── analyzer.py      # AI analýza článků (max 100 řádků)  
│   ├── generator.py     # Generování příspěvků (max 100 řádků)
│   ├── publisher.py     # Publikování na sociální síť (max 100 řádků)
│   └── scheduler.py     # Hlavní orchestrace (max 100 řádků)
├── config/
│   ├── sources.yaml     # Konfigurace zdrojů
│   └── settings.py      # Nastavení API klíčů
├── data/
│   └── articles/        # Cache článků
├── logs/               # Logy aplikace
└── requirements.txt    # Python dependencies
```

## Detailní specifikace modulů

### 1. scraper.py (max 100 řádků)
**Účel**: Stahování článků z českých ekonomických portálů

**Klíčové funkce**:
- `EconomyScraper.__init__(config_path)`: Inicializace s konfigurací zdrojů
- `scrape_rss_feed(feed_url, source_name)`: Stahování z RSS feedů
- `scrape_web_page(url
```

</details>
