---
name: wemake-services__django-modern-rest__skill
source: https://github.com/wemake-services/django-modern-rest/blob/62aef819dd37d6e3125fbeb77998d138d59bd1dd/.agents/skills/dmr/SKILL.md
repo: wemake-services/django-modern-rest
kind: skill
stars: 1270
last_pushed: 2026-06-15T02:06:50Z
license: mit
score: 9
domains: [backend-api, python, django]
tags: [performance, best-practices, django-modern-rest]
curated: 2026-06-15
curated_by: config-scout
---

# wemake-services/django-modern-rest — skill

**Why it's worth keeping:** Uses high-signal 'Wrong vs Correct' code blocks to teach specific API nuances, performance wins (msgspec vs pydantic), and correct error handling patterns.

**Summary:** Provides highly specific performance optimizations and architectural best practices for the django-modern-rest (DMR) framework.

**Source credibility:** High; based on a popular, actively maintained Django library with significant GitHub traction.

**Recency:** Very current; leverages modern Python type-hinting and async standards compatible with today's agentic workflows.

**Source:** [wemake-services/django-modern-rest/.agents/skills/dmr/SKILL.md](https://github.com/wemake-services/django-modern-rest/blob/62aef819dd37d6e3125fbeb77998d138d59bd1dd/.agents/skills/dmr/SKILL.md) · 1270★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: dmr
description: Write the best DMR code possible with all the recommended best practices, avoiding common mistakes.
---

# django-modern-rest skill

Here's a list of best practices to use for different parts of the application.


## Installing `django-modern-rest`

Always prefer to install `msgspec` extra, because it provides
the fastest json parsing / loading.

Always add `django-stubs[compatible-mypy]` to the dev dependencies,
because `django-modern-rest` requires types for Django during type checking.


## Defining controller

### Do not use `@validate`, when `@modify` is enough

This code:

```python
from http import HTTPStatus

import msgspec
from django.http import HttpResponse

from dmr import Body, Controller, ResponseSpec, validate
from dmr.plugins.msgspec import MsgspecSerializer


class UserModel(msgspec.Struct):
    email: str


class UserController(Controller[MsgspecSerializer]):
    @validate(  # <- describes unique return types from this endpoint
        ResponseSpec(
            UserModel,
            status_code=HTTPStatus.OK,
        ),
    )
    def post(self, parsed_body: Body[UserModel]) -> HttpResponse:
        # This response would have an explicit
```

</details>
