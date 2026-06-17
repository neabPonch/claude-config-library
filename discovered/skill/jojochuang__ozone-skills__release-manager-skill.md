---
name: jojochuang__ozone-skills__release-manager-skill
source: https://github.com/jojochuang/ozone-skills/blob/7c03a04c23ceed90afc47f115cbd2e1a30a11e25/sherpa/release_manager_skill.md
repo: jojochuang/ozone-skills
kind: skill
stars: 0
last_pushed: 2026-05-30T00:10:44Z
license: unknown
score: 9
domains: [devops, cli-tools, security]
tags: [release-management, safety-protocols, credential-setup]
curated: 2026-06-16
curated_by: config-scout
---

# jojochuang/ozone-skills — skill

**Why it's worth keeping:** It utilizes strict 'Halt & Human-in-the-Loop' protocols and provides granular, multi-step instructions for verifying high-stakes credentials like GPG and SSH through Docker.

**Summary:** A highly structured, safety-centric playbook for managing complex software release lifecycles, including credential verification and environment readiness.

**Source credibility:** High technical depth indicates a specialized engineering background despite low repository visibility.

**Recency:** Current; addresses modern containerized development workflows and security practices.

**Source:** [jojochuang/ozone-skills/sherpa/release_manager_skill.md](https://github.com/jojochuang/ozone-skills/blob/7c03a04c23ceed90afc47f115cbd2e1a30a11e25/sherpa/release_manager_skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: release-manager
description: >-
  Verify environment, sign, and build Apache Ozone releases. Use when performing
  release management, GPG verification, Jira prep, protolock updates, maven staging,
  release candidate builds, or using the Sherpa docker environment.
---

# Apache Ozone Release Manager Agent Playbook & Skill

> [!CAUTION]
> **MANDATORY SAFETY PROTOCOLS — READ BEFORE COMMENCING**
> 1. **100% Confidence Rule:** The Release Manager agent must **ONLY** proceed if it is 100% confident in the current state and execution of a command.
> 2. **Mandatory Halt & Human-in-the-Loop Approval:** The agent **MUST halt execution and ask the user for permission** to proceed if:
>    - Any command fails or returns a non-zero exit code.
>    - Any output, file structure, or system response diverges from the Release Manager Guide.
>    - There is any ambiguity, missing parameter, or environment inconsistency.
> 3. **No Automatic Bypasses:** The agent is strictly forbidden from making guesses, auto-fixing unexpected errors without reporting, or ignoring warnings.

---

## Phase 1: Environment & GPG Keys Verification

### 1.1 GPG Key Autodetect and Setup Guide
Before starting any
```

</details>
