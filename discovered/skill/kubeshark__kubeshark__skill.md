---
name: kubeshark__kubeshark__skill
source: https://github.com/kubeshark/kubeshark/blob/9396e64b9b4848dbbd8116d2c63c99f50c4fa852/skills/kfl/SKILL.md
repo: kubeshark/kubeshark
kind: skill
stars: 11951
last_pushed: 2026-06-03T18:01:45Z
license: apache-2.0
score: 9
domains: [kubernetes, observability, network-security, cli-tools]
tags: [query-language, schema, k8s, eBPF]
curated: 2026-06-15
curated_by: config-scout
---

# kubeshark/kubeshark — skill

**Why it's worth keeping:** It uses highly specific trigger phrases and provides critical 'safety' instructions (like using map_get for labels) that prevent the model from making common syntax errors in a specialized language.

**Summary:** Enables an AI agent to act as a KFL2 expert by providing precise syntax, schema definitions, and protocol-specific field mappings for Kubeshark traffic analysis.

**Source credibility:** High; Kubeshark is a popular, well-maintained open-source Kubernetes observability tool.

**Recency:** Current; includes modern eBPF and Kubernetes context with a future-dated timestamp.

**Source:** [kubeshark/kubeshark/skills/kfl/SKILL.md](https://github.com/kubeshark/kubeshark/blob/9396e64b9b4848dbbd8116d2c63c99f50c4fa852/skills/kfl/SKILL.md) · 11951★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: kfl
user-invocable: false
description: >
  KFL2 (Kubeshark Filter Language) reference. This skill MUST be loaded before
  writing, constructing, or suggesting any KFL filter expression. KFL is statically
  typed — incorrect field names or syntax will fail silently or error. Do not guess
  at KFL syntax without this skill loaded. Trigger on any mention of KFL, CEL filters,
  traffic filtering, display filters, query syntax, filter expressions, write a filter,
  construct a query, build a KFL, create a filter expression, "how do I filter",
  "show me only", "find traffic where", protocol-specific queries (HTTP status codes,
  DNS lookups, Redis commands, Kafka topics), Kubernetes-aware filtering (by namespace,
  pod, service, label, annotation), L4 connection/flow filters, time-based queries,
  or any request to slice/search/narrow network traffic in Kubeshark. Also trigger
  when other skills need to construct filters — KFL is the query language for all
  Kubeshark traffic analysis.
last-updated: 2026-05-08
---

# KFL2 — Kubeshark Filter Language

You are a KFL2 expert. KFL2 is built on Google's CEL (Common Expression Language)
and is the query language for all Kubeshark t
```

</details>
