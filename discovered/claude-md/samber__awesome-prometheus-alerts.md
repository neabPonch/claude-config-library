---
name: samber__awesome-prometheus-alerts
source: https://github.com/samber/awesome-prometheus-alerts/blob/5cc052fc0a2a641ca3863dc748c32e1a1a552f4f/CLAUDE.md
repo: samber/awesome-prometheus-alerts
kind: claude-md
stars: 8030
last_pushed: 2026-06-02T16:39:32Z
license: other
score: 9
domains: [devops, observability, infrastructure]
tags: [prometheus, promql, rules-validation, alerts]
curated: 2026-06-14
curated_by: config-scout
---

# samber/awesome-prometheus-alerts — claude-md

**Why it's worth keeping:** The 'Query Validation' section is exceptional; it provides specific technical edge cases (unit differences, naming transitions, and metric existence patterns) to prevent common LLM hallucinations in a niche domain.

**Summary:** A highly detailed instruction set that combines project architecture with deep domain-specific validation rules for Prometheus/PromQL.

**Source credibility:** Very high; the source repository is a major industry resource with over 8k stars.

**Recency:** Current; includes up-to-date technical nuances regarding recent exporter version changes.

**Source:** [samber/awesome-prometheus-alerts/CLAUDE.md](https://github.com/samber/awesome-prometheus-alerts/blob/5cc052fc0a2a641ca3863dc748c32e1a1a552f4f/CLAUDE.md) · 8030★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A curated collection of ~940 Prometheus alerting rules covering 90+ services across 100+ exporters, organized in categories: basic resource monitoring (Prometheus, host/hardware, SMART, Docker, Blackbox, Windows, VMware, Netdata), databases (MySQL, PostgreSQL, Redis, MongoDB, Elasticsearch, Cassandra, Clickhouse, CouchDB, etc.), message brokers (RabbitMQ, Kafka, Pulsar, Nats, Zookeeper), proxies/load balancers/service meshes (Nginx, Apache, HaProxy, Traefik, Caddy, Linkerd, Istio), runtimes (PHP-FPM, JVM, Sidekiq), data engineering (Apache Flink, Apache Spark, Hadoop), orchestrators (Kubernetes, Nomad, Consul, Etcd, OpenStack), CI/CD (Jenkins, ArgoCD, FluxCD, GitLab CI, Spinnaker), network and security (SSL/TLS, CoreDNS, Vault, Cloudflare, Cilium, eBPF), storage (Ceph, ZFS, OpenEBS, Minio), cloud providers (AWS, Azure, DigitalOcean), observability (Thanos, Loki, Cortex, OpenTelemetry Collector, Grafana Tempo/Mimir/Alloy, Jaeger), and other (APC UPS, Graph Node).

All rules are stored in a single YAML data file (`_data/rules.yml`) and rendered as
```

</details>
