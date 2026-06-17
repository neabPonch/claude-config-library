---
name: affaan-m__ECC__skill
source: https://github.com/affaan-m/ECC/blob/68e926bf77dd8ac15ea67b1aa551cba5b8b17e53/skills/django-tdd/SKILL.md
repo: affaan-m/ECC
kind: skill
stars: 216299
last_pushed: 2026-06-16T05:59:23Z
license: mit
score: 9
domains: [backend-api, python]
tags: [django, tdd, pytest, testing]
curated: 2026-06-16
curated_by: config-scout
---

# affaan-m/ECC — skill

**Why it's worth keeping:** Includes critical performance optimizations like disabling migrations and faster password hashing to minimize test suite latency. It provides highly structured fixtures and factories that serve as perfect scaffolding for agentic code generation.

**Summary:** A high-performance Django TDD blueprint using pytest and factory_boy, optimized for rapid development cycles.

**Source credibility:** High; utilizes industry-standard patterns used in professional enterprise Django environments.

**Recency:** 

**Source:** [affaan-m/ECC/skills/django-tdd/SKILL.md](https://github.com/affaan-m/ECC/blob/68e926bf77dd8ac15ea67b1aa551cba5b8b17e53/skills/django-tdd/SKILL.md) · 216299★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: django-tdd
description: Django testing strategies with pytest-django, TDD methodology, factory_boy, mocking, coverage, and testing Django REST Framework APIs.
metadata:
  origin: ECC
---

# Django Testing with TDD

Test-driven development for Django applications using pytest, factory_boy, and Django REST Framework.

## When to Activate

- Writing new Django applications
- Implementing Django REST Framework APIs
- Testing Django models, views, and serializers
- Setting up testing infrastructure for Django projects

## TDD Workflow for Django

### Red-Green-Refactor Cycle

```python
# Step 1: RED - Write failing test
def test_user_creation():
    user = User.objects.create_user(email='test@example.com', password='testpass123')
    assert user.email == 'test@example.com'
    assert user.check_password('testpass123')
    assert not user.is_staff

# Step 2: GREEN - Make test pass
# Create User model or factory

# Step 3: REFACTOR - Improve while keeping tests green
```

## Setup

### pytest Configuration

```ini
# pytest.ini
[pytest]
DJANGO_SETTINGS_MODULE = config.settings.test
testpaths = tests
python_files = test_*.py
python_classes = Test*
python_functions = test_*
addopts
```

</details>
