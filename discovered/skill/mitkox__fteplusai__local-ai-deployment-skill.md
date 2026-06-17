---
name: mitkox__fteplusai__local-ai-deployment-skill
source: https://github.com/mitkox/fteplusai/blob/7af47a9d8b8260234209d156c6449154bcabe3fc/skills/local-ai-deployment.skill.md
repo: mitkox/fteplusai
kind: skill
stars: 81
last_pushed: 2025-12-31T09:44:19Z
license: mit
score: 8
domains: [infrastructure, ai-inference, devops]
tags: [local-llm, vllm, docker, kubernetes, deployment]
curated: 2026-06-16
curated_by: config-scout
---

# mitkox/fteplusai — skill

**Why it's worth keeping:** Includes specific, production-ready optimization flags (tensor parallelism, prefix caching) and ready-to-use container/K8s templates that prevent manual trial-and-error.

**Summary:** A highly actionable deployment guide for self-hosting high-performance LLM inference engines like vLLM and SGLang using Docker and Kubernetes.

**Source credibility:** Decent; 81 stars indicates a specialized but validated utility for enterprise-grade vendor replacement.

**Recency:** 

**Source:** [mitkox/fteplusai/skills/local-ai-deployment.skill.md](https://github.com/mitkox/fteplusai/blob/7af47a9d8b8260234209d156c6449154bcabe3fc/skills/local-ai-deployment.skill.md) · 81★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
skill: 'local-ai-deployment'
version: '2.0.0'
updated: '2025-12-31'
category: 'local-ai-infrastructure'
complexity: 'advanced'
prerequisite_skills:
  - 'hardware-sizing'
composable_with:
  - 'mlops-operations'
  - 'data-sovereignty'
  - 'production-readiness'
  - 'open-source-licensing'
---

# Local AI Deployment Skill

## Overview
Expertise in deploying and configuring self-hosted LLM platforms for enterprise environments, ensuring data sovereignty, performance optimization, and production-grade reliability without external dependencies.

## Key Capabilities
- Self-hosted LLM platform selection and configuration
- Containerized deployment (Docker, Kubernetes, Podman)
- Model serving optimization (quantization, batching, caching)
- Air-gapped and network-isolated deployments
- High availability and load balancing
- API gateway and authentication integration

## Self-Hosted LLM Platforms

### Platform Comparison Matrix

| Platform | Type | Best For | API Compat | GPU Support | Ease of Use |
|----------|------|----------|------------|-------------|-------------|
| **vLLM** | Inference server | High throughput | OpenAI | NVIDIA, AMD | Medium |
| **SGLang** | Inference server | Pro
```

</details>
