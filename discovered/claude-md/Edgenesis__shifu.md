---
name: Edgenesis__shifu
source: https://github.com/Edgenesis/shifu/blob/0f87da39e5b3d19b2ba0d4041791a44c36381ef1/CLAUDE.md
repo: Edgenesis/shifu
kind: claude-md
stars: 1420
last_pushed: 2026-06-12T22:42:43Z
license: apache-2.0
score: 9
domains: [kubernetes, iot, backend-infrastructure, go]
tags: [k8s, go, architecture-pattern, iot]
curated: 2026-06-15
curated_by: config-scout
---

# Edgenesis/shifu — claude-md

**Why it's worth keeping:** Includes high-value 'how-to' procedures for extending the system and critical warnings about side-effect tasks like CRD manifest generation.

**Summary:** Provides a comprehensive technical blueprint covering build commands, architectural patterns, and specific extensibility workflows.

**Source credibility:** Highly credible; it is a popular CNCF/Kubernetes-native project with active maintenance.

**Recency:** 

**Source:** [Edgenesis/shifu/CLAUDE.md](https://github.com/Edgenesis/shifu/blob/0f87da39e5b3d19b2ba0d4041791a44c36381ef1/CLAUDE.md) · 1420★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Shifu is a Kubernetes-native IoT gateway (CNCF landscape project) that creates "digital twins" of physical IoT devices as Kubernetes pods. Each device gets a DeviceShifu pod that translates between the device's native protocol and a unified HTTP API.

## Build & Development Commands

```bash
# Build all targets
make build

# Run all tests (requires envtest setup — auto-downloaded)
make test

# Run a single package's tests
go test -v ./pkg/deviceshifu/deviceshifuhttp/...

# Format and vet
make fmt
make vet

# Install shifuctl CLI
make install

# Generate CRD manifests (from pkg/k8s/crd/)
cd pkg/k8s/crd && make manifests generate

# Build Docker images locally (single platform)
make buildx-build-image-deviceshifu-http-http
make buildx-build-image-shifu-controller
```

## Architecture

### Digital Twin Pattern

The core concept: for each physical IoT device, Shifu deploys a DeviceShifu pod in Kubernetes. This pod speaks the device's native protocol (MQTT, OPC UA, etc.) on one side and exposes a standard HTTP API on the other. Applications interact w
```

</details>
