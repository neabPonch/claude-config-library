---
name: manu14357__zskills__skill
source: https://github.com/manu14357/zskills/blob/250ccff751f2aca9ad0ca680a856d3333bd32411/skills/appinsights-instrumentation/SKILL.md
repo: manu14357/zskills
kind: skill
stars: 16
last_pushed: 2026-05-06T17:56:00Z
license: mit
score: 9
domains: [devops, cloud-infrastructure, observability, azure]
tags: [telemetry, opentelemetry, app-insights, monitoring]
curated: 2026-06-15
curated_by: config-scout
---

# manu14357/zskills — skill

**Why it's worth keeping:** The decision tree and maturity model provide excellent reasoning frameworks that allow an agent to choose the correct implementation strategy based on service scale and complexity.

**Summary:** A highly structured guide for implementing end-to-end observability using Azure Application Insights and OpenTelemetry across various tech stacks.

**Source credibility:** Small niche repository, but the content reflects professional DevOps/SRE standards.

**Recency:** 

**Source:** [manu14357/zskills/skills/appinsights-instrumentation/SKILL.md](https://github.com/manu14357/zskills/blob/250ccff751f2aca9ad0ca680a856d3333bd32411/skills/appinsights-instrumentation/SKILL.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: appinsights-instrumentation
description: >
  Instrument applications with Azure Application Insights and OpenTelemetry for end-to-end observability.
  Use this skill when users ask about telemetry, tracing, metrics, logging, or monitoring setup.
  Covers SDK setup, correlation, sampling, dashboards, and alerts per OpenTelemetry standards.
compatibility:
  models: [any-llm]
  cloud: azure
  observability: [application-insights, opentelemetry]
---

# App Insights Instrumentation

Implement high-value telemetry with minimal noise and strong trace correlation for production troubleshooting and performance optimization.

## Use This Skill When

- The user needs monitoring for apps running in Azure
- The user needs distributed tracing across microservices
- The user needs alerting, dashboards, or root cause analysis visibility
- The user wants to migrate from custom logging to structured telemetry

## Context: Observability Maturity

**Immature**: No monitoring, errors discovered by users  
**Developing**: Logs and metrics collected, no correlation or alerting  
**Managed**: Traces linked across services, alerts firing, dashboards useful → **Target**  
**Optimized**: Real-time
```

</details>
