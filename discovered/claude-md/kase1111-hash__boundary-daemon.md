---
name: kase1111-hash__boundary-daemon
source: https://github.com/kase1111-hash/boundary-daemon/blob/cd0c01f5d5a48ac743fcc91271aa8f27cb1b0800/claude.md
repo: kase1111-hash/boundary-daemon
kind: claude-md
stars: 2
last_pushed: 2026-05-29T14:29:20Z
license: gpl-3.0
score: 9
domains: [agents-ai, security, system-programming]
tags: [security-daemon, policy-enforcement, fail-closed, agent-os]
curated: 2026-06-14
curated_by: config-scout
---

# kase1111-hash/boundary-daemon — claude-md

**Why it's worth keeping:** Includes highly effective 'What NOT to Do' negative constraints, provides structured workflows for common tasks, and uses architecture-specific code patterns to enforce security logic.

**Summary:** Defines a rigorous security framework for AI agent boundaries using specific 'modes' and strict behavioral constraints. It bridges high-level philosophy with low-level implementation requirements.

**Source credibility:** High-quality niche project with recent updates; demonstrates deep domain expertise in security-first system design.

**Recency:** Very current; highly optimized for modern LLM context windows and Claude Code's capabilities.

**Source:** [kase1111-hash/boundary-daemon/claude.md](https://github.com/kase1111-hash/boundary-daemon/blob/cd0c01f5d5a48ac743fcc91271aa8f27cb1b0800/claude.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md - Boundary Daemon

## Project Overview

Boundary Daemon (Agent Smith) is a security daemon and cognition boundary control layer for multi-agent AI systems. It's the core trust enforcement system for Agent OS—a natural language operating system for AI agents.

**Core Mission:** Define, enforce, and audit AI boundary policies between cognitive modules. It determines where AI can think, what it can access, and ensures secure agent orchestration.

**Key Question It Answers:** "Where am I allowed to think right now?"

## Architecture

### Core Components

| Component | File | Purpose |
|-----------|------|---------|
| Main Daemon | `daemon/boundary_daemon.py` | Service orchestration, lifecycle management |
| State Monitor | `daemon/state_monitor.py` | Environment sensing at 1Hz (network, hardware, processes) |
| Policy Engine | `daemon/policy_engine.py` | Permission evaluation against boundary modes |
| Tripwires | `daemon/tripwires.py` | Security violation detection, auto-lockdown triggers |
| Event Logger | `daemon/event_logger.py` | Immutable SHA-256 hash-chained audit trail |

### Directory Structure

```
daemon/
├── auth/           # Authentication & ceremony workflows
```

</details>
