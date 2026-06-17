---
name: Codebrahma__guardian_shell
source: https://github.com/Codebrahma/guardian_shell/blob/9d720ab9d2360a740c4d62cea786e268dbfe3a3e/CLAUDE.md
repo: Codebrahma/guardian_shell
kind: claude-md
stars: 1
last_pushed: 2026-04-03T10:18:13Z
license: apache-2.0
score: 8
domains: [security, systems-programming, linux, rust]
tags: [ebpf, architecture-handoff, security-hardening]
curated: 2026-06-15
curated_by: config-scout
---

# Codebrahma/guardian_shell — claude-md

**Why it's worth keeping:** It provides deep technical reasoning for complex security decisions (e.g., Landlock vs eBPF), which prevents the AI from introducing regression vulnerabilities during refactoring or new feature implementation.

**Summary:** A highly detailed architectural handoff document that tracks development phases and granular security enforcement logic.

**Source credibility:** Niche specialized tool; content demonstrates high-level systems programming expertise.

**Recency:** Highly current, reflecting modern Linux/Rust/eBPF development patterns.

**Source:** [Codebrahma/guardian_shell/CLAUDE.md](https://github.com/Codebrahma/guardian_shell/blob/9d720ab9d2360a740c4d62cea786e268dbfe3a3e/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Guardian Shell - Claude Agent Handoff Document

This document provides everything a Claude agent needs to continue development
on this project on a Linux machine.

## Project Summary

Guardian Shell is a Linux security tool that uses eBPF to monitor and restrict
LLM agent activities. It's built with Rust and the Aya eBPF framework.

**Current state: Phase 11 - Security Hardening & Performance (compiled on Linux)**

Phase 10 introduces **defense-in-depth for cgroup agents** — a creative architectural shift that solves all CRITICAL and HIGH security vulnerabilities by using the right enforcement tool for each layer:

- **Landlock LSM sandbox** (Linux 5.13+): Inode-level file access control applied in `guardian-launch` before exec. Resolves symlinks at kernel VFS layer — completely immune to the #1 CRITICAL symlink bypass. Default-deny model mirrors agent policy.
- **Expanded seccomp filter**: Blocks mount (165-166), namespace escape (setns 308, unshare 272), chroot (161), pivot_root (155), and new mount API (428-433, 442) in addition to existing io_uring and memfd_create blocks.
- **PR_SET_NO_NEW_PRIVS**: Prevents SUID privilege escalation. Required by Landlock, good practice regar
```

</details>
