---
name: ivncmp__crayfish-js
source: https://github.com/ivncmp/crayfish-js/blob/7e84aeed10db21a843f62658243223d84563c3b9/CLAUDE.md
repo: ivncmp/crayfish-js
kind: claude-md
stars: 0
last_pushed: 2026-03-22T14:40:08Z
license: gpl-3.0
score: 8
domains: [backend-api, serverless, typescript]
tags: [aws-lambda, mvc-framework, cli-tooling]
curated: 2026-06-15
curated_by: config-scout
---

# ivncmp/crayfish-js — claude-md

**Why it's worth keeping:** It explicitly defines the unique decorator-based patterns (@Route, @Inject) and scaffolding commands, allowing an agent to implement features within the custom MVC structure without hallucinating standard Express or NestJS patterns.

**Summary:** A highly detailed architectural manual for a custom serverless TypeScript framework, covering CLI tooling, decorator APIs, and project structure.

**Source credibility:** Professional technical documentation from a single author; low social proof (0 stars) but high content quality.

**Recency:** Very current, targeting modern Node.js 22+ environments.

**Source:** [ivncmp/crayfish-js/CLAUDE.md](https://github.com/ivncmp/crayfish-js/blob/7e84aeed10db21a843f62658243223d84563c3b9/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - CrayfishJS Developer Guide

## 📦 Project Overview

**CrayfishJS** is a lightweight TypeScript backend framework specifically built for **AWS Lambda serverless** environments. It provides scaffolding, decorators, routing, and authentication utilities to accelerate serverless API development.

**Type:** npm package (CLI + framework library)  
**Version:** 1.3.0  
**License:** GPL-3.0-only  
**Author:** Iván Campillo (ivncmp@gmail.com)  
**Repository:** https://github.com/ivncmp/crayfish-js  

---

## 🎯 Purpose

CrayfishJS solves:
- ✅ **Serverless boilerplate** - Scaffold Lambda-ready projects in seconds
- ✅ **TypeScript-first** - Full type safety with decorators
- ✅ **AWS integration** - Cognito auth, SDK pre-configured
- ✅ **MVC pattern** - Controllers, services, models with dependency injection
- ✅ **Zero config routing** - Automatic route discovery via decorators

---

## 🏗️ Stack

- **Runtime:** Node.js 22+
- **Language:** TypeScript 5.8+
- **Framework:** Express.js (for local dev server)
- **Cloud:** AWS Lambda + API Gateway + Cognito
- **Dependencies:**
  - `@aws-sdk/client-cognito-identity-provider` - Cognito auth
  - `aws-sdk` - AWS services
  - `bcrypt` - Passw
```

</details>
