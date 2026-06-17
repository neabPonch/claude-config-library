---
name: g1157__spider2__claude
source: https://github.com/g1157/spider2/blob/4a6b9e9f5302d53ee5df1ec48ecc36a53275b3ea/methods/spider-agent-lite/CLAUDE.md
repo: g1157/spider2
kind: claude-md
stars: 0
last_pushed: 2026-01-23T07:02:46Z
license: mit
score: 8
domains: [agents-ai, data-engineering]
tags: [benchmark, text-to-sql, agent-framework]
curated: 2026-06-15
curated_by: config-scout
---

# g1157/spider2 — claude-md

**Why it's worth keeping:** The 'External Interfaces' table effectively maps available tool actions to descriptions, which is crucial context for an AI assistant; the explicit command templates facilitate error-free runtime operations.

**Summary:** Provides highly specific setup, execution, and evaluation workflows for a specialized text-to-SQL agent benchmark environment.

**Source credibility:** Low visibility (0 stars), likely a specialized research or individual project.

**Recency:** Extremely current (dated January 2026).

**Source:** [g1157/spider2/methods/spider-agent-lite/CLAUDE.md](https://github.com/g1157/spider2/blob/4a6b9e9f5302d53ee5df1ec48ecc36a53275b3ea/methods/spider-agent-lite/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
[Root](../../CLAUDE.md) > [methods](../) > **spider-agent-lite**

# spider-agent-lite

## Module Purpose

Docker-based agent framework for Spider 2.0-Lite benchmark. Handles text-to-SQL tasks across multiple database backends: BigQuery, Snowflake, and local SQLite databases.

## Entry and Startup

- **Main Entry**: `run.py`
- **Agent Logic**: `spider_agent/agent/agents.py` (PromptAgent class)
- **Environment**: `spider_agent/envs/spider_agent.py`
- **Setup Script**: `spider_agent_setup_lite.py`

### Setup Process

```bash
# Download local databases
gdown 'https://drive.google.com/uc?id=1coEVsCZq-Xvj9p2TnhBFoFTsY-UoYGmG' -O ../../spider2-lite/resource/
unzip ../../spider2-lite/resource/local_sqlite.zip -d ../../spider2-lite/resource/databases/spider2-localdb

# Configure credentials
# Update bigquery_credential.json and snowflake_credential.json

# Run setup
python spider_agent_setup_lite.py
```

### Running the Agent

```bash
export OPENAI_API_KEY=your_key
python run.py --model gpt-4o -s experiment_name
```

## External Interfaces

### Action Classes

| Action | Description |
|--------|-------------|
| `Bash` | Execute shell commands |
| `Terminate` | Complete task with result |
|
```

</details>
