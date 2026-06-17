---
name: k5tuck__RivrQuant
source: https://github.com/k5tuck/RivrQuant/blob/43bff7fa9f1974dc3b6aee5682f5e91a95d04637/Claude.md
repo: k5tuck/RivrQuant
kind: claude-md
stars: 4
last_pushed: 2026-03-05T20:06:45Z
license: unknown
score: 9
domains: [backend-api, fintech]
tags: [context-discovery, multi-repo-orchestration, architectural-alignment]
curated: 2026-06-16
curated_by: config-scout
---

# k5tuck/RivrQuant — claude-md

**Why it's worth keeping:** The 'Step 0' context retrieval script is a brilliant way to give an agent multi-repo intelligence; the 'Identity' section effectively prevents scope creep by explicitly stating what the service does NOT own.

**Summary:** Implements a sophisticated 'Step 0' automated discovery script to clone and inspect related repositories for cross-project architectural patterns. It provides deep system boundaries and strict production-level coding requirements.

**Source credibility:** High-quality source from an active quantitative trading project with complex dependencies.

**Recency:** Very recent (3 months ago), perfectly aligned with modern agentic workflows.

**Source:** [k5tuck/RivrQuant/Claude.md](https://github.com/k5tuck/RivrQuant/blob/43bff7fa9f1974dc3b6aee5682f5e91a95d04637/Claude.md) · 4★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — RivrQuant: Backend Execution Engine for Binelek Risk OS

## Step 0 — Repository Context Retrieval

Before writing ANY code, you need access to existing codebases for context.

**Ask the user for a temporary GitHub personal access token (classic) with `repo` scope.**

Say exactly: "I need a temporary GitHub personal access token to read your repositories
for context. Generate one at https://github.com/settings/tokens with `repo` scope and
paste it here. You can revoke it immediately after this session."

Once you have the token:

```bash
export GITHUB_TOKEN="<paste_token_here>"

# Clone this repo for self-inspection
git clone https://${GITHUB_TOKEN}@github.com/k5tuck/RivrQuant.git /tmp/rq-ref 2>/dev/null || true

# Clone binelek-backend WITH SUBMODULES (it has 11 git submodules — won't work without --recursive)
git clone --recursive https://${GITHUB_TOKEN}@github.com/k5tuck/binelek-backend.git /tmp/bl-ref 2>/dev/null || true
cd /tmp/bl-ref && git submodule update --init --recursive 2>/dev/null; cd -

# ── RIVRQUANT: Read everything ──
echo "=== RQ: Solution ==="
cat $(find /tmp/rq-ref -name "*.sln" | head -1) 2>/dev/null

echo "=== RQ: Domain ==="
for f in $(find /tmp/
```

</details>
