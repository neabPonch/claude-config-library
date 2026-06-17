---
name: txn2__kubefwd
source: https://github.com/txn2/kubefwd/blob/a9fcc746f4ea5ecfbe726d71a6cd490c7f34e788/CLAUDE.md
repo: txn2/kubefwd
kind: claude-md
stars: 4120
last_pushed: 2026-06-09T22:50:36Z
license: apache-2.0
score: 9
domains: [cli-tools, kubernetes, go, networking]
tags: [architecture-mapping, system-design, dev-ops]
curated: 2026-06-15
curated_by: config-scout
---

# txn2/kubefwd — claude-md

**Why it's worth keeping:** The architectural breakdown explains not just what packages exist, but how they interact and why specific patterns like debouncing or shutdown orchestration are used. Including 'Key Differentiators' prevents the AI from suggesting generic alternatives that violate the tool's core purpose.

**Summary:** Provides an exceptionally deep mental model of the project, covering unique value propositions, detailed TUI architecture (MVU), and a full component flow.

**Source credibility:** Highly credible; a high-star (4k+), well-maintained Kubernetes utility.

**Recency:** Current; utilizes modern patterns and provides context optimized for LLM reasoning.

**Source:** [txn2/kubefwd/CLAUDE.md](https://github.com/txn2/kubefwd/blob/a9fcc746f4ea5ecfbe726d71a6cd490c7f34e788/CLAUDE.md) · 4120★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

kubefwd is a popular command-line utility for bulk Kubernetes port forwarding, featured in "essential k8s developer tools" lists. It forwards multiple services from one or more namespaces, adding corresponding entries to `/etc/hosts` for local development.

**Key Differentiator from `kubectl port-forward`**: Each service gets its own unique loopback IP address (127.x.x.x), allowing multiple services to use the same port simultaneously (e.g., multiple databases on port 3306, or multiple web services on port 80). This mirrors how services work in the cluster, enabling truly cluster-like local development.

The tool automatically monitors service and pod lifecycle events, starting/stopping port forwards as services are created, deleted, or pods are rescheduled.

## Integration and Usage Patterns

kubefwd is commonly integrated into development workflows:

- **With Tilt**: Blog posts document using kubefwd with Tilt for automated local development setups
- **Development Environment Setup**: Teams use kubefwd to mirror production-like service topologi
```

</details>
