---
name: d4n-sec__jdb-mcp
source: https://github.com/d4n-sec/jdb-mcp/blob/88d41e7ca2df74977f82f9c22bc34c0db455c94b/Skill.md
repo: d4n-sec/jdb-mcp
kind: skill
stars: 31
last_pushed: 2026-01-30T10:39:01Z
license: mit
score: 8
domains: [backend, java, debugging, cli-tools]
tags: [java, debugger, mcp, runtime]
curated: 2026-06-14
curated_by: config-scout
---

# d4n-sec/jdb-mcp — skill

**Why it's worth keeping:** It teaches high-level context management techniques, such as using shallow inspection before deep recursion to protect token limits, and establishes a reactive workflow for breakpoint notifications.

**Summary:** Provides a structured operational playbook for an AI agent to debug live Java applications via JDWP using the JDB-MCP server.

**Source credibility:** Niche specialized tool with moderate GitHub interest.

**Recency:** Very current; reflects modern MCP interaction patterns.

**Source:** [d4n-sec/jdb-mcp/Skill.md](https://github.com/d4n-sec/jdb-mcp/blob/88d41e7ca2df74977f82f9c22bc34c0db455c94b/Skill.md) · 31★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Java Debugging Skill for AI Agents (JDB-MCP)

## Role
You are an expert Java Debugger. You use the JDB-MCP server to obtain deep runtime information from Java applications, enabling you to inspect state, trace execution flow, and modify variables in real-time.

## Core Workflows

### 1. Connecting to target VM
- **Attach Mode (Current Focus)**: Use `debug_attach` to connect to a running Java process that has JDWP enabled.
- **Prerequisite**: Ensure the target application is started with: `-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:5005`.

### 2. Strategic Debugging
- **Locate**: Use `debug_set_breakpoint` with the fully qualified `className` and `line` number.
- **Inspect**: When a breakpoint is hit:
    1. Use `debug_list_threads` to identify suspended threads.
    2. Use `debug_list_vars` to get a structured overview of local variables in the current stack frame.
    3. Use `debug_get_var` for deep, recursive inspection of complex objects (adjust `maxDepth` as needed).
- **Trace**: Use `debug_get_stack_trace` to understand the execution path leading to the current state.
- **Modify**: Use `debug_set_var` to change variable values at runtime to test fixes or
```

</details>
