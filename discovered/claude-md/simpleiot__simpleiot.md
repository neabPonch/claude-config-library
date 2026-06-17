---
name: simpleiot__simpleiot
source: https://github.com/simpleiot/simpleiot/blob/b3ee632ab1ced6a89166a02aee441a933e7e67ab/CLAUDE.md
repo: simpleiot/simpleiot
kind: claude-md
stars: 211
last_pushed: 2026-05-16T22:24:20Z
license: apache-2.0
score: 9
domains: [iot, backend, embedded-systems, go]
tags: [architecture-centric, workflow-driven, structured-plans]
curated: 2026-06-15
curated_by: config-scout
---

# simpleiot/simpleiot — claude-md

**Why it's worth keeping:** The 'Plans' section is a masterclass in instruction by defining a specific execution pattern (phase-based commits), and the architectural breakdown provides essential mental models for new feature development.

**Summary:** A comprehensive guide that bridges high-level architecture with low-level build requirements for a Go/Elm IoT platform.

**Source credibility:** Solid open-source project with 211 stars and active maintenance history.

**Recency:** Highly current, explicitly referencing Claude Code workflows.

**Source:** [simpleiot/simpleiot/CLAUDE.md](https://github.com/simpleiot/simpleiot/blob/b3ee632ab1ced6a89166a02aee441a933e7e67ab/CLAUDE.md) · 211★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Simple IoT is a Go-based IoT platform with an Elm frontend that enables distributed sensor data collection, telemetry, configuration, and device management. The system runs the same application in both cloud and edge instances, automatically synchronizing data between them using NATS messaging.

## Build System and Common Commands

### Setup and Dependencies
```bash
# Source environment setup (required for all operations)
source envsetup.sh

# Initial setup - installs frontend deps and configures Elm
siot_setup

# Install frontend dependencies only
siot_install_frontend_deps
```

### Building
```bash
# Build everything (frontend + backend)
siot_build

# Build frontend only (Elm SPA)
siot_build_frontend

# Build backend only (Go binary)
siot_build_backend

# Cross-compile for ARM
siot_build_arm
siot_build_arm64
```

### Development and Testing
```bash
# Start development mode with hot reloading (both frontend and backend)
siot_watch

# Run the application locally
siot_run [arguments]

# Run complete test suite (frontend + backend + linting)
siot_t
```

</details>
