---
name: DataDog__serverless-sample-app__claude
source: https://github.com/DataDog/serverless-sample-app/blob/25de6432ea519856d4b8566b4bc58e79718f0998/src/order-service/CLAUDE.md
repo: DataDog/serverless-sample-app
kind: claude-md
stars: 60
last_pushed: 2026-06-16T12:30:39Z
license: apache-2.0
score: 9
domains: [.net, aws-lambda, serverless, backend-api]
tags: [tdd, dotnet, aws, architecture]
curated: 2026-06-17
curated_by: config-scout
---

# DataDog/serverless-sample-app — claude-md

**Why it's worth keeping:** Provides high-signal constraints like 'tests must follow the public API exclusively' and includes complete code examples for complex patterns like Dependency Injection and Test Data Builders.

**Summary:** Establishes a strict TDD-first workflow for .NET AWS Lambda development, emphasizing behavior-driven testing and immutable patterns.

**Source credibility:** High: authored by Datadog engineers in an active, well-maintained repository.

**Recency:** Highly current: targets .NET 9 and C# 12+ standards.

**Source:** [DataDog/serverless-sample-app/src/order-service/CLAUDE.md](https://github.com/DataDog/serverless-sample-app/blob/25de6432ea519856d4b8566b4bc58e79718f0998/src/order-service/CLAUDE.md) · 60★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Development Guidelines for .NET

The order services allows users to place orders, and traces the flow of an order through the system using a Step Function workflow. It is made up of 2 independent services

1. The `Orders.Api` provides various API endpoints to create, update and manage orders as they flow through the system
2. The `Orders.BackgroundWorkers` service is an [anti-corruption layer](https://learn.microsoft.com/en-us/azure/architecture/patterns/anti-corruption-layer) that consumes events published by external services, translates them to internal events and processes them

The .NET sample code uses the [Lambda Annotations Framework](https://github.com/aws/aws-lambda-dotnet/blob/master/Libraries/src/Amazon.Lambda.Annotations/README.md) to simplify how you define Lambda functions.

## Core Philosophy

**TEST-DRIVEN DEVELOPMENT IS NON-NEGOTIABLE.** Every single line of production code must be written in response to a failing test. No exceptions. This is not a suggestion or a preference - it is the fundamental practice that enables all other principles in this document.

I follow Test-Driven Development (TDD) with a strong emphasis on behavior-driven testing and functional
```

</details>
