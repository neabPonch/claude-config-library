---
name: cryfs__cryfs-web-next__claude
source: https://github.com/cryfs/cryfs-web-next/blob/fd4b5ce3625a418ea30f3ea0b3e936557476f4ba/backend/CLAUDE.md
repo: cryfs/cryfs-web-next
kind: claude-md
stars: 0
last_pushed: 2026-04-13T22:48:37Z
license: unknown
score: 8
domains: [backend-api, serverless]
tags: [aws-lambda, typescript, sam, patterns]
curated: 2026-06-16
curated_by: config-scout
---

# cryfs/cryfs-web-next — claude-md

**Why it's worth keeping:** The 'Code Conventions' section is excellent; it defines higher-order functions, naming standards, and specific caching patterns that ensure AI-generated code adheres to the project's unique architecture.

**Summary:** A detailed guide for an AWS Lambda backend that includes tech stack details, command references, and specific architectural patterns.

**Source credibility:** Low star count on repo, but the documentation style suggests a professional developer structure.

**Recency:** Very recent; pushed 2 months ago.

**Source:** [cryfs/cryfs-web-next/backend/CLAUDE.md](https://github.com/cryfs/cryfs-web-next/blob/fd4b5ce3625a418ea30f3ea0b3e936557476f4ba/backend/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Backend

AWS Lambda serverless functions for the CryFS website, deployed with AWS SAM.

## Tech Stack

- **Runtime**: AWS Lambda with AWS SAM (Serverless Application Model)
- **Language**: TypeScript
- **Bundler**: esbuild (built into SAM, handles TypeScript natively)
- **Testing**: Jest with ts-jest
- **External Services**: AWS SES (email), Mailchimp (newsletter)
- **Secrets**: AWS SSM Parameter Store

## Prerequisites

Install the AWS SAM CLI:
- macOS: `brew install aws-sam-cli`
- Other: https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/install-sam-cli.html

## API Endpoints

| Method | Path | Description |
|--------|------|-------------|
| POST | `/newsletter/register` | Subscribe email to Mailchimp newsletter |
| POST | `/contact/send` | Send contact form message via AWS SES |

Both endpoints use simple token-based spam protection (not authentication).

## Directory Structure

```
backend/
├── *.ts              # Source modules (handlers and utilities)
├── *.test.ts         # Jest tests (colocated)
├── __mocks__/        # Jest mocks for external services
├── types/            # Type declarations for untyped packages
├── iam/              # IAM pol
```

</details>
