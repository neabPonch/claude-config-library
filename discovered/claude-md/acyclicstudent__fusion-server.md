---
name: acyclicstudent__fusion-server
source: https://github.com/acyclicstudent/fusion-server/blob/18bd65d910107795133457af082da62e12972eab/CLAUDE.md
repo: acyclicstudent/fusion-server
kind: claude-md
stars: 0
last_pushed: 2026-04-15T20:19:08Z
license: mit
score: 9
domains: [backend, serverless, aws-lambda, typescript]
tags: [clean-architecture, pattern-matching, dependency-injection]
curated: 2026-06-16
curated_by: config-scout
---

# acyclicstudent/fusion-server — claude-md

**Why it's worth keeping:** Uses highly specific 'Example Pattern' blocks to teach unique rules (like UCExecutor vs @Injectable) and complex event-matching logic that an AI would otherwise hallucinate.

**Summary:** Provides exhaustive architectural constraints and implementation patterns for a serverless AWS Lambda framework.

**Source credibility:** The repository has low social proof, but the technical depth of the documentation suggests high authorship quality.

**Recency:** Very current, including modern AWS service patterns like Bedrock Agent Actions.

**Source:** [acyclicstudent/fusion-server/CLAUDE.md](https://github.com/acyclicstudent/fusion-server/blob/18bd65d910107795133457af082da62e12972eab/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is the **@fusion-framework/server** - a TypeScript library for building AWS Lambda serverless applications with a clean architecture approach. The framework is built on top of TSDX and uses dependency injection via TSyringe.

## Commands

### Development
- `npm start` or `yarn start` - Build to `/dist` and run in watch mode
- `npm run build` or `yarn build` - One-off build
- `npm test` or `yarn test` - Run Jest tests
- `npm run lint` or `yarn lint` - Lint code with TSDX linter

### Analysis
- `npm run size` - Calculate bundle size with size-limit
- `npm run analyze` - Visualize bundle with size-limit

## Architecture

### Clean Architecture with Fusion Framework

The framework implements Clean Architecture patterns with specific conventions:

**Use Cases:**
- All use cases must be decorated with `@UseCase()` (not `@Injectable()`)
- Use cases must extend the `UC` abstract class
- Use cases are called via `UCExecutor` instead of direct constructor injection
- Example pattern:
  ```ts
  @UseCase()
  class MyUseCase extends UC {
    execute(para
```

</details>
