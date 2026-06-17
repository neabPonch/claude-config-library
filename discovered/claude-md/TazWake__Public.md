---
name: TazWake__Public
source: https://github.com/TazWake/Public/blob/9a0cb2cd1f9afdbfd79bcc27d93949689e646a03/CLAUDE.md
repo: TazWake/Public
kind: claude-md
stars: 43
last_pushed: 2026-06-14T00:30:11Z
license: cc0-1.0
score: 9
domains: [security, cli-tools, devops]
tags: [dfir, cross-platform, docker, forensics]
curated: 2026-06-15
curated_by: config-scout
---

# TazWake/Public — claude-md

**Why it's worth keeping:** Includes critical cross-platform side-effect warnings (like PowerShell vs. Bash redirection) and provides highly specific command templates for complex toolchains.

**Summary:** Provides high-fidelity environmental context for a hybrid Windows/WSL2/Docker DFIR workflow.

**Source credibility:** Publicly maintained repository with active commits and established star count.

**Recency:** Extremely current; addresses modern containerized workflows and recent forensic framework versions.

**Source:** [TazWake/Public/CLAUDE.md](https://github.com/TazWake/Public/blob/9a0cb2cd1f9afdbfd79bcc27d93949689e646a03/CLAUDE.md) · 43★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a comprehensive DFIR (Digital Forensics and Incident Response) tools repository containing production-ready forensic analysis scripts, containerized lab environments, and specialized plugins for memory analysis frameworks.

## Environment Notes

- **Host Environment**: Windows with PowerShell (not Linux)
- **WSL2 Access**: Bash is available via WSL2 for Linux-specific commands
- **CRITICAL**: Avoid piping output to `nul` - this creates a file in Windows that breaks git push and other commands. Use `>$null` in PowerShell or `>/dev/null` in WSL2/bash instead.
- **Container Development**: Use Docker for Linux-specific testing and tools
- **Cross-Platform Compatibility**: Bash scripts are designed for Linux/macOS execution or WSL2
- **Building**: Request assistance for compilation if cross-platform issues occur

## Code Best Practices

### General Guidelines
- Always use descriptive variable names unless specifically asked to create obfuscated code
- If an instruction is unclear or impossible to complete without more information, ask questions
- Foll
```

</details>
