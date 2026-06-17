---
name: abdomohamed__Leashd
source: https://github.com/abdomohamed/Leashd/blob/0da9e0a9987c42ce35e0b6c159ff2c12ec9790e7/CLAUDE.md
repo: abdomohamed/Leashd
kind: claude-md
stars: 2
last_pushed: 2026-04-01T18:38:13Z
license: mit
score: 9
domains: [cli-tools, security, systems-programming, linux]
tags: [ebpf, go, security, linux-kernel]
curated: 2026-06-15
curated_by: config-scout
---

# abdomohamed/Leashd — claude-md

**Why it's worth keeping:** The 'Key Gotchas' section proactively solves environment/permission issues, while the architectural breakdown of goroutines and BPF layers enables sophisticated reasoning about system behavior.

**Summary:** Provides comprehensive technical context for a complex eBPF-based security project, including detailed build, test, and release workflows.

**Source credibility:** Niche systems-level tool with high technical density and recent activity.

**Recency:** Highly current; addresses modern Linux kernel requirements and eBPF workflows.

**Source:** [abdomohamed/Leashd/CLAUDE.md](https://github.com/abdomohamed/Leashd/blob/0da9e0a9987c42ce35e0b6c159ff2c12ec9790e7/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What This Project Does

Leashd is a per-project eBPF-based network firewall that enforces domain/IP allowlists at the kernel level. It wraps a child process in a cgroup and uses eBPF kprobes + cgroup/skb filters to detect and block unexpected outbound connections.

## Build Commands

```bash
make build        # Generate BPF objects + build binary (requires clang, llvm, libbpf-dev)
make generate     # Re-run bpf2go to regenerate internal/bpf/leashd_bpf*.go from ebpf/leashd.c
make vmlinux      # Regenerate ebpf/headers/vmlinux.h from running kernel (rarely needed)
make lint         # Run golangci-lint
make release-local # GoReleaser snapshot build (no publish, artifacts in dist/)
make clean        # Remove binaries and generated eBPF objects
```

`vmlinux.h` is pre-committed; do not regenerate it unless intentionally targeting a different kernel ABI.

## Test Commands

```bash
# Unit tests — no root required
make test
go test ./internal/... -v -run TestFooBar

# Integration tests — requires root, no eBPF kernel needed
make test-int
sudo -E env PATH="$PATH" go test -
```

</details>
