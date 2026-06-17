---
name: DanNeidle__epstein_search
source: https://github.com/DanNeidle/epstein_search/blob/9297b257d816b8398fabbc15f62e8cce72eabeb8/claude.md
repo: DanNeidle/epstein_search
kind: claude-md
stars: 17
last_pushed: 2026-02-13T22:02:15Z
license: unknown
score: 9
domains: [cli-tools, data-research]
tags: [workflow, command-line, search]
curated: 2026-06-14
curated_by: config-scout
---

# DanNeidle/epstein_search — claude-md

**Why it's worth keeping:** It defines specific command aliases, proactively addresses OCR error handling/verification, and establishes a rigorous 'Research Methodology' and reporting format that ensures traceability.

**Summary:** Provides specialized instructions for an agent to interact with a local CLI tool to query and analyze large-scale document data via Elasticsearch.

**Source credibility:** A niche research project with moderate social proof (17 stars).

**Recency:** Highly current; reflects modern agentic patterns for specialized tool interaction.

**Source:** [DanNeidle/epstein_search/claude.md](https://github.com/DanNeidle/epstein_search/blob/9297b257d816b8398fabbc15f62e8cce72eabeb8/claude.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Epstein Documents Research Agent

## Data Source
You have access to an Elasticsearch index at `http://localhost:9200` containing 1,046,911 OCR'd PDF documents from the Epstein case files. The index is called `sist2`.

## Document Schema
- `name`: Document filename (e.g. "EFTA02290848") - these are Bates numbers
- `content`: OCR-extracted full text (quality varies, expect typos and garbled text)
- `pages`: Page count
- `size`: File size in bytes
- `extension`: Always "pdf"
- `mtime`: Modified timestamp

## Querying with `ep`

**Always use `./ep.py` for all queries. Do not write raw curl or Python ES queries.**

The `ep` CLI tool handles query construction, output formatting, Bates numbers, clickable sist2 links, highlight snippets, and near-duplicate detection automatically.

### Counting documents
```bash
./ep.py count "Prince Andrew"          # How many docs mention this term?
./ep.py count -c "Andrew" "Epstein"    # Co-occurrence count (both terms must appear)
./ep.py c "Ghislaine"                  # Alias: c = count
```

### Searching with highlights
```bash
./ep.py search "flight log"            # Default 10 results with highlights
./ep.py search -n 20 "Mandelson"       # Mor
```

</details>
