---
name: bobmatnyc__claude-mpm-skills__skill
source: https://github.com/bobmatnyc/claude-mpm-skills/blob/557f86db6e51f415578ece110817ef495ea1c1bb/toolchains/python/async/celery/SKILL.md
repo: bobmatnyc/claude-mpm-skills
kind: skill
stars: 54
last_pushed: 2026-06-15T19:03:04Z
license: mit
score: 9
domains: [backend, python, distributed-systems]
tags: [celery, task-queue, asynchronous]
curated: 2026-06-15
curated_by: config-scout
---

# bobmatnyc/claude-mpm-skills — skill

**Why it's worth keeping:** The 'progressive_disclosure' metadata pattern is a sophisticated way to handle large docs, and the inclusion of deep configuration patterns (like Redis Sentinel and SQS) provides high-density utility.

**Summary:** A highly structured technical reference for Celery that uses progressive disclosure to manage context window efficiency.

**Source credibility:** Good; active repository with reasonable social proof and up-to-date content.

**Recency:** 

**Source:** [bobmatnyc/claude-mpm-skills/toolchains/python/async/celery/SKILL.md](https://github.com/bobmatnyc/claude-mpm-skills/blob/557f86db6e51f415578ece110817ef495ea1c1bb/toolchains/python/async/celery/SKILL.md) · 54★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: celery
description: Distributed task queue system for Python enabling asynchronous execution of background jobs, scheduled tasks, and workflows across multiple workers with Django, Flask, and FastAPI integration.
user-invocable: false
disable-model-invocation: true
progressive_disclosure:
  entry_point:
    - summary
    - when_to_use
    - quick_start
  sections:
    - core_concepts
    - broker_setup
    - task_basics
    - task_execution
    - task_routing
    - periodic_tasks
    - workflows
    - error_handling
    - monitoring
    - framework_integration
    - testing
    - production_patterns
    - performance
    - use_cases
    - alternatives
    - best_practices
    - troubleshooting
---

# Celery: Distributed Task Queue

## Summary
Celery is a distributed task queue system for Python that enables asynchronous execution of background jobs across multiple workers. It supports scheduling, retries, task workflows, and integrates seamlessly with Django, Flask, and FastAPI.

## When to Use
- **Background Processing**: Offload long-running operations (email, file processing, reports)
- **Scheduled Tasks**: Cron-like periodic jobs (cleanup, backups, data sync)
- **Dist
```

</details>
