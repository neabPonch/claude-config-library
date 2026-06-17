---
name: greedychipmunk__agent-skills__skill
source: https://github.com/greedychipmunk/agent-skills/blob/78a35a661f69af8e86cb8d26851be7b9697d89e5/nextjs-developer/skill.md
repo: greedychipmunk/agent-skills
kind: skill
stars: 8
last_pushed: 2026-05-26T02:23:43Z
license: mit
score: 9
domains: [web-frontend, nextjs, react]
tags: [nextjs, app-router, react-19, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# greedychipmunk/agent-skills — skill

**Why it's worth keeping:** It provides specific implementation patterns for high-level nuances like Partial Prerendering (PPR), the new 'after()' function, and updated fetch caching behaviors that prevent AI hallucination of deprecated v13/14 patterns.

**Summary:** A dense technical reference for building production-ready Next.js 15+ applications using the App Router and React 19.

**Source credibility:** The depth of detail regarding recent Next.js 15 changes suggests a highly competent author.

**Recency:** Extremely current; specifically targets Next.js 15 and React 19 features.

**Source:** [greedychipmunk/agent-skills/nextjs-developer/skill.md](https://github.com/greedychipmunk/agent-skills/blob/78a35a661f69af8e86cb8d26851be7b9697d89e5/nextjs-developer/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: nextjs-developer
description: Expert Next.js development with App Router, Server Components, and modern React patterns
---

# Next.js Developer Skill

## Overview

This skill provides comprehensive expertise in building production-ready Next.js applications using the **App Router** (Next.js 15+). It covers Server Components, React 19 support, data fetching patterns, routing, API routes, caching, and performance optimization.

## Core Capabilities

### App Router Architecture
- **Server Components**: Default rendering model for optimal performance
- **Client Components**: Interactive components with `"use client"` directive
- **Layouts**: Shared UI with preserved state across routes
- **Templates**: Fresh instances on navigation (no state preservation)
- **Loading UI**: Streaming with `loading.tsx` files
- **Error Handling**: Granular error boundaries with `error.tsx`

### Data Fetching
- **Server-side fetching**: Direct database/API access in Server Components
- **Caching strategies**: Dynamic rendering by default, explicit caching, and incremental regeneration
- **Revalidation**: Time-based and on-demand cache invalidation
- **Parallel fetching**: Optimized data loading
```

</details>
