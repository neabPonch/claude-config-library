---
name: aaione__everything-claude-code-zh__skill
source: https://github.com/aaione/everything-claude-code-zh/blob/e0bac9878ae3641cc8d04bd03bd9cbbada9a0dba/skills/django-celery/SKILL.md
repo: aaione/everything-claude-code-zh
kind: skill
stars: 19
last_pushed: 2026-06-01T01:07:30Z
license: mit
score: 9
domains: [backend-api, distributed-systems, python]
tags: [django, celery, async-tasks, task-queues]
curated: 2026-06-16
curated_by: config-scout
---

# aaione/everything-claude-code-zh — skill

**Why it's worth keeping:** Includes critical advanced patterns like exponential backoff with jitter, idempotency through database guard clauses, and handling SoftTimeLimitExceeded for graceful cleanup. It also provides practical implementations of complex Canvas workflows (chain/group/chord).

**Summary:** A production-ready blueprint for integrating Django with Celery for asynchronous task processing.

**Source credibility:** Solid community-driven resource; specific enough to be a high-quality reference.

**Recency:** Very current with modern Django and Celery best practices.

**Source:** [aaione/everything-claude-code-zh/skills/django-celery/SKILL.md](https://github.com/aaione/everything-claude-code-zh/blob/e0bac9878ae3641cc8d04bd03bd9cbbada9a0dba/skills/django-celery/SKILL.md) · 19★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: django-celery
description: Django + Celery 异步任务模式 — 配置、任务设计、Beat 调度、重试、Canvas 工作流、监控和测试。当向 Django 应用添加后台任务、定时任务或异步处理时使用。
origin: ECC
---

# Django + Celery 异步任务模式

在 Django 中使用 Celery 配合 Redis 或 RabbitMQ 进行后台任务处理的生产级模式。

## 何时激活

- 向 Django 应用添加后台任务或异步处理
- 实现周期性/定时任务
- 从请求周期中卸载慢操作（邮件、PDF 生成、API 调用）
- 设置 Celery Beat 进行类 cron 调度
- 调试任务失败、重试或队列积压
- 为 Celery 任务编写测试

## 项目设置

### 安装

```bash
pip install celery[redis] django-celery-results django-celery-beat
```

### `celery.py` — 应用入口

```python
# config/celery.py
import os
from celery import Celery

os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'config.settings.development')

app = Celery('myproject')
app.config_from_object('django.conf:settings', namespace='CELERY')
app.autodiscover_tasks()  # 发现每个 INSTALLED_APP 中的 tasks.py

@app.task(bind=True, ignore_result=True)
def debug_task(self):
    print(f'请求：{self.request!r}')
```

```python
# config/__init__.py
from .celery import app as celery_app

__all__ = ('celery_app',)
```

### Django 设置

```python
# config/settings/base.py

# Broker（生产环境推荐 Redis）
CELERY_BROKER_URL = env('CELERY_BROKER_URL', default='redis://localhost:6379/0')
CELERY_RESULT_BACKEND = env('CELERY_RESULT_BAC
```

</details>
