---
name: mohitmishra786__low-level-dev-skills__skill
source: https://github.com/mohitmishra786/low-level-dev-skills/blob/6dbfcb393f1bafc31aac9b6572d9cdb49b1269fc/skills/observability/ebpf/SKILL.md
repo: mohitmishra786/low-level-dev-skills
kind: skill
stars: 111
last_pushed: 2026-04-18T20:05:21Z
license: mit
score: 9
domains: [systems-programming, linux-kernel, observability, networking]
tags: [ebpf, linux, tracing, xdp, low-level]
curated: 2026-06-16
curated_by: config-scout
---

# mohitmishra786/low-level-dev-skills — skill

**Why it's worth keeping:** The 'Verifier error triage' table and the decision tree for tool selection are high-value assets that transform an agent from a coder to a debugger.

**Summary:** Provides a comprehensive guide for eBPF development including tool selection, code templates, and networking (XDP) examples.

**Source credibility:** High; the specific technical depth in the verifier/map sections reflects genuine systems expertise.

**Recency:** 

**Source:** [mohitmishra786/low-level-dev-skills/skills/observability/ebpf/SKILL.md](https://github.com/mohitmishra786/low-level-dev-skills/blob/6dbfcb393f1bafc31aac9b6572d9cdb49b1269fc/skills/observability/ebpf/SKILL.md) · 111★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ebpf
description: eBPF skill for Linux observability and networking. Use when writing eBPF programs with libbpf or bpftrace, attaching kprobes/tracepoints/XDP hooks, debugging verifier errors, working with eBPF maps, or achieving CO-RE portability across kernel versions. Activates on queries about eBPF, bpftool, bpftrace, XDP programs, libbpf, verifier errors, eBPF maps, or kernel tracing with BPF.
---

# eBPF

## Purpose

Guide agents through writing, loading, and debugging eBPF programs using libbpf, bpftrace, and bpftool. Covers map types, program types, verifier errors, XDP networking, and CO-RE portability.

## Triggers

- "How do I write an eBPF program to trace system calls?"
- "My eBPF program fails with a verifier error"
- "How do I use bpftrace to trace kernel events?"
- "How do I share data between kernel eBPF and userspace?"
- "How do I write an XDP program for packet filtering?"
- "How do I make my eBPF program portable across kernel versions (CO-RE)?"

## Workflow

### 1. Choose the right tool

```
Goal?
├── One-liner kernel tracing / scripting → bpftrace
├── Production eBPF program with userspace → libbpf (C) or aya (Rust)
├── Inspect loaded programs and ma
```

</details>
