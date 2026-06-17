---
name: jhs__Chatfield__claude
source: https://github.com/jhs/Chatfield/blob/0e67171a5e133f21557f602d684f411dbedaec37/TypeScript/react/CLAUDE.md
repo: jhs/Chatfield
kind: claude-md
stars: 6
last_pushed: 2025-11-24T02:55:40Z
license: apache-2.0
score: 8
domains: [web-frontend, typescript, react]
tags: [api-reference, implementation-details, dev-workflow]
curated: 2026-06-14
curated_by: config-scout
---

# jhs/Chatfield — claude-md

**Why it's worth keeping:** It documents critical 'gotchas' like TypeScript configuration requirements and explains internal callback memoization logic to prevent the AI from introducing bugs.

**Summary:** Provides deep technical context for a React library integration, covering API surface, internal state logic, and build-system nuances.

**Source credibility:** Small open-source project with highly structured, professional-grade technical documentation.

**Recency:** Very recent (7 months ago) and follows modern development standards.

**Source:** [jhs/Chatfield/TypeScript/react/CLAUDE.md](https://github.com/jhs/Chatfield/blob/0e67171a5e133f21557f602d684f411dbedaec37/TypeScript/react/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# TypeScript React Integration - CLAUDE.md

This file provides guidance for working with the Chatfield React integration.

## Overview

`@chatfield/react` provides React hooks and utilities for integrating Chatfield conversational data collection into React applications. The package is designed to be headless (no UI components), focusing on business logic and state management.

**Package Name**: `@chatfield/react`
**Version**: 0.1.0
**Location**: `TypeScript/react/`

## Quick Start

```bash
cd TypeScript/react
npm install
npm run build
```

## Core API

### useChatfield Hook

The primary API for React integration. Provides state management and conversation orchestration for Chatfield interviews.

```typescript
import { useChatfield } from '@chatfield/react'
import { chatfield } from '@chatfield/core/lean'

const interview = chatfield()
  .field('name')
    .desc('Your name')
  .build()

function MyComponent() {
  const [state, actions] = useChatfield(interview, {
    onField: (fieldName, fieldProxy) => {
      console.log(`Collected: ${fieldName}`, fieldProxy)
    },
    onError: (error) => {
      console.error('Error:', error)
    }
  })

  if (state.interview._done) {
    return
```

</details>
