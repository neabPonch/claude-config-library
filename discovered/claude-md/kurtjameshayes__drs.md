---
name: kurtjameshayes__drs
source: https://github.com/kurtjameshayes/drs/blob/7a8afe87d9d0efcdc93765c41a65cffdfb645b39/CLAUDE.MD
repo: kurtjameshayes/drs
kind: claude-md
stars: 0
last_pushed: 2026-01-23T02:58:36Z
license: unknown
score: 9
domains: [backend-api, agents-ai, data-engineering]
tags: [architecture-heavy, pattern-driven, security-conscious]
curated: 2026-06-16
curated_by: config-scout
---

# kurtjameshayes/drs — claude-md

**Why it's worth keeping:** The inclusion of specific design patterns (Connector Pattern), visual data flow diagrams, and explicit 'Adding New...' workflows makes it extremely actionable for an LLM. It also preemptively addresses high-risk tasks like API key encryption/decryption.

**Summary:** Provides a highly detailed architectural blueprint and operational manual for a complex data retrieval system involving AI agents. It effectively maps out component relationships, data flows, and critical security procedures.

**Source credibility:** Low social proof on GitHub, but the depth of technical documentation suggests a sophisticated personal or internal tool.

**Recency:** Very current; references modern frameworks like LangGraph and specific model versions from 2025.

**Source:** [kurtjameshayes/drs/CLAUDE.MD](https://github.com/kurtjameshayes/drs/blob/7a8afe87d9d0efcdc93765c41a65cffdfb645b39/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - Data Retrieval System (DRS)

## Project Overview

The Data Retrieval System (DRS) is a flexible, extensible data retrieval framework built with Python, Flask, and MongoDB. It provides a unified interface for querying multiple data sources (USDA NASS, Census.gov, FBI Crime Data, local files) with caching, analysis capabilities, and AI-powered data source discovery.

## Core Architecture

### Components

1. **Core System** (`core/`)
   - `base_connector.py` - Abstract base class for all connectors
   - `connector_manager.py` - Manages connector lifecycle and routing
   - `query_engine.py` - Query execution, joining, and analysis orchestration
   - `cache_manager.py` - MongoDB-based caching with TTL
   - `data_analysis.py` - Statistical analysis engine (DataAnalysisEngine)
   - `analysis_plan_manager.py` - Manages saved analysis plans

2. **Connectors** (`connectors/`)
   - `usda_nass/` - USDA NASS QuickStats API connector
   - `census/` - Census.gov API connector
   - `fbi_crime/` - FBI Crime Data API connector
   - `local_file/` - Local CSV/JSON/Excel file connector
   - Each connector extends `BaseConnector` and implements `execute_query()`

3. **AI Discovery System**
```

</details>
