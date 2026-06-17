---
name: manikosto__claude-code-python-stack__skill
source: https://github.com/manikosto/claude-code-python-stack/blob/805c4d6a5783d10a9e771ad524668a8d8b7fdd0d/skills/celery-patterns/SKILL.md
repo: manikosto/claude-code-python-stack
kind: skill
stars: 40
last_pushed: 2026-03-25T14:40:39Z
license: unknown
score: 9
domains: [backend, distributed-systems, python]
tags: [celery, task-queue, redis, production]
curated: 2026-06-15
curated_by: config-scout
---

# manikosto/claude-code-python-stack — skill

**Why it's worth keeping:** Includes critical production configurations like 'task_acks_late' and memory leak protection via 'worker_max_tasks_per_child', alongside sophisticated error handling for timeouts.

**Summary:** A comprehensive guide to production-grade Celery patterns, covering task orchestration, retry strategies with exponential backoff, and progress tracking.

**Source credibility:** Reasonable; 40 stars on a specialized toolkit suggests curated, useful content rather than generic boilerplate.

**Recency:** 

**Source:** [manikosto/claude-code-python-stack/skills/celery-patterns/SKILL.md](https://github.com/manikosto/claude-code-python-stack/blob/805c4d6a5783d10a9e771ad524668a8d8b7fdd0d/skills/celery-patterns/SKILL.md) · 40★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: celery-patterns
description: Celery patterns for distributed task queues — task definitions, retry strategies, scheduling, chains/groups, monitoring, and production configuration with Redis/RabbitMQ.
origin: custom
---

# Celery Patterns

Distributed task queue patterns for Python applications.

## When to Activate

- Offloading long-running tasks (email, PDF generation, data processing)
- Scheduling periodic tasks (cron-like)
- Building data processing pipelines
- Implementing retry logic for external API calls
- Setting up task monitoring and alerting

## Setup

### Configuration

```python
# config/celery.py
from celery import Celery
from app.config import settings

celery_app = Celery(
    "worker",
    broker=settings.REDIS_URL,
    backend=settings.REDIS_URL,
)

celery_app.conf.update(
    task_serializer="json",
    accept_content=["json"],
    result_serializer="json",
    timezone="UTC",
    enable_utc=True,
    task_track_started=True,
    task_time_limit=300,           # Hard limit: 5 minutes
    task_soft_time_limit=240,      # Soft limit: 4 minutes
    worker_prefetch_multiplier=1,  # Disable prefetching for fair scheduling
    worker_max_tasks_per_child=1000
```

</details>
