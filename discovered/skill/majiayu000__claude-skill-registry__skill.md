---
name: majiayu000__claude-skill-registry__skill
source: https://github.com/majiayu000/claude-skill-registry/blob/0432e4f16a18b22ddcb36dfb8207b2efe6fb04ff/skills/devops/azure-emulators-2025-josiahsiegel-claude-plugin-market-071de710/SKILL.md
repo: majiayu000/claude-skill-registry
kind: skill
stars: 419
last_pushed: 2026-06-16T05:34:23Z
license: mit
score: 8
domains: [backend-api, devops, cloud-infrastructure]
tags: [azure, docker, local-development, sql]
curated: 2026-06-17
curated_by: config-scout
---

# majiayu000/claude-skill-registry — skill

**Why it's worth keeping:** It includes highly specific technical details like exact port mappings, recent API versioning, and new SQL vector search syntax which prevents hallucinated infrastructure setups.

**Summary:** Provides detailed Docker Compose configurations, connection strings, and integration snippets for local Azure service emulators in 2025.

**Source credibility:** High-quality registry with significant community traction (419 stars).

**Recency:** Extremely current, specifically targeting 2025 service updates and deprecations.

**Source:** [majiayu000/claude-skill-registry/skills/devops/azure-emulators-2025-josiahsiegel-claude-plugin-market-071de710/SKILL.md](https://github.com/majiayu000/claude-skill-registry/blob/0432e4f16a18b22ddcb36dfb8207b2efe6fb04ff/skills/devops/azure-emulators-2025-josiahsiegel-claude-plugin-market-071de710/SKILL.md) · 419★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: azure-emulators-2025
description: Azure service emulators for local development including Azurite, Cosmos DB, and Event Hub Docker containers
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
  azurite:
    image: mcr.microsoft.com/azure-storage/azurite:latest
    container_name: azurite
    command: azurite --blobHost 0.0.0.0 --queueHost 0.0.0.0 --tableHost 0.0.0.0 --loose
    ports:
      - "10000:10000"  # Blob service
      - "10001:10001"  # Queue service
      - "10002:10002"  # Table service
    volumes:
      - azurite-data:/data
    restart: unless-stopped
```

**Standard Development Connection String:**
```
DefaultEndpointsProtocol=http;AccountName=devstoreaccount1;AccountKey=Eby8vdM02xNOcqFlqUwJPLlmEtlCDX
```

</details>
