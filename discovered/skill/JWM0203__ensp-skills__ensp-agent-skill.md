---
name: JWM0203__ensp-skills__ensp-agent-skill
source: https://github.com/JWM0203/ensp-skills/blob/c09c244ba4d6dd45785df698e564e6df383af9d8/ensp-agent.skill.md
repo: JWM0203/ensp-skills
kind: skill
stars: 33
last_pushed: 2026-03-12T16:53:40Z
license: mit
score: 8
domains: [network-engineering, infrastructure-automation]
tags: [huawei, ensp, telnet, cli-automation]
curated: 2026-06-15
curated_by: config-scout
---

# JWM0203/ensp-skills — skill

**Why it's worth keeping:** It provides highly specific, 'low-level' instructions—such as repeating the `sys` command multiple times—to handle hardware state transitions that generic automation often fails to address.

**Summary:** An automated workflow for discovering, connecting to, and configuring Huawei network devices within the eNSP simulator using Telnet.

**Source credibility:** Decent; 33 stars indicates a useful specialized tool in its niche.

**Recency:** Current; explicitly addresses Python 3.13 compatibility issues.

**Source:** [JWM0203/ensp-skills/ensp-agent.skill.md](https://github.com/JWM0203/ensp-skills/blob/c09c244ba4d6dd45785df698e564e6df383af9d8/ensp-agent.skill.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# eNSP Network Device Configuration Agent Skill

This skill provides an automated workflow for configuring Huawei network devices in eNSP simulator. It guides through the entire process: topology discovery, device connection, and configuration deployment.

## Workflow Overview

```
┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
│  Step 1         │     │  Step 2         │     │  Step 3         │     │  Step 4         │
│  Discover Topo  │ --> │  Connect Device │ --> │  Configure      │ --> │  Verify Config  │
│  (Read Only)    │     │  (User Input)   │     │  (Apply Config) │     │  (Validate)     │
└─────────────────┘     └─────────────────┘     └─────────────────┘     └─────────────────┘
```

## Prerequisites

### Python Environment

This project uses Python 3.13 with conda. Run Python directly:

```bash
# Windows - Direct Python path
C:/ProgramData/miniconda3/python.exe <script>.py

# Or activate conda environment first
conda activate base
python <script>.py
```

**Note**: Python 3.13 removed the `telnetlib` module. This project uses a custom `socket`-based Telnet client implementation.

### eNSP Device Connection

eNSP devices can be
```

</details>
