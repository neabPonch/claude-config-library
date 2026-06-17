---
name: spring-ai-community__agent-client
source: https://github.com/spring-ai-community/agent-client/blob/d086dde4251082db70fdd214f21d0c3e2f6910cb/CLAUDE.md
repo: spring-ai-community/agent-client
kind: claude-md
stars: 102
last_pushed: 2026-04-30T03:02:48Z
license: other
score: 9
domains: [cli-tools, agents-ai, java, devops]
tags: [workarounds, multi-module, maven, architecture]
curated: 2026-06-16
curated_by: config-scout
---

# spring-ai-community/agent-client — claude-md

**Why it's worth keeping:** Includes a critical workaround for nested process tree detection using `systemd-run`, which is a highly transferable 'edge case' instruction. It also provides deep architectural patterns that aid LLM reasoning beyond simple command lists.

**Summary:** Provides high-density technical workarounds for tool-specific limitations and detailed build/architectural context.

**Source credibility:** High; part of the Spring AI ecosystem with active maintenance.

**Recency:** Very current, addressing specific Claude Code version limitations (2.1.39+).

**Source:** [spring-ai-community/agent-client/CLAUDE.md](https://github.com/spring-ai-community/agent-client/blob/d086dde4251082db70fdd214f21d0c3e2f6910cb/CLAUDE.md) · 102★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## CRITICAL: Running Claude CLI Subprocesses from Claude Code

Claude Code 2.1.39+ blocks nested `claude` invocations via process tree detection. Any command that spawns `claude` CLI as a subprocess (Maven IT tests, SDK tests) will fail silently with empty output or `[Tool result missing due to internal error]`.

**Use `~/scripts/claude-run.sh`** to run Maven builds that invoke Claude CLI:
```bash
~/scripts/claude-run.sh ./mvnw test -pl agent-models/spring-ai-claude-agent -Dtest="ClaudeAgentMcpIT"
```
The script uses `systemd-run` to escape the process tree. It works for Maven/Gradle builds (where claude is invoked indirectly via the SDK). See `~/scripts/claude-run.sh` for details.

## Build and Development Commands

### Basic Commands
- `./mvnw clean compile` - Compile all modules
- `./mvnw clean test` - Run unit tests
- `./mvnw clean verify` - Run full build including integration tests
- `./mvnw clean install` - Install artifacts to local repository
- `./mvnw spring-boot:run` - Run sample applications (from sample directories)

### Integration Tests
- `./mvnw clean
```

</details>
