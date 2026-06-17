---
name: NVIDIA__skills__skill
source: https://github.com/NVIDIA/skills/blob/5b2a1e80d0e03fc3c9f60e69a727cdfcc9ab8d4c/skills/tao-setup-nvidia-gpu-host/SKILL.md
repo: NVIDIA/skills
kind: skill
stars: 1269
last_pushed: 2026-06-15T05:53:35Z
license: other
score: 9
domains: [devops, infrastructure, ml-ops, cli-tools]
tags: [nvidia, cuda, linux, setup, gpu]
curated: 2026-06-15
curated_by: config-scout
---

# NVIDIA/skills — skill

**Why it's worth keeping:** Implements a critical 'check-then-install' pattern that prevents unauthorized changes; includes specific guidance for non-interactive agent execution using the '--yes' flag.

**Summary:** Provides a robust protocol for verifying and installing NVIDIA GPU drivers, CUDA, and Container Toolkit across multiple Linux distributions.

**Source credibility:** Very high: Official NVIDIA engineering content from a highly-starred, actively maintained repository.

**Recency:** Current: Targets modern Linux distributions and recent CUDA/Docker configurations.

**Source:** [NVIDIA/skills/skills/tao-setup-nvidia-gpu-host/SKILL.md](https://github.com/NVIDIA/skills/blob/5b2a1e80d0e03fc3c9f60e69a727cdfcc9ab8d4c/skills/tao-setup-nvidia-gpu-host/SKILL.md) · 1269★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: tao-setup-nvidia-gpu-host
description: >-
  Host setup for TAO GPU backends. Checks and, after user approval, installs
  NVIDIA driver branch 580, CUDA Toolkit 13.0, and NVIDIA Container Toolkit
  1.19.0 for Docker/local-Docker and Kubernetes GPU worker hosts. The
  `--check-only` path works on any Linux distribution; `--install` automates
  debian-family (Ubuntu/Debian/Pop!_OS/Mint/Zorin/Raspbian), rhel-family
  (Fedora/RHEL/Rocky/AlmaLinux), and suse-family (openSUSE/SLES) hosts, and
  prints actionable manual-install steps for everything else.
license: Apache-2.0
compatibility: Runs `--check-only` on any Linux distribution. `--install` automates Ubuntu 22.04/24.04 + Debian 12 (apt), Fedora + RHEL/Rocky/AlmaLinux 9/10 (dnf), and openSUSE Leap / SLES 15 (zypper). Requires sudo/root, internet access to NVIDIA package repositories (and download.docker.com on rhel-family), and an x86_64 or aarch64 (sbsa) host. Other distributions (Arch, Alpine, Gentoo, NixOS, …) get a clear error that names the version targets and the NVIDIA install-guide URL.
metadata:
  author: NVIDIA Corporation
  version: "0.1.0"
allowed-tools: Read Bash
tags:
- setup
- nvidia
- cuda
- docker
- kubernet
```

</details>
