---
name: InfernYaCr__DeepThroath
source: https://github.com/InfernYaCr/DeepThroath/blob/b61eb0e677a4b1406037e3811a773122b27fe000/CLAUDE.MD
repo: InfernYaCr/DeepThroath
kind: claude-md
stars: 1
last_pushed: 2026-04-28T08:25:14Z
license: unknown
score: 9
domains: [security, ai-testing, backend-api, python]
tags: [karpathy-methodology, red-teaming, engineering-principles]
curated: 2026-06-14
curated_by: config-scout
---

# InfernYaCr/DeepThroath — claude-md

**Why it's worth keeping:** The 'Four Principles' provide excellent meta-instructions for LLM behavior (like asking vs. guessing), while the 'Critical Problems' section acts as a proactive guardrail against repeating known bugs during refactoring.

**Summary:** Implements a behavioral framework based on Karpathy's principles to enforce surgical precision and prevent overengineering. It uniquely pairs these high-level mental models with project-specific 'Critical Problems' to preempt known architectural mistakes.

**Source credibility:** Low star count, but demonstrates highly sophisticated engineering standards and structure.

**Recency:** Highly current; reflects modern LLM-driven development workflows.

**Source:** [InfernYaCr/DeepThroath/CLAUDE.MD](https://github.com/InfernYaCr/DeepThroath/blob/b61eb0e677a4b1406037e3811a773122b27fe000/CLAUDE.MD) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DeepThroath: AI Coding Assistant Guidelines

**Основано на методологии Андрея Карпатого для LLM-ассистентов**
**Проект:** DeepThroath — Red Team Security Testing & RAG Quality Evaluation Platform
**Версия:** 2.0 (обновлено 2026-04-21)

---

## О проекте

DeepThroath — платформа для автоматизированного тестирования безопасности LLM моделей (Red Teaming) и оценки качества RAG систем через DeepEval метрики.

**Стек:**
- Frontend: Next.js 16.2.2, React 19, TypeScript, Tailwind CSS
- Backend: Python 3.11, FastAPI (в разработке), Streamlit (deprecated)
- LLM: OpenAI, Anthropic, DeepSeek, Gemini
- Testing: DeepEval, pytest
- Data: DuckDB, Parquet, Pandas

**Статус:** Рефакторинг для деплоя (см. `ARCHITECTURE_REFACTORING.md`)

---

## Четыре принципа работы (по Карпатому)

### 1. Думай перед кодированием — не угадывай, спрашивай

**Директива:** Не делай предположений. Не скрывай путаницу. Покажи варианты.

**Правила:**
- Формулируй предположения явно, если что-то неясно
- Задавай вопросы при неоднозначности требований
- Предлагай альтернативы, если есть несколько подходов
- Останавливайся и называй проблему, если что-то запутано

**Пример:**
```
Плохо:
User: "Добавь экспорт для Red Team"
```

</details>
