---
name: YergZakon__recidiv2
source: https://github.com/YergZakon/recidiv2/blob/4afdf0b75cde5af850bb085ddc4c19f5ada29f0b/CLAUDE.MD
repo: YergZakon/recidiv2
kind: claude-md
stars: 0
last_pushed: 2025-08-11T14:36:47Z
license: unknown
score: 9
domains: [data-science, fullstack-migration, security]
tags: [strict-constraints, mathematical-integrity, refactoring]
curated: 2026-06-14
curated_by: config-scout
---

# YergZakon/recidiv2 — claude-md

**Why it's worth keeping:** Uses powerful negative constraints ('DO NOT simplify') to prevent AI drift of critical research constants; provides exact hardcoded weights and time windows to ensure the agent cannot 'optimize' or round away scientific accuracy.

**Summary:** Enforces strict mathematical and logical integrity during a migration from a Streamlit prototype to a production FastAPI/React stack.

**Source credibility:** Low star count, but content exhibits high technical rigor characteristic of domain-specific scientific software.

**Recency:** Updated late 2024, making it highly relevant for current Claude Code usage.

**Source:** [YergZakon/recidiv2/CLAUDE.MD](https://github.com/YergZakon/recidiv2/blob/4afdf0b75cde5af850bb085ddc4c19f5ada29f0b/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
🚨 КРИТИЧЕСКИЕ ПРАВИЛА (НИКОГДА НЕ НАРУШАТЬ)
Сохранность кода

ЗАПРЕЩЕНО удалять существующий Streamlit код - он остается как прототип/reference
ЗАПРЕЩЕНО удалять или изменять файлы в папках utils/, pages/ без явного указания
ОБЯЗАТЕЛЬНО сохранять параллельные версии (Streamlit + FastAPI/React)

Бизнес-логика и данные исследования

ЗАПРЕЩЕНО упрощать формулы расчета рисков в risk_calculator.py
ЗАПРЕЩЕНО изменять коэффициенты и веса без явного указания
ОБЯЗАТЕЛЬНО сохранять все временные окна из исследования:

Мошенничество: 109 дней
Кража: 146 дней
Убийство: 143 дня
Вымогательство: 144 дня
Грабеж: 148 дней
Разбой: 150 дней
Изнасилование: 157 дней


ОБЯЗАТЕЛЬНО сохранять проценты предотвратимости (82.3%, 87.3%, 97.0% и т.д.)
ОБЯЗАТЕЛЬНО сохранять паттерны поведения и их распределение (72.7% нестабильных и т.д.)

Архитектура

Структура проекта:
project/
├── backend/          # FastAPI приложение
├── frontend/         # React/Vue приложение  
├── pages/           # НЕ ТРОГАТЬ - Streamlit страницы
├── utils/           # НЕ ТРОГАТЬ - оригинальная бизнес-логика
├── main.py          # НЕ ТРОГАТЬ - Streamlit главная
└── requirements.txt # НЕ ТРОГАТЬ - для Streamlit


Процесс разработки

ОБЯ
```

</details>
