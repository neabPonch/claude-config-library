---
name: BostonOrange__claude-code-framework__claude-example
source: https://github.com/BostonOrange/claude-code-framework/blob/1a57034fc128126f1a90039a20ec2386f76f7610/docs/examples/python-api/CLAUDE.md.example
repo: BostonOrange/claude-code-framework
kind: claude-md
stars: 1
last_pushed: 2026-06-11T02:13:11Z
license: mit
score: 9
domains: [backend-api, devops, ai-agents, workflow-automation]
tags: [onboarding, slash-commands, stateful-memory, cicd]
curated: 2026-06-16
curated_by: config-scout
---

# BostonOrange/claude-code-framework — claude-md

**Why it's worth keeping:** The 'Onboarding' logic that populates structured .claude/memory/ files is an elite technique for maintaining long-term context. The 'Skills' and 'Factory Mode' patterns provide a blueprint for defining high-level, multi-step autonomous workflows.

**Summary:** This configuration implements a sophisticated agentic development system using stateful memory files and intent-based slash commands. It transforms Claude from a simple code assistant into a project-aware engineer that follows specific workflows.

**Source credibility:** Low star count but very high-quality documentation suggests a highly skilled individual developer or architect.

**Recency:** Very current; aligns perfectly with Claude Code's capabilities for tool usage and slash commands.

**Source:** [BostonOrange/claude-code-framework/docs/examples/python-api/CLAUDE.md.example](https://github.com/BostonOrange/claude-code-framework/blob/1a57034fc128126f1a90039a20ec2386f76f7610/docs/examples/python-api/CLAUDE.md.example) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

## Project Overview

MedTrack API is a HIPAA-compliant backend service for a healthcare scheduling platform. It manages patient appointments, provider availability, insurance verification, and clinical notes. The API serves a React Native mobile app and an internal web dashboard. The system handles approximately 15k API requests per minute during peak hours and integrates with several EHR (Electronic Health Record) systems via HL7 FHIR.

**Key Technologies:**
- Python 3.12
- FastAPI 0.109
- SQLAlchemy 2.x with Alembic migrations
- PostgreSQL 16
- Redis 7 (caching and task queue broker)
- Celery 5.x for async task processing
- Pydantic v2 for request/response validation
- AWS (ECS Fargate, RDS, ElastiCache, S3, SQS)
- Terraform for infrastructure

## Onboarding

**On every conversation start**, check whether this project has been fully onboarded by looking for these memory files relative to the project root:

- `.claude/memory/user_role.md`
- `.claude/memory/project_context.md`
- `.claude/memory/project_environments.md`
- `.claude/memory/project_workflow.md`
- `.claude/memory/project_preferences.md`

### If any memory files are missing

Guide the user through onboarding
```

</details>
