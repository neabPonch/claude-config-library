---
name: Wscats__bilibili-all-in-one
source: https://github.com/Wscats/bilibili-all-in-one/blob/ebf24a4a4cf0616162353b4765f0fa5aab931d2a/skill.md
repo: Wscats/bilibili-all-in-one
kind: skill
stars: 16
last_pushed: 2026-05-02T07:16:08Z
license: mit
score: 9
domains: [media-automation, api-integration, cli-tools]
tags: [bilibili, video-automation, api-wrapper]
curated: 2026-06-14
curated_by: config-scout
---

# Wscats/bilibili-all-in-one — skill

**Why it's worth keeping:** The 'Trigger Scenarios' table provides an elite template for intent-based activation, while the granular security section sets a gold standard for handling sensitive session credentials.

**Summary:** A comprehensive Bilibity automation toolkit covering monitoring, downloading, and publishing via official APIs.

**Source credibility:** Decent; 16 stars and very recently updated (1 month ago).

**Recency:** Highly current; follows sophisticated agentic tool-definition patterns.

**Source:** [Wscats/bilibili-all-in-one/skill.md](https://github.com/Wscats/bilibili-all-in-one/blob/ebf24a4a4cf0616162353b4765f0fa5aab931d2a/skill.md) · 16★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: bilibili-all-in-one
description: >
  A comprehensive Bilibili toolkit that integrates hot trending monitoring,
  video downloading, video watching/playback, subtitle downloading,
  and video publishing capabilities into a single unified skill.
  Supports Bilibili session cookie authentication for publishing and
  high-quality downloads. Requests go to official Bilibili API endpoints
  over HTTPS.
version: 1.0.18
type: code
implementation: python
interface: cli-and-api
runtime: python>=3.8
languages:
  - zh-CN
  - en
tags:
  - bilibili
  - video-download
  - hot-trending
  - subtitle
  - danmaku
  - video-publish
  - video-player

  - batch-download
  - multi-format
author: wscats
license: MIT
homepage: https://github.com/wscats/bilibili-all-in-one
repository: https://github.com/wscats/bilibili-all-in-one
entry_point: main.py
required_env_vars: []
optional_env_vars:
  - BILIBILI_SESSDATA
  - BILIBILI_BILI_JCT
  - BILIBILI_BUVID3
  - BILIBILI_PERSIST
install: pip install -r requirements.txt
---

# Bilibili All-in-One Skill

A comprehensive Bilibili toolkit that integrates hot trending monitoring, video downloading, video watching/playback, subtitle downloading, and video pu
```

</details>
