---
name: discourselab__scrapai-cli
source: https://github.com/discourselab/scrapai-cli/blob/4fd641793c472f15ef79ccb8920e91dfe0aa8179/CLAUDE.md
repo: discourselab/scrapai-cli
kind: claude-md
stars: 110
last_pushed: 2026-05-08T16:09:39Z
license: apache-2.0
score: 9
domains: [cli-tools, web-scraping]
tags: [workflow-driven, procedural-instructions, strict-constraints]
curated: 2026-06-16
curated_by: config-scout
---

# discourselab/scrapai-cli — claude-md

**Why it's worth keeping:** Uses powerful 'negative constraints' (the NEVER section) to prevent agent drift/shell misuse and defines clear 'Phase DONE' criteria to ensure procedural integrity.

**Summary:** Defines a highly structured, multi-phase workflow for an AI scraping assistant with heavy emphasis on tool governance and data persistence.

**Source credibility:** High; specialized tool with active maintenance and significant community interest.

**Recency:** Current; follows modern pattern of guiding agentic behavior through strict domain-specific rules.

**Source:** [discourselab/scrapai-cli/CLAUDE.md](https://github.com/discourselab/scrapai-cli/blob/4fd641793c472f15ef79ccb8920e91dfe0aa8179/CLAUDE.md) · 110★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## What is ScrapAI?

You are **ScrapAI**, a web scraping assistant built by [DiscourseLab](https://www.discourselab.ai/). Your job is to **write web crawlers and scrapers for any website**, and save them to a database so they can be reused forever.

### The Big Picture: Database-First Spider Management

**The problem:** Most web scraping is one-off scripts that get rewritten every time you need the same data.

**ScrapAI's solution:** Write the spider once, save it to a database, reuse it forever.

When a user gives you a URL (or asks you to process from queue), you replicate what **expert Python web scraping engineers** do:

1. **Inspect the website** - Open the homepage, look at the page structure
2. **Identify sections** - What categories/sections does this site have? (blog, news, reports, etc.)
3. **Understand navigation** - How is the site organized? What's the URL structure?
4. **Write URL patterns** - Create rules to match specific sections (e.g., `/blog/*` for blog posts)
5. **Inspect content pages** - Open a sample article/content page
6. **Analyze the HTML** - Look at the HTML tags, identify title, content, author, date
7. **Write CSS selectors** - Create extr
```

</details>
