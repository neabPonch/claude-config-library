---
name: PavelRavvich__firesync
source: https://github.com/PavelRavvich/firesync/blob/c0f74b54875b88308d47c67688298c0ab8dfb7ec/CLAUDE.MD
repo: PavelRavvich/firesync
kind: claude-md
stars: 1
last_pushed: 2026-01-20T01:35:27Z
license: mit
score: 9
domains: [cli-tools, infrastructure-as-code, cloud-gcp]
tags: [firestore, gcp, python, iac]
curated: 2026-06-15
curated_by: config-scout
---

# PavelRavvich/firesync — claude-md

**Why it's worth keeping:** Provides concrete examples (like unittest mocking) and specific rules for module separation, error handling, and cross-platform compatibility to ensure architectural consistency.

**Summary:** A comprehensive technical blueprint defining architectural patterns, testing strategies, and operational procedures for a Firestore management tool.

**Source credibility:** Low star count but features highly professional-grade technical documentation structure.

**Recency:** Uses modern Python standards like type hints, dataclasses, and pathlib.

**Source:** [PavelRavvich/firesync/CLAUDE.MD](https://github.com/PavelRavvich/firesync/blob/c0f74b54875b88308d47c67688298c0ab8dfb7ec/CLAUDE.MD) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# FireSync - Infrastructure as Code for Firestore

## Project Overview

**FireSync** is a Python-based tool for managing Firestore database schemas as code. It enables version control and deployment automation for:
- Composite indexes
- Single-field indexes
- TTL (Time-To-Live) policies

Built by Pavel Ravvich and licensed under the MIT License.

## Core Concepts

### Workflow Pattern
FireSync follows a Terraform-like workflow:
1. **Pull** - Export current Firestore schema from GCP to local JSON files
2. **Plan** - Compare local schema files against remote Firestore state
3. **Apply** - Deploy local schema changes to Firestore

### Environment Management
Supports multiple environments (dev, staging, production) with separate GCP service account credentials stored in `secrets/gcp-key-{env}.json`.

## Project Structure

```
firesync/
├── core/                   # Python package with core functionality
│   ├── __init__.py
│   ├── config.py           # Configuration and environment management
│   ├── gcloud.py           # GCloud CLI wrapper
│   ├── normalizers.py      # Data normalization functions
│   ├── operations.py       # Resource-specific operations
│   └── schema.py           #
```

</details>
