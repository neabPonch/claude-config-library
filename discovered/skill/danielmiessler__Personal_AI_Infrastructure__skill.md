---
name: danielmiessler__Personal_AI_Infrastructure__skill
source: https://github.com/danielmiessler/Personal_AI_Infrastructure/blob/2fde1bbe9e8f280cd4998e244b53e3c66f3dc8b9/Packs/Apify/src/SKILL.md
repo: danielmiessler/Personal_AI_Infrastructure
kind: skill
stars: 15945
last_pushed: 2026-05-20T21:33:46Z
license: mit
score: 9
domains: [web-scraping, agents-ai, data-extraction]
tags: [apify, token-optimization, typescript, lead-gen]
curated: 2026-06-16
curated_by: config-scout
---

# danielmiessler/Personal_AI_Infrastructure — skill

**Why it's worth keeping:** Demonstrates a high-level 'filter-in-code' architecture that solves the token bloat problem; includes highly actionable code patterns for lead generation and social listening.

**Summary:** Provides TypeScript wrappers for Apify actors designed to filter large datasets locally before passing them to the model context.

**Source credibility:** High; source is a well-known, highly starred repository by Daniel Miessler.

**Recency:** Current; addresses critical context management strategies essential for modern agentic workflows.

**Source:** [danielmiessler/Personal_AI_Infrastructure/Packs/Apify/src/SKILL.md](https://github.com/danielmiessler/Personal_AI_Infrastructure/blob/2fde1bbe9e8f280cd4998e244b53e3c66f3dc8b9/Packs/Apify/src/SKILL.md) · 15945★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: Apify
description: "Scrape social media platforms, business data, and e-commerce via Apify actors — Instagram profiles/posts/hashtags/comments, LinkedIn profiles/jobs/posts, TikTok profiles/hashtags/videos/comments, YouTube channels/search/comments, Facebook posts/groups/comments, Google Maps business search with contact/review/image extraction, Amazon products/reviews/pricing, and general-purpose multi-page web crawling with custom pageFunction extraction logic. File-based TypeScript wrappers (scrapeInstagramProfile, searchGoogleMaps, scrapeAmazonProduct, scrapeWebsite, etc.) filter and transform data in code before returning to model context, achieving 95-99% token savings over direct MCP protocol. Parallel multi-platform queries via Promise.all for social listening dashboards. Lead enrichment pipeline: Google Maps → qualified filter → optional LinkedIn enrichment. Competitive analysis across Instagram, YouTube, and TikTok simultaneously. USE WHEN scrape Instagram, scrape LinkedIn, scrape TikTok, scrape YouTube, scrape Facebook, Google Maps leads, Amazon reviews, business intelligence, multi-platform social listening, competitive analysis, lead generation, social monito
```

</details>
