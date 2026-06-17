---
name: stephnangue__warden__skill
source: https://github.com/stephnangue/warden/blob/5a9a9c9835bce916a8f27b0eb8673a11bce9207f/provider/ansible_tower/skill.md
repo: stephnangue/warden
kind: skill
stars: 130
last_pushed: 2026-06-15T17:43:03Z
license: mpl-2.0
score: 9
domains: [devops, security, infrastructure-automation]
tags: [ansible-tower, api-proxy, secure-gateway]
curated: 2026-06-15
curated_by: config-scout
---

# stephnangue/warden — skill

**Why it's worth keeping:** The 'Quirks' section is a masterclass in detail, highlighting critical foot-guns like trailing slash requirements and path prefix variations that prevent agent failure. It also establishes an excellent pattern for credential-less authentication via a middleware role system.

**Summary:** Provides precise instructions for interacting with Ansible Tower through the Warden secure gateway proxy.

**Source credibility:** High; the repository shows active maintenance and has significant community interest (130 stars).

**Recency:** Very current, addressing modern security concerns regarding AI agents accessing enterprise infrastructure.

**Source:** [stephnangue/warden/provider/ansible_tower/skill.md](https://github.com/stephnangue/warden/blob/5a9a9c9835bce916a8f27b0eb8673a11bce9207f/provider/ansible_tower/skill.md) · 130★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ansible_tower
description: "Call the Ansible Tower / AWX / AAP REST API through Warden — launch job templates, read inventories, check job status — without holding a PAT."
category: provider-guide
provider: ansible_tower
requires: [foundation, discovery]
upstream: Ansible Tower / AWX / AAP REST API (api/v2)
---

# Ansible Tower through Warden

## What it does

Warden proxies Ansible Tower REST API requests. The agent calls a
Warden URL; Warden authenticates the caller (JWT/cert), looks up the
Ansible Tower Personal Access Token bound to the chosen role, injects
it as `Authorization: Bearer <pat>`, and forwards to Tower. The agent
**never holds a PAT**.

## Configure the CLI/SDK

`<mount-url>` and `<role>` below come from the discovery flow:
- `<mount-url>` is the chosen provider's `mount_url` from
  `warden provider list` (e.g. `/v1/ansible_tower/`,
  `/v1/team-ops/tower-prod/`). Warden has already baked the namespace
  + mount path in.
- `<role>` is the role you picked from `warden role list` to perform
  this task — it goes in the URL path.

```bash
URL pattern : $WARDEN_ADDR<mount-url>role/<role>/gateway/api/v2/<endpoint>
Auth header : Authorization: Bearer $WARDEN_TOK
```

</details>
