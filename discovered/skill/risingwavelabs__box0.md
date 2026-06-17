---
name: risingwavelabs__box0
source: https://github.com/risingwavelabs/box0/blob/66be3af827f27ce87fce885ac0a4c3b85d0aeb81/SKILL.md
repo: risingwavelabs/box0
kind: skill
stars: 79
last_pushed: 2026-04-06T18:30:31Z
license: mit
score: 8
domains: [agents-ai, cli-tools, orchestration]
tags: [multi-agent, parallelism, delegation]
curated: 2026-06-14
curated_by: config-scout
---

# risingwavelabs/box0 — skill

**Why it's worth keeping:** The 'How to write task prompts' section teaches the LLM to synthesize context (like git diffs) rather than blindly forwarding user input. It also provides clear patterns for parallel execution and error handling.

**Summary:** Provides a protocol for Claude Code to delegate tasks to the Box0 multi-agent platform via CLI.

**Source credibility:** Rising Wave Labs is an active open-source contributor with a specialized focus on agentic platforms.

**Recency:** Very current; updated 2 months ago, highly relevant to modern agent orchestration workflows.

**Source:** [risingwavelabs/box0/SKILL.md](https://github.com/risingwavelabs/box0/blob/66be3af827f27ce87fce885ac0a4c3b85d0aeb81/SKILL.md) · 79★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: b0
description: |
  Delegate tasks to AI agents via Box0. Use when the user asks to
  review code, check security, run tests, compare tools, get multiple
  perspectives, research a topic, analyze data, write docs, or any
  task that could benefit from specialized or parallel execution.
  Also use when the user mentions agent names or says "ask", "delegate",
  "get opinions from", or "have someone".
allowed-tools:
  - Bash
---

# Box0 (`b0`) Multi-Agent Platform

Run AI agents in parallel. Create agents with roles, trigger them on demand or on a schedule, and collect results.

## Setup

### Step 1: Check if Box0 is installed

```bash
b0 --version
```

If this succeeds, skip to Step 3.

### Step 2: Install

```bash
npm install -g @box0/cli@latest
```

If npm is not available, build from source:

```bash
git clone https://github.com/risingwavelabs/box0.git
cd box0 && cargo build --release
export PATH="$PWD/target/release:$PATH"
```

### Step 3: Check if server is running

```bash
b0 server status
```

If this shows "Server is running", skip to Step 5.

### Step 4: Start the server

```bash
b0 server
```

On first start, Box0 creates an admin account and auto-configures `~/.b
```

</details>
