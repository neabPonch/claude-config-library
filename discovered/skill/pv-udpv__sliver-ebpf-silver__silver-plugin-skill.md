---
name: pv-udpv__sliver-ebpf-silver__silver-plugin-skill
source: https://github.com/pv-udpv/sliver-ebpf-silver/blob/7d01d963de57bdf821247223696dbab6cbafe042/silver-plugin.skill.md
repo: pv-udpv/sliver-ebpf-silver
kind: skill
stars: 0
last_pushed: 2026-04-18T16:53:30Z
license: unknown
score: 9
domains: [security, systems-programming, observability, linux]
tags: [ebpf, network, security-tooling, grpc]
curated: 2026-06-16
curated_by: config-scout
---

# pv-udpv/sliver-ebpf-silver — skill

**Why it's worth keeping:** Provides an exceptional template for multi-component skills by explicitly mapping the relationship between low-level hooks (programs), data structures (maps), and high-level interfaces (gRPC).

**Summary:** Defines a complex eBPF-driven network observability extension that correlates low-level kernel events with process identity via gRPC.

**Source credibility:** Low social proof/stars, but demonstrates high technical depth characteristic of real security engineering.

**Recency:** Highly current; uses modern eBPF patterns like cgroup/sock_create and ring buffers.

**Source:** [pv-udpv/sliver-ebpf-silver/silver-plugin.skill.md](https://github.com/pv-udpv/sliver-ebpf-silver/blob/7d01d963de57bdf821247223696dbab6cbafe042/silver-plugin.skill.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: silver-network-plugin
version: 0.1.0
description: >
  Silver — Full packet accountability plugin for Sliver C2 / E2B sandboxes.
  Correlates every packet in/out to the originating process, protocol used,
  purpose, and target. No dark corners. Implemented as a Sliver extension
  backed by 6 eBPF programs sharing 7 BPF maps.
author: pv-udpv
tags: [ebpf, network, security, sliver, c2, observability, e2b, sandbox, grpc]
requires:
  - linux-kernel: ">=5.15"
  - btf: true
  - capabilities: [CAP_BPF, CAP_NET_ADMIN, CAP_SYS_ADMIN]
  - tools: [clang, bpftool, protoc, go]

components:
  bpf_programs:
    - name: silver_sock_create
      type: cgroup/sock_create
      attach: /sys/fs/cgroup
      purpose: Capture process identity (PID, comm, cgroup) at socket birth
      
    - name: silver_connect4
      type: cgroup/connect4
      attach: /sys/fs/cgroup
      purpose: Record outbound connection intent with destination and process

    - name: silver_sock_ops
      type: sockops
      attach: /sys/fs/cgroup
      purpose: Track TCP lifecycle (SYN, ESTABLISHED, FIN) with state callbacks

    - name: silver_xdp
      type: xdp
      attach: ${SILVER_IFACE:-eth0}
      purpose: Fast-
```

</details>
