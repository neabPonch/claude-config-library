---
name: modbender__skill-library-mcp__skill
source: https://github.com/modbender/skill-library-mcp/blob/5934c483768f9f8c792b8b7c0bb6f45a77df3edf/data/fastapi/SKILL.md
repo: modbender/skill-library-mcp
kind: skill
stars: 8
last_pushed: 2026-06-16T12:58:45Z
license: mit
score: 9
domains: [backend-api, python]
tags: [fastapi, asyncio, pydantic, patterns]
curated: 2026-06-16
curated_by: config-scout
---

# modbender/skill-library-mcp — skill

**Why it's worth keeping:** It highlights high-risk pitfalls like blocking the event loop with sync drivers and mutable default arguments that LLMs frequently hallucinate or ignore.

**Summary:** An expert-level pattern guide for production FastAPI development, specifically targeting async event loop management and Pydantic v2 nuances.

**Source credibility:** The content demonstrates deep technical knowledge of Python's asynchronous ecosystem, suggesting a highly competent author.

**Recency:** Highly current; includes modern 'lifespan' patterns and Pydantic v2 syntax which are essential for modern development.

**Source:** [modbender/skill-library-mcp/data/fastapi/SKILL.md](https://github.com/modbender/skill-library-mcp/blob/5934c483768f9f8c792b8b7c0bb6f45a77df3edf/data/fastapi/SKILL.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: FastAPI
description: Build fast, production-ready Python APIs with type hints, validation, and async support.
metadata: {"clawdbot":{"emoji":"⚡","requires":{"bins":["python3"]},"os":["linux","darwin","win32"]}}
---

# FastAPI Patterns

## Async Traps
- Mixing sync database drivers (psycopg2, PyMySQL) in async endpoints blocks the event loop — use async drivers (asyncpg, aiomysql) or run sync code in `run_in_executor`
- `time.sleep()` in async endpoints blocks everything — use `await asyncio.sleep()` instead
- CPU-bound work in async endpoints starves other requests — offload to `ProcessPoolExecutor` or background workers
- Async endpoints calling sync functions that do I/O still block — the entire call chain must be async

## Pydantic Validation
- Default values in models become shared mutable state: `items: list = []` shares the same list across requests — use `Field(default_factory=list)`
- `Optional[str]` doesn't make a field optional in the request — add `= None` or use `Field(default=None)`
- Pydantic v2 uses `model_validate()` not `parse_obj()`, and `model_dump()` not `.dict()` — v1 methods are deprecated
- Use `Annotated[str, Field(min_length=1)]` for reusable vali
```

</details>
