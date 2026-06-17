---
name: Jamkris__everything-gemini-code__skill
source: https://github.com/Jamkris/everything-gemini-code/blob/f8a6a263c88d26eb40e0c3f1634081378283d0f4/skills/django-tdd/SKILL.md
repo: Jamkris/everything-gemini-code
kind: skill
stars: 83
last_pushed: 2026-05-26T05:02:20Z
license: mit
score: 9
domains: [backend-api, python]
tags: [django, tdd, pytest, testing-infrastructure]
curated: 2026-06-16
curated_by: config-scout
---

# Jamkris/everything-gemini-code — skill

**Why it's worth keeping:** Includes critical speed optimizations like disabling migrations and faster password hashing, plus a complete pattern for using factory_boy with pytest fixtures.

**Summary:** A high-quality TDD blueprint for Django that includes performance-optimized test settings and automated data generation patterns.

**Source credibility:** The repository has decent social proof (83 stars) and provides highly specialized engineering configurations.

**Recency:** Modern; uses current best practices for Django testing ecosystems.

**Source:** [Jamkris/everything-gemini-code/skills/django-tdd/SKILL.md](https://github.com/Jamkris/everything-gemini-code/blob/f8a6a263c88d26eb40e0c3f1634081378283d0f4/skills/django-tdd/SKILL.md) · 83★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: django-tdd
description: Django testing strategies with pytest-django, TDD methodology, factory_boy, mocking, coverage, and testing Django REST Framework APIs.
---

# Django Testing with TDD

Test-driven development for Django applications using pytest, factory_boy, and Django REST Framework.

## When to Use

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
addopts =
    --reuse-db
    --nomig
```

</details>
