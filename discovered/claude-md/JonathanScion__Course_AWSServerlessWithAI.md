---
name: JonathanScion__Course_AWSServerlessWithAI
source: https://github.com/JonathanScion/Course_AWSServerlessWithAI/blob/6a133b6daab68285d0678475a8d481731ed63ccb/CLAUDE.md
repo: JonathanScion/Course_AWSServerlessWithAI
kind: claude-md
stars: 0
last_pushed: 2026-02-09T14:40:55Z
license: unknown
score: 9
domains: [aws, serverless, infrastructure-as-code, fullstack]
tags: [terraform, aws, debugging-guide, multi-project]
curated: 2026-06-17
curated_by: config-scout
---

# JonathanScion/Course_AWSServerlessWithAI — claude-md

**Why it's worth keeping:** The 'Debugging Workflow' section is elite; it tells the AI how to reason through failures by checking logs, then infra, then endpoints. The architectural pattern descriptions provide necessary mental models for data flow across services.

**Summary:** Provides a high-context map of an AWS serverless multi-repo architecture including infrastructure, deployment, and runtime patterns.

**Source credibility:** High-quality instructional content from a specialized AWS course repository.

**Recency:** Highly current, covering modern stack components like AWS Bedrock and OIDC auth.

**Source:** [JonathanScion/Course_AWSServerlessWithAI/CLAUDE.md](https://github.com/JonathanScion/Course_AWSServerlessWithAI/blob/6a133b6daab68285d0678475a8d481731ed63ccb/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Overview

This is an AWS Serverless course repository containing three independent full-stack serverless applications demonstrating different AWS architectures and patterns. Each sub-project uses Terraform for infrastructure as code and GitHub Actions for CI/CD.

## Project Structure

```
Course_AWSServerlessWithAI/
├── aws-oidc-setup/          # OIDC configuration for GitHub Actions → AWS
├── react-node-demo/         # React + Node.js Lambda + DynamoDB demo
├── test-llms-demo/          # Multi-LLM RAG chatbot with Bedrock
└── upload-file-demo/        # File upload with S3, DynamoDB, observability
```

## Sub-Projects Architecture

### 1. react-node-demo
**Stack:** React + Node.js Lambda + DynamoDB + API Gateway + CloudFront
- Frontend: React app in `client/`
- Backend: Express-like Lambda functions in `server/`
- Infrastructure: Terraform in `terraform/`
- Deployment: GitHub Actions workflow `.github/workflows/deploy-production.yml`

### 2. test-llms-demo
**Stack:** React + Python Lambda + Bedrock + OpenSearch Serverless + Knowledge Base
- Frontend: Re
```

</details>
