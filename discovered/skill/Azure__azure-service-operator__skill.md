---
name: Azure__azure-service-operator__skill
source: https://github.com/Azure/azure-service-operator/blob/2a5e098b37aed51ea44d89bd0b28f5661623f760/.agents/skills/testing-aso-recordings/SKILL.md
repo: Azure/azure-service-operator
kind: skill
stars: 901
last_pushed: 2026-06-14T23:27:15Z
license: mit
score: 9
domains: [cli-tools, cloud-infrastructure, testing]
tags: [go, azure, integration-tests, vcr]
curated: 2026-06-15
curated_by: config-scout
---

# Azure/azure-service-operator — skill

**Why it's worth keeping:** Includes high-value patterns for pre-flight environment validation, asynchronous progress monitoring via log tailing, and explicit success verification steps.

**Summary:** Provides instructions for running ASO tests that use go-vcr to record or replay Azure HTTP interactions.

**Source credibility:** High; sourced from a major, well-maintained Azure open-source repository.

**Recency:** Current; highly optimized for agentic workflows requiring long-running task management.

**Source:** [Azure/azure-service-operator/.agents/skills/testing-aso-recordings/SKILL.md](https://github.com/Azure/azure-service-operator/blob/2a5e098b37aed51ea44d89bd0b28f5661623f760/.agents/skills/testing-aso-recordings/SKILL.md) · 901★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: testing-aso-recordings
description: Use when you need to run ASO controller CRUD tests or sample tests, verify recordings play back correctly, or re-record after changes.
---

# Run ASO Recording-Based Tests

ASO uses [go-vcr](https://github.com/gophercloud/go-vcr) to record and replay HTTP interactions with Azure. Tests run in two modes:

- **Playback** — replays previously recorded HTTP interactions. Fast (minutes), no Azure credentials needed, deterministic.
- **Recording** — makes live HTTP calls to Azure, captures interactions to YAML files. Slow (20–60+ min), requires credentials, creates new recordings for future playback.

The test framework automatically chooses: if a recording file exists, it replays; if not, it records live. Both test suites use envtest (a local Kubernetes API server) to run the controller under test.

## Test Suites

|                            | Controllers                             | Samples                                                                |
| -------------------------- | --------------------------------------- | ---------------------------------------------------------------------- |
| **Task command**           | `controll
```

</details>
