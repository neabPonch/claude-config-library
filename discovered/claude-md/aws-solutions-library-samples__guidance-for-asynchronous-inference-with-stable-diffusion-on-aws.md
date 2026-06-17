---
name: aws-solutions-library-samples__guidance-for-asynchronous-inference-with-stable-diffusion-on-aws
source: https://github.com/aws-solutions-library-samples/guidance-for-asynchronous-inference-with-stable-diffusion-on-aws/blob/299c28b5940c5e0933a9e6b27a5c1f3d872c1f96/CLAUDE.md
repo: aws-solutions-library-samples/guidance-for-asynchronous-inference-with-stable-diffusion-on-aws
kind: claude-md
stars: 37
last_pushed: 2026-05-23T13:39:10Z
license: mit-0
score: 9
domains: [infrastructure-as-code, devops, cloud-computing, machine-learning]
tags: [aws-cdk, eks, kubernetes, stable-diffusion]
curated: 2026-06-15
curated_by: config-scout
---

# aws-solutions-library-samples/guidance-for-asynchronous-inference-with-stable-diffusion-on-aws — claude-md

**Why it's worth keeping:** The directory structure map includes semantic descriptions of every module, and the 'Key Patterns' section explains internal architectural interfaces to ensure AI-generated code follows existing design patterns.

**Summary:** A highly detailed guide for complex AWS EKS infrastructure and machine learning deployment patterns. It provides essential context on how configuration flows through multiple layers of abstraction.

**Source credibility:** High; an official AWS Solutions Library sample with recent maintenance activity.

**Recency:** Very current, using modern versions of Kubernetes (v1.35) and Karpenter (v1.9).

**Source:** [aws-solutions-library-samples/guidance-for-asynchronous-inference-with-stable-diffusion-on-aws/CLAUDE.md](https://github.com/aws-solutions-library-samples/guidance-for-asynchronous-inference-with-stable-diffusion-on-aws/blob/299c28b5940c5e0933a9e6b27a5c1f3d872c1f96/CLAUDE.md) · 37★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Project Guide for AI Assistants

## Project Overview

Guidance for Asynchronous Image Generation with Stable Diffusion on AWS. A fast-scaling, low-cost Stable Diffusion inference solution using serverless and container services on AWS. Deploys an EKS cluster with GPU auto-scaling (Karpenter) and event-driven pod scaling (KEDA) for asynchronous image generation.

## Tech Stack

- AWS CDK (TypeScript) with EKS Blueprints v1.18.0
- EKS Kubernetes v1.35
- Karpenter v1.9.0 (stable CRDs: NodePool, EC2NodeClass)
- KEDA for queue-based pod autoscaling
- Bottlerocket OS on GPU nodes
- SOCI Parallel Pull for fast container image loading
- NVMe instance store for kubelet/containerd storage

## Directory Structure

```
bin/                         # CDK app entry point
  stable-difussion-on-eks.ts # Main app, loads config.yaml and creates DataPlaneStack
lib/                         # CDK infrastructure code
  dataPlane.ts               # Main stack - EKS Blueprint builder with all add-ons
  addons/
    dcgmExporter.ts          # NVIDIA GPU metrics (Helm addon)
    ebsThroughputTuner.ts    # EBS throughput tuning via Lambda + Step Functions
    s3CSIDriver.ts           # S3 Mountp
```

</details>
