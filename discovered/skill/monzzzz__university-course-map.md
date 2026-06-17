---
name: monzzzz__university-course-map
source: https://github.com/monzzzz/university-course-map/blob/e1cbc33fa2436455acf149c8486c354e0fb529d7/SKILL.MD
repo: monzzzz/university-course-map
kind: skill
stars: 1
last_pushed: 2026-05-08T05:03:53Z
license: unknown
score: 8
domains: [data-scraping, data-engineering]
tags: [scraping, json-schema, structured-data]
curated: 2026-06-15
curated_by: config-scout
---

# monzzzz/university-course-map — skill

**Why it's worth keeping:** It demonstrates excellent 'situational awareness' by defining the current state of the project and uses highly structured lookup tables (URLs/Subject Codes) to prevent agent hallucination. The inclusion of strict schema definitions and specific transformation rules (e.g., handling external prerequisites) is a masterclass in agentic prompting.

**Summary:** A high-fidelity instruction set for a large-scale web scraping and data structuring task. It provides the exact schema, business logic, and reference mapping required to transform unstructured university catalogs into structured JSON graphs.

**Source credibility:** Low star count, but the high technical density suggests a functional, high-quality private or niche project.

**Recency:** Very current; last updated within the past month.

**Source:** [monzzzz/university-course-map/SKILL.MD](https://github.com/monzzzz/university-course-map/blob/e1cbc33fa2436455acf149c8486c354e0fb529d7/SKILL.MD) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Course Map — Scraping Instructions for Codex / Claude Code

## Context

This project visualizes university course prerequisites as interactive flowcharts.
`public/data/{university-id}/{program}.json` holds one graph per university + program.

**Current state:**
- **UCI** — fully scraped (143 nodes, real descriptions + prereqs)
- **Purdue, Georgia Tech** — partial stubs (11 nodes, no descriptions)
- **All other 47 universities** — placeholder template data (`data_source: "top50_template"`, 11 fake nodes)

**Goal:** Replace every placeholder file with real data scraped from the official course catalog.

---

## Output JSON Schema

Every output file must match this schema exactly:

```json
{
  "university": "Full Official University Name",
  "us_news_national_rank_2026": 12,
  "catalog_year": "2025-26",
  "generated_at_utc": "2026-01-15T00:00:00+00:00",
  "subject": {
    "code": "CS",
    "name": "Computer Science",
    "url": "https://catalog.university.edu/courses/cs/"
  },
  "major_slug": "computer-science",
  "data_source": "scraped",
  "nodes": [
    {
      "id": "CS 101",
      "code": "CS 101",
      "title": "Introduction to Programming",
      "units": "3",
      "descrip
```

</details>
