---
name: mitkox__fteplusai__api-integration-skill
source: https://github.com/mitkox/fteplusai/blob/7af47a9d8b8260234209d156c6449154bcabe3fc/skills/api-integration.skill.md
repo: mitkox/fteplusai
kind: skill
stars: 81
last_pushed: 2025-12-31T09:44:19Z
license: mit
score: 8
domains: [backend-api, agents-ai, reliability-engineering]
tags: [api-integration, resilience-patterns, python]
curated: 2026-06-15
curated_by: config-scout
---

# mitkox/fteplusai — skill

**Why it's worth keeping:** The thread-safe Circuit Breaker implementation and the exponential backoff decorator provide highly transferable, production-ready code for building reliable agentic workflows.

**Summary:** A high-level technical guide for implementing resilient API integration patterns including authentication, error recovery, and provider abstraction.

**Source credibility:** Moderate; the repo has a decent star count and provides high-quality architectural patterns rather than just boilerplate.

**Recency:** Current; references modern models like Claude 3.5 Sonnet.

**Source:** [mitkox/fteplusai/skills/api-integration.skill.md](https://github.com/mitkox/fteplusai/blob/7af47a9d8b8260234209d156c6449154bcabe3fc/skills/api-integration.skill.md) · 81★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
skill: 'api-integration'
version: '2.0.0'
updated: '2025-12-31'
category: 'technical-integration'
complexity: 'advanced'
prerequisite_skills: ['code-examples']
composable_with: ['code-examples', 'technical-writing', 'production-readiness']
---

# API Integration Skill

## Overview
Comprehensive expertise in integrating AI APIs and SDKs into enterprise development workflows, covering authentication, error handling, performance optimization, and multi-provider strategies.

## Core Integration Patterns

### Authentication Methods

**API Key Authentication:**
```python
import os
from openai import OpenAI

# Load from environment variable (recommended)
client = OpenAI(api_key=os.environ.get("OPENAI_API_KEY"))

# Never hardcode API keys
# BAD: client = OpenAI(api_key="sk-1234567890abcdef")
```

**OAuth 2.0 Integration:**
```python
import requests
from oauthlib.oauth2 import BackendApplicationClient
from requests_oauthlib import OAuth2Session

# Client credentials flow for service-to-service
client = BackendApplicationClient(client_id=CLIENT_ID)
oauth = OAuth2Session(client=client)
token = oauth.fetch_token(
    token_url="https://provider.com/oauth/token",
    client_id=CLIENT_ID,
```

</details>
