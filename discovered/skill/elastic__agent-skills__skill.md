---
name: elastic__agent-skills__skill
source: https://github.com/elastic/agent-skills/blob/e0d6b02194d4ec74cf9e5975290e950fc5ba549f/skills/cloud/network-security/SKILL.md
repo: elastic/agent-skills
kind: skill
stars: 504
last_pushed: 2026-06-01T14:43:57Z
license: apache-2.0
score: 9
domains: [cloud-infrastructure, security-ops, api-integration]
tags: [network-security, elastic-cloud, agentic-reasoning]
curated: 2026-06-15
curated_by: config-scout
---

# elastic/agent-skills — skill

**Why it's worth keeping:** Includes a high-quality 'Decomposing Requests' section that provides the agent with a logical chain-of-thought pattern; also contains excellent protocols for environment variable management and error handling.

**Summary:** Instructions for an agent to manage IP and VPC network security filters within Elastic Cloud Serverless.

**Source credibility:** High; this is an official skill set from Elastic, well-maintained and highly starred.

**Recency:** Current; follows modern agentic reasoning patterns suitable for Claude Code.

**Source:** [elastic/agent-skills/skills/cloud/network-security/SKILL.md](https://github.com/elastic/agent-skills/blob/e0d6b02194d4ec74cf9e5975290e950fc5ba549f/skills/cloud/network-security/SKILL.md) · 504★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cloud-network-security
description: >
  Manage Serverless network security (traffic filters): create, update, and delete
  IP filters and AWS PrivateLink VPC filters. Use when restricting network access
  or configuring private connectivity.
compatibility: >
  Requires Python 3.8+, network access to the Elastic Cloud API (api.elastic-cloud.com).
  Environment variables: EC_API_KEY (required, set by cloud-setup), EC_BASE_URL (optional,
  defaults to https://api.elastic-cloud.com).
metadata:
  author: elastic
  version: 0.1.0
---

# Cloud Network Security

Manage network security policies for Elastic Cloud Serverless projects: IP filters to allowlist specific IPs or CIDRs,
and VPC filters (AWS PrivateLink) to restrict traffic to specific VPC endpoints.

> **Prerequisite:** This skill assumes the **cloud-setup** skill has already run — `EC_API_KEY` is set in the
> environment and the organization context is established. If `EC_API_KEY` is missing, instruct the agent to invoke
> **cloud-setup** first. Do NOT prompt the user for an API key directly.

For project creation and day-2 operations (including associating filters with projects), see **cloud-create-project**
and **clou
```

</details>
