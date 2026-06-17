---
name: google__agents-cli__skill
source: https://github.com/google/agents-cli/blob/91b4511cb9fcc52746e8141e20b48aa195fb159a/skills/google-agents-cli-observability/SKILL.md
repo: google/agents-cli
kind: skill
stars: 2873
last_pushed: 2026-06-10T17:15:35Z
license: apache-2.0
score: 9
domains: [agents-ai, observability, cloud-infrastructure, devops]
tags: [telemetry, tracing, logging, gcp, monitoring]
curated: 2026-06-15
curated_by: config-scout
---

# google/agents-cli — skill

**Why it's worth keeping:** The 'Order of Operations' section prevents critical Terraform state mismatches, and the 'Observability Tiers' table offers a clear decision matrix for complex tool selection.

**Summary:** A highly structured skill file for configuring observability (tracing, logging, and analytics) for AI agents on Google Cloud. It provides precise instructions on infrastructure provisioning, deployment tiers, and third-party integrations.

**Source credibility:** High: Official Google repository with high star count and active maintenance.

**Recency:** Very current; reflects modern agentic deployment workflows and cloud-native observability patterns.

**Source:** [google/agents-cli/skills/google-agents-cli-observability/SKILL.md](https://github.com/google/agents-cli/blob/91b4511cb9fcc52746e8141e20b48aa195fb159a/skills/google-agents-cli-observability/SKILL.md) · 2873★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: google-agents-cli-observability
description: >
  This skill should be used when the user wants to "set up tracing",
  "monitor my ADK agent", "configure logging", "add observability",
  "debug production traffic", or needs guidance on monitoring deployed
  ADK (Agent Development Kit) agents.
  Covers Cloud Trace, prompt-response logging, BigQuery Agent Analytics,
  third-party integrations (AgentOps, Phoenix, MLflow, etc.), and troubleshooting.
  Part of the Google ADK (Agent Development Kit) skills suite.
  Do NOT use for deployment setup (use google-agents-cli-deploy) or
  API code patterns (use google-agents-cli-adk-code).
metadata:
  author: Google
  license: Apache-2.0
  version: 0.4.0
  requires:
    bins:
      - agents-cli
    install: "uv tool install google-agents-cli"
---

# ADK Observability Guide

> **Cloud Trace** works out of the box — no infrastructure needed. **Prompt-response logging** and **BigQuery Agent Analytics** require Terraform-provisioned infrastructure (service account, GCS bucket, BigQuery dataset). Run `agents-cli infra single-project --project PROJECT_ID` to provision these resources. See `references/cloud-trace-and-logging.md` for details,
```

</details>
