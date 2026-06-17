---
name: AprilxHeart__manga-translate-ai
source: https://github.com/AprilxHeart/manga-translate-ai/blob/374b78c23ea21a86f1a6b00c1cf87bb553d8d28a/claude.md
repo: AprilxHeart/manga-translate-ai
kind: claude-md
stars: 0
last_pushed: 2026-04-30T14:47:45Z
license: unknown
score: 9
domains: [computer-vision, automation, cli-tools]
tags: [refactor-spec, pipeline, ocr]
curated: 2026-06-15
curated_by: config-scout
---

# AprilxHeart/manga-translate-ai — claude-md

**Why it's worth keeping:** The 'Implementation Order' is an elite technique for guiding agents through complex dependency chains, and the granular module constraints prevent AI over-engineering.

**Summary:** A highly structured technical specification for refactoring a manga translation pipeline into a modular, production-ready system.

**Source credibility:** Low GitHub presence/stars, but high technical density suggests it is a functional project specification rather than generic content.

**Recency:** Current; references modern models like gpt-4o-mini and claude-haiku.

**Source:** [AprilxHeart/manga-translate-ai/claude.md](https://github.com/AprilxHeart/manga-translate-ai/blob/374b78c23ea21a86f1a6b00c1cf87bb553d8d28a/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Manga Translation Pipeline — Refactor Spec

## Goal
End-to-end manga/comic translation pipeline:
**Scraper → Panel Split → Text Detection → OCR → Translation → Inpainting → Typesetting → Output**

---

## Current Stack (to replace)
| Component | Current | Replace With |
|---|---|---|
| OCR | pytesseract | PaddleOCR |
| Text Detection | heuristic threshold + morphology | DBNet via PaddleOCR |
| Translation | GoogleTranslator | OpenAI / Claude API |
| Text Removal | white ellipse draw | OpenCV inpaint (Telea) |
| Scraper | basic Playwright | async + retry + lazy-load |

---

## Module Structure
```
/project
  /scraper        — Playwright scraper (async, retry, lazy-load)
  /ocr            — PaddleOCR wrapper (detect + recognize)
  /translate      — LLM translation (OpenAI/Claude, batch)
  /inpaint        — Text removal via OpenCV inpaint
  /render         — Thai typesetting (LINE Seed Sans, auto-wrap, center)
  /pipeline       — Orchestrator that wires all modules
  main.py         — CLI entry point
  requirements.txt
```

---

## Tasks

### TASK 1 — Project Scaffold
- [ ] Create folder structure: scraper/, ocr/, translate/, inpaint/, render/, pipeline/
- [ ] Add `__init__.py` to e
```

</details>
