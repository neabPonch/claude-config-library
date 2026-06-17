---
name: abra5umente__api-proxy__skill
source: https://github.com/abra5umente/api-proxy/blob/b5bac79a2be4d10713b0ee51b3590573b234693e/skill/skill.md
repo: abra5umente/api-proxy
kind: skill
stars: 17
last_pushed: 2025-12-31T09:55:32Z
license: mit
score: 7
domains: [agents-ai, cli-tools, api-proxy]
tags: [ip-bypass, residential-proxy, network-fallback, python]
curated: 2026-06-16
curated_by: config-scout
---

# abra5umente/api-proxy — skill

**Why it's worth keeping:** Includes a dual-purpose pattern: an ad-hoc CLI fallback for quick retries and a programmatic helper module template for building complex skills.

**Summary:** Provides instructions and patterns for routing API requests through a residential proxy to bypass cloud IP blocks.

**Source credibility:** Small, specialized niche repository with moderate star count suggesting utility for specific use cases.

**Recency:** Highly relevant as IP reputation/blocking remains a core challenge in agentic workflows.

**Source:** [abra5umente/api-proxy/skill/skill.md](https://github.com/abra5umente/api-proxy/blob/b5bac79a2be4d10713b0ee51b3590573b234693e/skill/skill.md) · 17★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api-proxy
description: Routes API requests through the user's residential proxy to bypass cloud IP blocks. TWO use cases - (1) Runtime fallback when direct curl/fetch fails with 403/blocked errors, use fetch.py for quick retry. (2) Template for building new skills that need proxy routing, copy proxy_helper.py into the new skill.
---

# API Proxy Skill

Routes requests through residential IP via `proxy.address.here.com`.

## Runtime Fallback (ad-hoc)

When a direct request fails with 403 or IP blocking, retry through the proxy:

```bash
# Simple GET
python3 /mnt/skills/user/api-proxy/scripts/fetch.py "https://api.example.com/endpoint"

# POST with body
python3 /mnt/skills/user/api-proxy/scripts/fetch.py "https://api.example.com/endpoint" POST '{"key": "value"}'
```

Returns JSON response or `{"error": "message"}` on failure.

## Template Mode (building skills)

When creating skills that need proxy routing:

1. Copy `proxy_helper.py` into the new skill's `scripts/` folder
2. Import and use:

```python
from proxy_helper import proxy_get, proxy_request

data = proxy_get("https://api.example.com/endpoint")

data = proxy_request(
    url="https://api.example.com/endpoint",
```

</details>
