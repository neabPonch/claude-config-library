---
name: digitalis-io__k3s-on-prem-production
source: https://github.com/digitalis-io/k3s-on-prem-production/blob/a3fc3132bbd7eb9447c8194b3fab7bb95033cf25/CLAUDE.md
repo: digitalis-io/k3s-on-prem-production
kind: claude-md
stars: 161
last_pushed: 2026-04-29T09:45:17Z
license: apache-2.0
score: 9
domains: [devops, infrastructure, security]
tags: [ansible, k8s, hardening, guardrails]
curated: 2026-06-15
curated_by: config-scout
---

# digitalis-io/k3s-on-prem-production — claude-md

**Why it's worth keeping:** The 'What NOT to Change' section is a masterclass in providing negative constraints to prevent AI from breaking intentional workarounds. The phased task list provides excellent context for the current state of technical debt and migrations.

**Summary:** A highly structured project tracking file for an Ansible/K3s infrastructure modernization effort.

**Source credibility:** Strong; based on an active, starred repository focused on production-grade K3s/security.

**Recency:** Very recent; utilizes up-to-date versioning (K3s v1.32) and modern DevOps practices.

**Source:** [digitalis-io/k3s-on-prem-production/CLAUDE.md](https://github.com/digitalis-io/k3s-on-prem-production/blob/a3fc3132bbd7eb9447c8194b3fab7bb95033cf25/CLAUDE.md) · 161★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# K3s Ansible Playbook Modernization — Project Tracking

## Overview

Ansible playbook that provisions a hardened k3s Kubernetes cluster (3-master HA + 3 workers)
with CIS/STIG compliance, Falco runtime security, MetalLB load balancing, NGINX ingress,
Kubernetes dashboard, and Keepalived VIP.

---

## Task Status

### Phase 0: Tooling and Baseline

- [x] **Task 0.1** — Add `.ansible-lint`, `.yamllint.yml`, and `requirements.yml`
- [x] **Task 0.2** — Create GitHub Actions CI skeleton (lint + syntax-check jobs)

### Phase 1: Ansible Compatibility Fixes

- [x] **Task 1.1** — Remove `warn: no` from `roles/hardening/tasks/auditd.yml`
- [x] **Task 1.2** — Convert `yes`/`no` booleans to `true`/`false` across all YAML files
- [x] **Task 1.3** — Fix double-template `when` conditions
- [x] **Task 1.4** — Convert safe `include_tasks` to `import_tasks` where no runtime variables needed

### Phase 2: Secrets Management

- [x] **Task 2.1** — Migrate plaintext secrets to Ansible Vault
- [x] **Task 2.2** — Rotate all secrets (new values for cluster token, encryption key, Slack webhook)

### Phase 3: PSP Removal → Pod Security Admission

- [x] **Task 3.1** — Create PSA admission configuration and u
```

</details>
