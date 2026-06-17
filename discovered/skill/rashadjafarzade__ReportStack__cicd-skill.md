---
name: rashadjafarzade__ReportStack__cicd-skill
source: https://github.com/rashadjafarzade/ReportStack/blob/8134ff5efb324c2810a392903373ef9f5e216aae/cicd-skill.md
repo: rashadjafarzade/ReportStack
kind: skill
stars: 0
last_pushed: 2026-05-09T21:43:43Z
license: unknown
score: 9
domains: [devops, cicd, infrastructure]
tags: [linux, environment-context, system-admin]
curated: 2026-06-15
curated_by: config-scout
---

# rashadjafarzade/ReportStack — skill

**Why it's worth keeping:** The 'Key decisions with reasoning' section is elite; it prevents the agent from attempting resource-heavy tasks like deploying Ollama based on known RAM limits. The inclusion of architecture diagrams and multi-arch development warnings makes it highly practical for troubleshooting.

**Summary:** Provides exhaustive environmental context for a CI/CD and reporting stack on a specific Linux host. It includes hardware constraints, network mappings, and architectural reasoning.

**Source credibility:** Low public visibility (0 stars), but high technical density suggests a legitimate engineering document.

**Recency:** Very current, mentioning Ubuntu 24.04 and modern Docker/Node versions.

**Source:** [rashadjafarzade/ReportStack/cicd-skill.md](https://github.com/rashadjafarzade/ReportStack/blob/8134ff5efb324c2810a392903373ef9f5e216aae/cicd-skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: automation-cicd-twd00030
description: Set up, deploy, troubleshoot, or extend the CI/CD pipeline and Automation Reports web app on Linux host twd00030. Use this skill whenever the user asks about Jenkins setup, the pytest automation framework, the Reports app deployment, Docker Compose configuration, the integration between Jenkins and the Reports app, or any infrastructure on this specific Linux machine. Trigger on phrases like "the pipeline", "Jenkins", "the reports app", "automation framework", "deploy", "twd00030", or any mention of test reporting infrastructure.
---

# Automation CI/CD + Reports App on twd00030

## Project overview

This project consists of two integrated systems running on a single Linux host:

1. **CI/CD pipeline** — Jenkins orchestrates a pytest-based automation framework. Jenkins pulls code from GitHub, builds a Docker image with the framework, runs the test suite in that container, and reports results.
2. **Automation Reports web app** — A self-hosted ReportPortal-style platform (FastAPI + React + Postgres) that receives test results from the pytest framework via a custom plugin (`pytest-automation-reports`) and presents them to users.

The two
```

</details>
