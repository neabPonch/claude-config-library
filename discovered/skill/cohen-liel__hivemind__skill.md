---
name: cohen-liel__hivemind__skill
source: https://github.com/cohen-liel/hivemind/blob/918dd9b5aa7e4eca42979882bb34967c184a044e/.claude/skills/celery-tasks/SKILL.md
repo: cohen-liel/hivemind
kind: skill
stars: 100
last_pushed: 2026-04-18T22:33:46Z
license: apache-2.0
score: 9
domains: [backend, python, distributed-systems]
tags: [celery, background-jobs, task-queue, async]
curated: 2026-06-15
curated_by: config-scout
---

# cohen-liel/hivemind — skill

**Why it's worth keeping:** Includes critical reliability settings like exponential backoff retries, task prioritization via multiple queues, and a concise 'Rules' section for idempotent execution.

**Summary:** A production-grade template for implementing Celery background tasks with prioritized queues and robust error handling.

**Source credibility:** High; the source repository is well-regarded with significant stars and recent maintenance.

**Recency:** Highly current; uses modern Python patterns and industry-standard Celery configurations.

**Source:** [cohen-liel/hivemind/.claude/skills/celery-tasks/SKILL.md](https://github.com/cohen-liel/hivemind/blob/918dd9b5aa7e4eca42979882bb34967c184a044e/.claude/skills/celery-tasks/SKILL.md) · 100★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: celery-tasks
description: Celery background task patterns for Python apps. Use when implementing background jobs, scheduled tasks, email sending, image processing, or any async work that shouldn't block a web request.
---

# Celery Background Tasks

## Setup
```python
# celery_app.py
from celery import Celery
from kombu import Queue

celery = Celery(
    "myapp",
    broker=settings.REDIS_URL,
    backend=settings.REDIS_URL,
    include=["app.tasks.email", "app.tasks.processing"],
)

celery.conf.update(
    task_serializer="json",
    result_serializer="json",
    accept_content=["json"],
    timezone="UTC",
    task_track_started=True,
    task_acks_late=True,          # Re-queue if worker crashes
    worker_prefetch_multiplier=1,  # Fair distribution
    task_queues=[
        Queue("high", routing_key="high"),
        Queue("default", routing_key="default"),
        Queue("low", routing_key="low"),
    ],
    task_default_queue="default",
    # Retry policy
    task_max_retries=3,
    task_soft_time_limit=300,   # 5 min warning
    task_time_limit=600,        # 10 min hard kill
)
```

## Task Patterns
```python
# tasks/email.py
from celery import shared_task
from celery
```

</details>
