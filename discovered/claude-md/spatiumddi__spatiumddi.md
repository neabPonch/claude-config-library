---
name: spatiumddi__spatiumddi
source: https://github.com/spatiumddi/spatiumddi/blob/e1509d05d4276b3234a271047319f0ef27f02edb/CLAUDE.md
repo: spatiumddi/spatiumddi
kind: claude-md
stars: 25
last_pushed: 2026-06-15T10:20:02Z
license: other
score: 9
domains: [backend-api, devops, infrastructure]
tags: [project-mapping, architecture-index]
curated: 2026-06-15
curated_by: config-scout
---

# spatiumddi/spatiumddi — claude-md

**Why it's worth keeping:** The 'Document Map' is an exceptional technique that prevents AI hallucination by directing it to authoritative sources for every subsystem. The tech stack and repo layout provide immediate, high-density environmental awareness.

**Summary:** Acts as a highly structured project index that maps complex domain logic to specific technical documentation and architectural specs.

**Source credibility:** High; an active, specialized infrastructure project with clear domain expertise.

**Recency:** Current; reflects modern practices for providing highly structured context to LLMs.

**Source:** [spatiumddi/spatiumddi/CLAUDE.md](https://github.com/spatiumddi/spatiumddi/blob/e1509d05d4276b3234a271047319f0ef27f02edb/CLAUDE.md) · 25★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

> **GitHub Org:** https://github.com/spatiumddi  
> **Docs:** https://spatiumddi.github.io/spatiumddi/  
> **License:** Apache 2.0  
> **Package:** `spatiumddi` on PyPI  
> **Container registry:** `ghcr.io/spatiumddi/*`  

> **Read this file first.** This is the entry point for all Claude Code sessions on the SpatiumDDI project. It defines the project scope, the document map, and the non-negotiable conventions every generated file must follow.

---

## What Is SpatiumDDI?

SpatiumDDI is a production-grade, open-source **all-in-one DDI (DNS, DHCP, IPAM)** platform. It does not merely configure external DDI servers — it manages and runs the DHCP and DNS service containers directly. The control plane (FastAPI + PostgreSQL) is the source of truth; all managed service containers (Kea, BIND9) are deployed and configured by SpatiumDDI.

It can be deployed as individual containers, a full Docker Compose stack, a Kubernetes application, or as a **self-contained OS appliance image**. Supported on `linux/amd64` and `linux/arm64` (all Docker images must be built multi-arch).

It
```

</details>
