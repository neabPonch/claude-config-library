---
name: LinuxSuRen__api-testing__claude-skill
source: https://github.com/LinuxSuRen/api-testing/blob/80189da964f2d4f7227bba4949ed095b844bfcda/claude-skill.md
repo: LinuxSuRen/api-testing
kind: skill
stars: 367
last_pushed: 2026-04-03T13:24:43Z
license: apache-2.0
score: 9
domains: [api-testing, cli-tools, devops, backend]
tags: [atest, api-testing, load-testing, grpc, docker]
curated: 2026-06-15
curated_by: config-scout
---

# LinuxSuRen/api-testing — skill

**Why it's worth keeping:** The inclusion of a 'Pre-Test Execution Checklist' is brilliant; it instructs the agent on how to orchestrate environments using Docker Compose, verify service health, and handle environment variables before executing tests.

**Summary:** This skill provides a specialized persona for using the 'atest' CLI to manage multi-protocol API testing and load testing via YAML suites.

**Source credibility:** Highly credible; the source tool has significant community traction (367 stars) and recent maintenance.

**Recency:** 

**Source:** [LinuxSuRen/api-testing/claude-skill.md](https://github.com/LinuxSuRen/api-testing/blob/80189da964f2d4f7227bba4949ed095b844bfcda/claude-skill.md) · 367★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# API Testing Skill (atest)

> **Claude Code Skill for api-testing (atest)**
> This skill helps you create, manage, and debug API test suites using the [api-testing](https://github.com/LinuxSuRen/api-testing) tool.

## How to Use This Skill

1. Copy this skill file to your Claude skills directory:
   ```bash
   # On macOS/Linux
   cp claude-skill.md ~/.claude/skills/api-testing.md

   # On Windows
   copy claude-skill.md %USERPROFILE%\.claude\skills\api-testing.md
   ```

2. Restart Claude Code to load the skill

3. Use trigger phrases like:
   - "create an API test suite"
   - "write a test for API"
   - "create grpc test"
   - "API load testing"
   - "mock API server"

## What is api-testing (atest)?

[api-testing](https://github.com/LinuxSuRen/api-testing) is a comprehensive API testing framework that supports:

- **Multi-protocol**: HTTP/REST, gRPC, GraphQL
- **Load Testing**: Duration-based, thread-based, QPS-based
- **Mock Server**: Create mock APIs from test suites
- **Code Generation**: Generate test code in Go, Python, Java, JavaScript
- **Multiple Reports**: Markdown, HTML, PDF, JSON, Prometheus
- **Web UI**: Built-in interface for test management

## Description

You are
```

</details>
