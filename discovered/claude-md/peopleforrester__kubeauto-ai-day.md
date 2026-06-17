---
name: peopleforrester__kubeauto-ai-day
source: https://github.com/peopleforrester/kubeauto-ai-day/blob/b7bc20eb6c2174f0c0396088146ca68f3a155c75/CLAUDE.md
repo: peopleforrester/kubeauto-ai-day
kind: claude-md
stars: 12
last_pushed: 2026-05-28T09:13:39Z
license: apache-2.0
score: 9
domains: [infrastructure-as-code, devops, kubernetes]
tags: [gitops, tdd, kubernetes]
curated: 2026-06-15
curated_by: config-scout
---

# peopleforrester/kubeauto-ai-day — claude-md

**Why it's worth keeping:** Employs advanced agentic patterns like structured completion tags (<promise>) and modular skill directories. It mandates high-fidelity testing against real infrastructure rather than mocks to prevent hallucination in infra work.

**Summary:** A rigorous, test-driven protocol for building production Kubernetes infrastructure via GitOps and ArgoCD.

**Source credibility:** High; part of an active, specific production-grade IDP project.

**Recency:** Current; uses modern DevOps toolsets and sophisticated state-tracking protocols.

**Source:** [peopleforrester/kubeauto-ai-day/CLAUDE.md](https://github.com/peopleforrester/kubeauto-ai-day/blob/b7bc20eb6c2174f0c0396088146ca68f3a155c75/CLAUDE.md) · 12★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# KubeAuto Day IDP Build

Building a production-grade Internal Developer Platform on EKS from scratch. Every component deployed via ArgoCD GitOps after Phase 2.

This repo serves three purposes:
1. Live demo platform for KubeAuto Day Europe 2026 talk
2. Open-source reference IDP (Apache 2.0)
3. Evidence for the AI Platform Building Scorecard

**Stack**: EKS 1.34+, ArgoCD 3.2+, Kyverno 1.17+, Backstage 1.46+, Falco, OTel Collector 0.140+, Grafana 12.x, cert-manager 1.19+, Terraform EKS module ~>21.0, Python (uv, pytest)

## How To Work

1. Read `spec/BUILD-SPEC.md` for the full build plan
2. Check current phase via `spec/SCORECARD.md`
3. Write tests first (`tests/test_phase_0X_*.py`), then implement until they pass
4. Update scorecard after each component with honest scores
5. Commit after each working component, not after each file

## Commands

```bash
uv run pytest tests/ -v    # Full test suite

# Pre-push verification
git branch --show-current  # Must show "staging"
git pull origin staging
uv run pytest tests/ -v
git push origin staging
```

## Project-Specific Rules

- **Everything after Phase 2 must be an ArgoCD Application**
- **No secrets in Git** — use External Secrets Ope
```

</details>
