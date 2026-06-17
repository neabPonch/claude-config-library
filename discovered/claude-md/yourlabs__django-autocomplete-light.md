---
name: yourlabs__django-autocomplete-light
source: https://github.com/yourlabs/django-autocomplete-light/blob/0f228d49b79e99af76421bf3c6f3b8a4b76d2623/CLAUDE.md
repo: yourlabs/django-autocomplete-light
kind: claude-md
stars: 1869
last_pushed: 2026-05-27T12:25:44Z
license: mit
score: 7
domains: [backend-api, django]
tags: [architecture-mapping, request-flow, testing]
curated: 2026-06-14
curated_by: config-scout
---

# yourlabs/django-autocomplete-light — claude-md

**Why it's worth keeping:** The 'Request flow' section is a high-level technique that gives an agent a mental model of the logic path, preventing hallucinated implementation steps.

**Summary:** Provides essential architectural context by mapping component roles and detailing specific request execution flows alongside testing procedures.

**Source credibility:** High-star (1800+), well-maintained Django library.

**Recency:** Current; reflects modern testing and project structure patterns.

**Source:** [yourlabs/django-autocomplete-light/CLAUDE.md](https://github.com/yourlabs/django-autocomplete-light/blob/0f228d49b79e99af76421bf3c6f3b8a4b76d2623/CLAUDE.md) · 1869★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Django Autocomplete Light

Django autocomplete library based on Select2.

## Structure
- `src/dal/` — core: `views.py`, `widgets.py`, `forms.py`, `forward.py`
- `src/dal_select2/` — Select2 integration: main view `Select2QuerySetView`
- `test_project/` — 17 test apps (unit + Selenium/Splinter)

## Request flow
`GET ?q=…&forward={…}` → `ViewMixin.dispatch()` → `BaseQuerySetView.get_queryset()` → Select2 JSON

## Common customisation
Override `get_queryset()`. Configure `search_fields`, `create_field`, `paginate_by`.
Forwarding: `forward=['country']` on the widget → `self.forwarded.get('country')` in the view.

## Tests
```bash
cd test_project/
pytest -v --liveserver 127.0.0.1:9999
BROWSER=firefox MOZ_HEADLESS=1 pytest -v   # headless
```
```

</details>
