---
name: JosiahSiegel__claude-plugin-marketplace__skill
source: https://github.com/JosiahSiegel/claude-plugin-marketplace/blob/a775642a55a1ff79fe350d67f697d5f49e2171eb/plugins/azure-to-docker-master/skills/azure-emulators-2025/SKILL.md
repo: JosiahSiegel/claude-plugin-marketplace
kind: skill
stars: 45
last_pushed: 2026-05-28T04:04:26Z
license: mit
score: 9
domains: [backend-api, devops, cloud-infrastructure]
tags: [azure, docker, local-development, emulators]
curated: 2026-06-17
curated_by: config-scout
---

# JosiahSiegel/claude-plugin-marketplace — skill

**Why it's worth keeping:** Provides high-value 'copy-paste' assets like standard development connection strings, specific resource limits, and up-to-date API version/deprecations to prevent configuration errors.

**Summary:** A dense technical reference providing Docker Compose configurations and connection strings for Azure service emulators.

**Source credibility:** The repo shows recent activity and a reasonable star count for a niche plugin collection.

**Recency:** Highly current; includes 2025 updates like SQL Server Vector Search and Cosmos DB vnext-preview.

**Source:** [JosiahSiegel/claude-plugin-marketplace/plugins/azure-to-docker-master/skills/azure-emulators-2025/SKILL.md](https://github.com/JosiahSiegel/claude-plugin-marketplace/blob/a775642a55a1ff79fe350d67f697d5f49e2171eb/plugins/azure-to-docker-master/skills/azure-emulators-2025/SKILL.md) · 45★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: azure-emulators-2025
description: |
  Azure service emulators for local development in Docker (2025).
  PROACTIVELY activate for: (1) Azurite for Storage (Blob, Queue, Table) emulation, (2) Cosmos DB Linux Emulator container, (3) Event Hubs emulator, (4) Service Bus emulator, (5) Azure Functions Core Tools image, (6) Azure SQL Edge container, (7) Azure App Configuration emulator, (8) connection-string conventions for emulators, (9) seeding emulators with fixtures, (10) running integration tests against emulators in CI.
  Provides: emulator selection matrix, docker-compose templates, well-known dev connection strings, seed-data patterns, and CI integration recipes.
---

# Azure Service Emulators for Local Development (2025)

## Overview

This skill provides comprehensive knowledge of Azure service emulators available as Docker containers for local development in 2025.

## Available Azure Emulators

### 1. Azurite (Azure Storage Emulator)

**Official replacement for Azure Storage Emulator (deprecated)**

**Image:** `mcr.microsoft.com/azure-storage/azurite:latest`

**Supported Services:**
- Blob Storage
- Queue Storage
- Table Storage

**Configuration:**
```yaml
services:
```

</details>
