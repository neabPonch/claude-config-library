---
name: tosin2013__jupyter-notebook-validator-operator
source: https://github.com/tosin2013/jupyter-notebook-validator-operator/blob/e2271510beee4121bec75a0f8b26f85c8f037bfd/CLAUDE.md
repo: tosin2013/jupyter-notebook-validator-operator
kind: claude-md
stars: 2
last_pushed: 2026-04-22T18:04:33Z
license: apache-2.0
score: 9
domains: [kubernetes, mlops, backend]
tags: [go, operator-sdk, architectural-patterns]
curated: 2026-06-15
curated_by: config-scout
---

# tosin2013/jupyter-notebook-validator-operator — claude-md

**Why it's worth keeping:** The 'Reconciliation Workflow' section provides a vital mental model for state machine transitions; the tiered testing strategy gives crucial context on test execution times/complexity.

**Summary:** Provides a comprehensive technical blueprint of the Kubernetes operator, covering build commands, system architecture, and reconciliation logic.

**Source credibility:** Real-world MLOps project with active maintenance history.

**Recency:** Very current, referencing Go 1.22 and Kubernetes 1.31.

**Source:** [tosin2013/jupyter-notebook-validator-operator/CLAUDE.md](https://github.com/tosin2013/jupyter-notebook-validator-operator/blob/e2271510beee4121bec75a0f8b26f85c8f037bfd/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

The Jupyter Notebook Validator Operator is a Kubernetes-native operator that automates Jupyter Notebook validation in MLOps workflows. Built with Operator SDK and Go, it orchestrates notebook execution in isolated pods, performs golden notebook comparisons, integrates with Git repositories, and validates against deployed ML models.

**Key Technologies**: Go 1.22+, Operator SDK v1.37.0, controller-runtime, OpenShift 4.18+, Kubernetes 1.31+

## Common Development Commands

### Building and Testing

```bash
# Build the operator binary
make build

# Run tests (unit + integration, excludes e2e)
make test

# Run E2E tests
make test-e2e

# Format code
make fmt

# Run static analysis
make vet

# Run linter
make lint

# Fix linting issues automatically
make lint-fix

# Generate CRD manifests and DeepCopy code
make manifests generate
```

### Running Locally

```bash
# Run operator locally (requires kubeconfig)
make run

# Install CRDs into cluster
make install

# Uninstall CRDs from cluster
make uninstall

# Deploy operator to cluster
make deploy IMG=quay
```

</details>
