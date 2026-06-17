---
name: openshift__release
source: https://github.com/openshift/release/blob/b3e0d712df84b0eb592a9868e2cba18bb09b55f2/CLAUDE.md
repo: openshift/release
kind: claude-md
stars: 320
last_pushed: 2026-06-15T11:29:21Z
license: apache-2.0
score: 9
domains: [devops, ci-cd, infrastructure-as-code]
tags: [make, kubernetes, openshift, prow, workflow-automation]
curated: 2026-06-15
curated_by: config-scout
---

# openshift/release — claude-md

**Why it's worth keeping:** It includes custom slash commands to navigate a massive component registry and provides specific 'make' command mappings for various workflow stages (config vs. validation).

**Summary:** Provides deep architectural context for a complex CI/CD orchestration system used by OpenShift, covering generation pipelines and strict naming conventions.

**Source credibility:** High; maintained by the Red Hat OpenShift team in a high-traffic repository.

**Recency:** Current; utilizes advanced Claude Code features like custom slash commands.

**Source:** [openshift/release/CLAUDE.md](https://github.com/openshift/release/blob/b3e0d712df84b0eb592a9868e2cba18bb09b55f2/CLAUDE.md) · 320★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

This repository holds OpenShift cluster manifests, component build manifests and CI workflow configuration for OpenShift component repositories for both OKD and OCP.

## Documentation

Additional documentation and references for working with this repository:

- [OpenShift CI Documentation](https://docs.ci.openshift.org/) - Main documentation site for OpenShift CI infrastructure
- [CI Operator Reference](https://steps.ci.openshift.org/ci-operator-reference) - Comprehensive reference for CI operator configuration specification and step registry

## Repository Structure

- `ci-operator/config/` - CI configuration files defining builds and tests for component repositories
- `ci-operator/jobs/` - Generated Prow job configurations (auto-generated, rarely edited manually)
- `ci-operator/step-registry/` - Reusable test steps, chains, and workflows for multi-stage jobs
- `ci-operator/templates/` - Legacy black-box test workflows (deprecated, use step-registry instead)
- `core-services/` - Core service configurations applied to api.ci cluster
- `services/` - Additional service
```

</details>
