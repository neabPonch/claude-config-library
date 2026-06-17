---
name: yangchuansheng__browser-harness-rust__skill
source: https://github.com/yangchuansheng/browser-harness-rust/blob/9960f9a97b342a10813ca1c40e4cd5c978b044c4/domains/duckduckgo/skill.md
repo: yangchuansheng/browser-harness-rust
kind: skill
stars: 7
last_pushed: 2026-06-15T19:08:48Z
license: mit
score: 9
domains: [agents-ai, api-integration, knowledge-retrieval]
tags: [duckduckgo, json-api, instant-answers, entity-lookup]
curated: 2026-06-16
curated_by: config-scout
---

# yangchuansheng/browser-harness-rust — skill

**Why it's worth keeping:** Provides highly specific JSON schemas for complex structures like Infoboxes and RelatedTopics, along with critical parameter optimizations (skip_disambig/no_html) that prevent LLM confusion.

**Summary:** Detailed API specification for high-speed, zero-auth knowledge retrieval via DuckDuckGo's instant answer service. It provides a low-latency alternative to heavy browser automation for entity and utility lookups.

**Source credibility:** High; part of a specialized Rust-based browser harness with recent maintenance.

**Recency:** 

**Source:** [yangchuansheng/browser-harness-rust/domains/duckduckgo/skill.md](https://github.com/yangchuansheng/browser-harness-rust/blob/9960f9a97b342a10813ca1c40e4cd5c978b044c4/domains/duckduckgo/skill.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DuckDuckGo — Instant Answer API

`https://api.duckduckgo.com` — completely public, no auth, no API key. Returns Wikipedia-sourced abstracts, infoboxes, and instant answers for well-known entities, calculations, and utility queries. Not a search engine — it does not return a list of web results for arbitrary queries.

## Do this first: pick your query type

| Query type | Example | `Type` | Returns |
|------------|---------|--------|---------|
| Named entity (specific) | `apple inc` | A | Full abstract + infobox |
| Ambiguous term | `python` | D | Disambiguation list in `RelatedTopics` |
| Instant answer | `random number` | E | Direct answer in `Answer` field |
| No match | `how to cook pasta` | `""` | All fields empty |

**Use `skip_disambig=1` and `no_html=1` in almost every call.** `skip_disambig=1` upgrades D→A when there's an obvious primary result (e.g., `elon musk` goes from disambiguation to full article). `no_html=1` removes `<b>` tags from the `Answer` field and strips bold markup from `Result` HTML strings.

**Never use a browser.** Everything is a single `http_get` JSON call, 183–320ms.

---

## Fastest path: entity lookup

```text
import json, urllib.parse
from helper
```

</details>
