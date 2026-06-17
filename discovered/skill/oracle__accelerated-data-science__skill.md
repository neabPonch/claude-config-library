---
name: oracle__accelerated-data-science__skill
source: https://github.com/oracle/accelerated-data-science/blob/193028b0a25583a79a90a1af9562ff1c4c50ae5a/skills/aqua-metrics/SKILL.md
repo: oracle/accelerated-data-science
kind: skill
stars: 126
last_pushed: 2026-06-10T11:00:40Z
license: upl-1.0
score: 8
domains: [mlops, infrastructure-as-code, observability]
tags: [oci, vllm, prometheus, grafana, monitoring]
curated: 2026-06-15
curated_by: config-scout
---

# oracle/accelerated-data-science — skill

**Why it's worth keeping:** Features a clever architecture pattern using a 'signing proxy' to handle authenticated metric scraping and includes specific, high-value PromQL queries for LLM performance tracking.

**Summary:** Provides a complete blueprint for setting up a Prometheus and Grafana observability stack to monitor vLLM model deployments on OCI.

**Source credibility:** High; developed by Oracle for their Accelerated Data Science SDK.

**Recency:** Current, leveraging modern vLLM standards and OCI infrastructure patterns.

**Source:** [oracle/accelerated-data-science/skills/aqua-metrics/SKILL.md](https://github.com/oracle/accelerated-data-science/blob/193028b0a25583a79a90a1af9562ff1c4c50ae5a/skills/aqua-metrics/SKILL.md) · 126★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aqua-metrics
description: Set up Prometheus and Grafana monitoring for AQUA vLLM model deployments on OCI. Covers the signing proxy, container registry setup, OCI Container Instance deployment, and PromQL dashboards. Triggered when user wants to monitor LLM deployments, view TTFT/latency/throughput metrics, or set up observability for AQUA.
user-invocable: true
disable-model-invocation: false
---

# AQUA Deployment Metrics Monitoring

Monitor vLLM model deployments with Prometheus + Grafana hosted on an OCI Container Instance. The monitoring stack consists of:

- **Signing Proxy** — handles OCI IAM auth when scraping the `/metrics` endpoint
- **Prometheus** — scrapes metrics every 5s, stores time series
- **Grafana** — visualizes dashboards from Prometheus data

## Available Metrics (vLLM Prometheus)

All standard vLLM Prometheus metrics are available:

| Metric | Description |
|---|---|
| `vllm:time_to_first_token_seconds` | TTFT histogram |
| `vllm:inter_token_latency_seconds` | ITL histogram |
| `vllm:e2e_request_latency_seconds` | End-to-end request latency |
| `vllm:num_requests_running` | Concurrent requests in flight |
| `vllm:num_requests_waiting` | Requests queue
```

</details>
