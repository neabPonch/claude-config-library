---
name: Claude-Code-Community-Ireland__claude-code-resources__skill
source: https://github.com/Claude-Code-Community-Ireland/claude-code-resources/blob/b9f5c0fea31eb7ee5f20960fd976a7c31ee7a0df/skills/general/aws-serverless/skill.md
repo: Claude-Code-Community-Ireland/claude-code-resources
kind: skill
stars: 8
last_pushed: 2026-06-01T15:01:23Z
license: mit
score: 8
domains: [backend, cloud-infrastructure, aws]
tags: [serverless, lambda, sqs, api-gateway, sam]
curated: 2026-06-16
curated_by: config-scout
---

# Claude-Code-Community-Ireland/claude-code-resources — skill

**Why it's worth keeping:** Includes high-level production techniques like out-of-handler SDK initialization, partial batch failure handling in SQS, and cold start mitigations.

**Summary:** A professional implementation guide for AWS Serverless architecture covering Lambda, API Gateway, and SQS patterns using SAM.

**Source credibility:** Curated by a community repository with active maintenance and recent commits.

**Recency:** Highly current; utilizes modern Node.js 20.x runtimes and contemporary AWS patterns.

**Source:** [Claude-Code-Community-Ireland/claude-code-resources/skills/general/aws-serverless/skill.md](https://github.com/Claude-Code-Community-Ireland/claude-code-resources/blob/b9f5c0fea31eb7ee5f20960fd976a7c31ee7a0df/skills/general/aws-serverless/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: aws-serverless
description: "Specialized skill for building production-ready serverless applications on AWS. Covers Lambda functions, API Gateway, DynamoDB, SQS/SNS event-driven patterns, SAM/CDK deployment, and cold start optimization."
source: vibeship-spawner-skills (Apache 2.0)
---

# AWS Serverless

## Patterns

### Lambda Handler Pattern

Proper Lambda function structure with error handling

**When to use**: ['Any Lambda function implementation', 'API handlers, event processors, scheduled tasks']

```python
```javascript
// Node.js Lambda Handler
// handler.js

// Initialize outside handler (reused across invocations)
const { DynamoDBClient } = require('@aws-sdk/client-dynamodb');
const { DynamoDBDocumentClient, GetCommand } = require('@aws-sdk/lib-dynamodb');

const client = new DynamoDBClient({});
const docClient = DynamoDBDocumentClient.from(client);

// Handler function
exports.handler = async (event, context) => {
  // Optional: Don't wait for event loop to clear (Node.js)
  context.callbackWaitsForEmptyEventLoop = false;

  try {
    // Parse input based on event source
    const body = typeof event.body === 'string'
      ? JSON.parse(event.body)
      : even
```

</details>
