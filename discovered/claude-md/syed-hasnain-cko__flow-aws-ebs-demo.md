---
name: syed-hasnain-cko__flow-aws-ebs-demo
source: https://github.com/syed-hasnain-cko/flow-aws-ebs-demo/blob/312b1020ab238ca0b815c7da5ab2865296e6c9c0/CLAUDE.md
repo: syed-hasnain-cko/flow-aws-ebs-demo
kind: claude-md
stars: 0
last_pushed: 2026-06-12T11:28:35Z
license: unknown
score: 9
domains: [backend-api, payment-integration, aws-serverless, ai-agents]
tags: [architectural-patterns, slash-commands, operational-manual]
curated: 2026-06-15
curated_by: config-scout
---

# syed-hasnain-cko/flow-aws-ebs-demo — claude-md

**Why it's worth keeping:** It provides a high-density API endpoint registry and introduces a system of slash-commandable skills that turn the agent into a specialized developer for this specific domain.

**Summary:** An advanced operational manual that documents not just the codebase, but also custom AI 'skills' and coding patterns specific to the project.

**Source credibility:** A personal demo repository, but the technical documentation quality is highly professional.

**Recency:** Extremely recent/current; demonstrates advanced usage of Claude Code's capabilities.

**Source:** [syed-hasnain-cko/flow-aws-ebs-demo/CLAUDE.md](https://github.com/syed-hasnain-cko/flow-aws-ebs-demo/blob/312b1020ab238ca0b815c7da5ab2865296e6c9c0/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

A Checkout.com payment integration testing suite app showcasing Flow (prebuilt UI) card payments, Google Pay, Apple Pay, and all payment methods like PayPal, Klarna tested via payment setup API and management operations (capture, void, refund) with a webhook endpoint polling for 2 mins until received. Deployed on AWS Amplify and API Gateway with a parallel Lambda/Amplify manual deployment path.

## Commands

```bash
npm start         # Local env runs on http://localhost:4244
```

App runs at `http://localhost:4244`.

No lint or test commands are configured.

## Architecture

### Deployment Modes

Frontend folder is deployed on AWS amplify and backend is deployed manually by making changes via AWS console to my lambda function directly and adding gateway API endpoints on AWS API Gateway:

| Mode | Entry Point | API Routes | Use |
|------|------------|------------|-----|
| AWS Lambda (Amplify) | `frontend/tabs/loader.js` | `amplify/backend/function/src/index.js` → `amplify/backend/function/function/src/api-route-controller.js` | Serverless deployment |

##
```

</details>
