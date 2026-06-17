---
name: abelrguezr__hacktricks-skills__skill-md
source: https://github.com/abelrguezr/hacktricks-skills/blob/b856f838a36c16deb457413ea9d3ab7afbd486f6/skills/linux-hardening/privilege-escalation/selinux/SKILL.MD
repo: abelrguezr/hacktricks-skills
kind: skill
stars: 15
last_pushed: 2026-03-23T14:34:10Z
license: unknown
score: 7
domains: [security, devops, cli-tools]
tags: [selinux, containers, podman, security]
curated: 2026-06-16
curated_by: config-scout
---

# abelrguezr/hacktricks-skills — skill

**Why it's worth keeping:** The specific mapping of 'container_t' to 'container_file_t' and the inclusion of practical command examples enable actionable troubleshooting steps for a coding agent.

**Summary:** Explains SELinux labeling mechanics for containers and provides essential CLI commands for security auditing.

**Source credibility:** Sourced from a collection derived from Hacktricks, a highly respected cybersecurity resource.

**Recency:** Current; aligns with modern container security and podman/docker workflows.

**Source:** [abelrguezr/hacktricks-skills/skills/linux-hardening/privilege-escalation/selinux/SKILL.MD](https://github.com/abelrguezr/hacktricks-skills/blob/b856f838a36c16deb457413ea9d3ab7afbd486f6/skills/linux-hardening/privilege-escalation/selinux/SKILL.MD) · 15★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: selinux-container-security
description: How to understand and configure SELinux for container security. Use this skill whenever the user mentions SELinux, container security, container escape prevention, podman, docker security, or needs to harden container environments with mandatory access controls.
---

# SELinux Container Security

A skill for understanding and configuring SELinux to secure container environments.

## What SELinux Does for Containers

SELinux is a **labeling system** that provides mandatory access control. Every process and file system object has a label. SELinux policies define rules about what a process label is allowed to do with all other labels on the system.

### Container Labeling

Container engines launch container processes with a single confined SELinux label, usually `container_t`, and set the container filesystem to be labeled `container_file_t`. The SELinux policy rules say that `container_t` processes can only read/write/execute files labeled `container_file_t`.

**Why this matters:** If a container process escapes the container and attempts to write to content on the host, the Linux kernel denies access and only allows the container pro
```

</details>
