---
name: declan94__smart-inventory
source: https://github.com/declan94/smart-inventory/blob/1eacd0a679cd9fe21813628cb002d8d5350003cd/CLAUDE.md
repo: declan94/smart-inventory
kind: claude-md
stars: 0
last_pushed: 2025-11-30T08:48:29Z
license: unknown
score: 7
domains: [web-frontend, backend-api, aws-serverless]
tags: [fullstack, aws, serverless]
curated: 2026-06-16
curated_by: config-scout
---

# declan94/smart-inventory — claude-md

**Why it's worth keeping:** Includes vital local testing environment variables and detailed business logic workflows (like the OCR process) that help an agent understand state transitions.

**Summary:** Provides high-level architecture and specific operational context for a full-stack AWS application.

**Source credibility:** Low-star personal repository, but provides high signal-to-noise ratio content.

**Recency:** Current; reflects modern serverless/React development patterns.

**Source:** [declan94/smart-inventory/CLAUDE.md](https://github.com/declan94/smart-inventory/blob/1eacd0a679cd9fe21813628cb002d8d5350003cd/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Smart Inventory is an inventory management system for restaurants:
- Normal user can submit `Shortage` report when there is a stock shortage
- Admin user can view and manage all reports, the system will generate guide tables for admin to make orders of the shortage materials
- System will record all the shortage records and the order records for future iteration to a more automatic system

The system consists of a React frontend and AWS Lambda serverless backend with MySQL database.

## Architecture

### Backend (`/backend`)
- **AWS SAM serverless** application deployed to AWS Lambda
- **TypeORM** for database operations with MySQL
- **Functions**:
  - `ocr.ts` - OCR processing using Replicate API for receipt scanning
  - `material.ts` - Material CRUD operations and supplier management
  - `stockShortage.ts` - Stock shortage tracking and email alerts
- **Infrastructure**: Cognito auth, S3 for file storage, SES for emails

### Frontend (`/frontend`)
- **React 18** with TypeScript
- **Arco Design** component library
- **AWS Amplify** for Cognito au
```

</details>
