---
name: iMerica__dj-rest-auth
source: https://github.com/iMerica/dj-rest-auth/blob/90082e3a4d257c053e5eef3f30f51cc7f55492ee/CLAUDE.md
repo: iMerica/dj-rest-auth
kind: claude-md
stars: 1859
last_pushed: 2026-06-05T17:02:00Z
license: mit
score: 9
domains: [backend-api, python, django]
tags: [architecture-focused, testing-guidance, django]
curated: 2026-06-14
curated_by: config-scout
---

# iMerica/dj-rest-auth — claude-md

**Why it's worth keeping:** It explains the 'Settings-as-import-strings' pattern, which is crucial for an AI to understand how to override components via configuration rather than subclassing. It also highlights specific test helpers like `override_api_settings` that are vital for writing valid unit tests.

**Summary:** Provides high-level architectural patterns and specific testing utility guidance for a Django authentication library.

**Source credibility:** Highly credible; a well-maintained, high-star industry standard in the Django ecosystem.

**Recency:** Current; aligns perfectly with modern Python development workflows and Claude Code's capabilities.

**Source:** [iMerica/dj-rest-auth/CLAUDE.md](https://github.com/iMerica/dj-rest-auth/blob/90082e3a4d257c053e5eef3f30f51cc7f55492ee/CLAUDE.md) · 1859★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

dj-rest-auth is a Django REST Framework package providing authentication API endpoints (login, logout, registration, password reset/change, JWT auth). It integrates with django-allauth for social auth and registration.

## Common Commands

### Running Tests
```bash
# All tests
python runtests.py

# Single test
DJANGO_SETTINGS_MODULE=dj_rest_auth.tests.settings python -m django test dj_rest_auth.tests.test_api.APIBasicTests.test_login

# With coverage
coverage run ./runtests.py && coverage report
```

### Linting
```bash
flake8 dj_rest_auth/
```

### Tox (full CI matrix: Python 3.8-3.12, Django 4.2/5.0)
```bash
tox                  # all envs
tox -e flake8        # lint only
tox -e coverage      # coverage only
```

### Install Test Dependencies
```bash
pip install -r dj_rest_auth/tests/requirements.txt
```

## Architecture

### Core Package (`dj_rest_auth/`)

- **`app_settings.py`** — Central configuration via `REST_AUTH` Django setting dict. All serializers and the token model are specified as dotted import strings, making everything overridable
```

</details>
