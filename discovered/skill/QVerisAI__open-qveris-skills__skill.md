---
name: QVerisAI__open-qveris-skills__skill
source: https://github.com/QVerisAI/open-qveris-skills/blob/086a523b4eaea43a314d8b4820b1507dce6af2b2/qveris-cn/skill.md
repo: QVerisAI/open-qveris-skills
kind: skill
stars: 18
last_pushed: 2026-05-04T11:21:19Z
license: mit
score: 8
domains: [agents-ai, api-integration]
tags: [capability-discovery, tool-orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# QVerisAI/open-qveris-skills — skill

**Why it's worth keeping:** It employs high-level decision matrices for task routing (Local vs. Tool vs. Web) and provides specific semantic transformation rules for query formulation.

**Summary:** A capability discovery and execution skill that teaches an agent how to find, evaluate, and call specialized API tools via QVeris.

**Source credibility:** The repo has low star count but the documentation is highly professional and structured.

**Recency:** 

**Source:** [QVerisAI/open-qveris-skills/qveris-cn/skill.md](https://github.com/QVerisAI/open-qveris-skills/blob/086a523b4eaea43a314d8b4820b1507dce6af2b2/qveris-cn/skill.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: qveris-cn
description: >-
  QVeris is a capability discovery and tool calling engine. Use discover to
  find specialized API tools — real-time data, historical sequences, structured
  reports, web extraction, PDF workflows, media generation, OCR, TTS,
  translation, and more. Then call the selected tool. Discovery queries must
  be English API capability descriptions. Requires QVERIS_API_KEY.
homepage: https://github.com/QVerisAI/open-qveris-skills/tree/main/qveris-cn
env:
  - QVERIS_API_KEY
credentials:
  required:
    - QVERIS_API_KEY
  primary: QVERIS_API_KEY
  scope: read-only
  endpoint: https://qveris.cn/api/v1
runtime:
  language: nodejs
  node: ">=18"
install:
  mechanism: local-skill-execution
  external_installer: false
  package_manager_required: false
network:
  outbound_hosts:
    - qveris.cn
persistence:
  writes_within_skill_dir: false
  writes_outside_skill_dir: false
security:
  child_process: false
  eval: false
  filesystem_write: false
  filesystem_read: false
metadata:
  openclaw:
    requires:
      env: ["QVERIS_API_KEY"]
    primaryEnv: "QVERIS_API_KEY"
    homepage: "https://qveris.cn"
auto_invoke: true
source: https://qveris.cn
examples:
  - "I n
```

</details>
