---
name: redpanda-data__connect__skill
source: https://github.com/redpanda-data/connect/blob/6a3627b34e03a1a194be6ad8c320cac126b9ccd3/.claude-plugin/plugins/redpanda-connect/skills/pipeline-assistant/SKILL.md
repo: redpanda-data/connect
kind: skill
stars: 8679
last_pushed: 2026-06-13T23:06:38Z
license: unknown
score: 9
domains: [cli-tools, data-engineering, devops]
tags: [streaming, yaml, pipeline, redpanda]
curated: 2026-06-15
curated_by: config-scout
---

# redpanda-data/connect — skill

**Why it's worth keeping:** It uses high-level delegation to specialized skills (discovery vs. transformation) and provides a clear, testable workflow of 'scaffold -> lint -> run'.

**Summary:** An orchestrator skill for creating, validating, and executing Redpanda Connect stream processing pipelines via CLI.

**Source credibility:** Very high; sourced from the official Redpanda repository which is highly starred and actively maintained.

**Recency:** 

**Source:** [redpanda-data/connect/.claude-plugin/plugins/redpanda-connect/skills/pipeline-assistant/SKILL.md](https://github.com/redpanda-data/connect/blob/6a3627b34e03a1a194be6ad8c320cac126b9ccd3/.claude-plugin/plugins/redpanda-connect/skills/pipeline-assistant/SKILL.md) · 8679★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pipeline-assistant
description: This skill should be used when users need to create or fix Redpanda Connect pipeline configurations. Trigger when users mention "config", "pipeline", "YAML", "create a config", "fix my config", "validate my pipeline", or describe a streaming pipeline need like "read from Kafka and write to S3".
---

# Redpanda Connect Configuration Assistant

Create working, validated Redpanda Connect configurations from scratch or repair existing configurations that have issues.

**This skill REQUIRES skills: `component-search`, `bloblang-authoring`.**

## Objective

Deliver a complete, valid YAML configuration that passes validation and meets the user's requirements.
Whether starting from a description or fixing a broken config, the result must be production-ready with properly secured credentials.

Handle Two Scenarios:
**Creation** - User provides description like "Read from Kafka on localhost:9092 topic 'events' to stdout"
**Repair** - User provides config file path and optional error context

This skill focuses ONLY on pipeline configuration orchestration and validation.

**Skill Delegation**:

NEVER directly use component-search or bloblang-authoring
```

</details>
