---
name: OpenNHP__opennhp
source: https://github.com/OpenNHP/opennhp/blob/69a428d7dbacbc2f6680ea0f9b5c7cced5fa7e71/CLAUDE.md
repo: OpenNHP/opennhp
kind: claude-md
stars: 13797
last_pushed: 2026-06-12T12:57:13Z
license: apache-2.0
score: 9
domains: [security, systems-programming, go, infrastructure]
tags: [build-guide, formatting-rules, architecture, go]
curated: 2026-06-14
curated_by: config-scout
---

# OpenNHP/opennhp — claude-md

**Why it's worth keeping:** Excellent use of actionable guardrails (signed commits) and highly detailed formatting standards to prevent CI failures. The architecture section maps out the entire system's data structures and module relationships, which is vital for complex codebases.

**Summary:** Provides a comprehensive technical manual covering build commands, rigorous Go formatting/import rules, and deep architectural context. It also includes specific deployment-related secret schemas for infrastructure management.

**Source credibility:** Highly credible; the repository is widely recognized with high star counts and active maintenance.

**Recency:** Extremely current, reflecting modern Go development practices and recent project updates.

**Source:** [OpenNHP/opennhp/CLAUDE.md](https://github.com/OpenNHP/opennhp/blob/69a428d7dbacbc2f6680ea0f9b5c7cced5fa7e71/CLAUDE.md) · 13797★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

OpenNHP is a Go-based Zero Trust security toolkit implementing two core protocols:
- **NHP (Network-infrastructure Hiding Protocol)**: Conceals server ports, IPs, and domains from unauthorized access
- **DHP (Data-content Hiding Protocol)**: Ensures data security via encryption and confidential computing

The system follows NIST Zero Trust Architecture with three core components that communicate via encrypted UDP packets using the Noise Protocol Framework.

## Git Commit Requirements

All commits must be signed with a verified GPG or SSH key. Unsigned commits will fail CI checks.

```bash
# Sign commits (if not configured globally)
git commit -S -m "your message"

# Amend to sign an existing commit
git commit --amend --no-edit -S
```

## Build Commands

```bash
# Full build (all components + SDKs + plugins + archive)
make

# Build individual components
make agentd      # Build nhp-agent daemon
make serverd     # Build nhp-server daemon
make acd         # Build nhp-ac (access controller) daemon
make db          # Build nhp-db daemon
make kgc
```

</details>
