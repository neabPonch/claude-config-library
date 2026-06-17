---
name: openshift__distributed-tracing-qe__skill
source: https://github.com/openshift/distributed-tracing-qe/blob/ddaf0cbcc3874962c598caf79012d42711792eab/plugins/qe-agent/skills/SKILL.md
repo: openshift/distributed-tracing-qe
kind: skill
stars: 4
last_pushed: 2026-06-10T06:45:59Z
license: apache-2.0
score: 9
domains: [devops, ci-cd, kubernetes, observability]
tags: [test-triage, environment-reproduction, ci-automation]
curated: 2026-06-15
curated_by: config-scout
---

# openshift/distributed-tracing-qe — skill

**Why it's worth keeping:** It includes highly transferable patterns for 'environment reconstruction,' such as converting ephemeral image-mount commands into idempotent git clones, and pre-flight checks for cluster stability to prevent false positives.

**Summary:** An advanced agentic skill that automates the triage, reproduction, and fixing of complex CI failures in OpenShift environments.

**Source credibility:** High; authored by Red Hat OpenShift QE with active maintenance.

**Recency:** Current; utilizes modern Kubernetes/OpenShift orchestration workflows.

**Source:** [openshift/distributed-tracing-qe/plugins/qe-agent/skills/SKILL.md](https://github.com/openshift/distributed-tracing-qe/blob/ddaf0cbcc3874962c598caf79012d42711792eab/plugins/qe-agent/skills/SKILL.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: qe-agent
description: Use this skill to analyze failing CI tests for Red Hat OpenShift Distributed Tracing (OpenTelemetry Operator, Tempo Operator, Tracing UI console plugin), rerun the specific failing tests, diagnose whether the failure is a product bug or a test that needs fixing, apply fixes to test source files when needed, and export results to the artifact directory. Trigger whenever $SHARED_DIR/qe-agent-context.json is present with has_test_failures=true or when an engineer asks to debug, rerun, or fix failing distributed tracing QE tests.
---

# RHOSDT QE Agent — Test Failure Triage and Fix

This skill drives an agentic loop that takes failing CI test results, reruns the failing tests, determines root cause (product bug vs broken test), and either fixes the test or writes a structured bug report.

## Test Infrastructure Overview

Three test suites are supported. The JUnit report name prefix tells you which suite failed:

| JUnit prefix | Suite | Framework | Repo |
|---|---|---|---|
| `junit_otel_*` | OpenTelemetry Operator | chainsaw | `https://github.com/openshift/opentelemetry-operator` |
| `junit_tempo_*` | Tempo Operator | chainsaw | `https://github.com/grafa
```

</details>
