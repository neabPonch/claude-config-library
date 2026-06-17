---
name: dwexjs__dwex__claude-ejs
source: https://github.com/dwexjs/dwex/blob/29eacd4c61126d2f234ef367d394a884111c2832/packages/create-dwex/templates/base/CLAUDE.md.ejs
repo: dwexjs/dwex
kind: claude-md
stars: 8
last_pushed: 2025-11-26T10:32:25Z
license: mit
score: 9
domains: [backend-api, typescript]
tags: [framework, mcp, bun, dependency-injection]
curated: 2026-06-16
curated_by: config-scout
---

# dwexjs/dwex — claude-md

**Why it's worth keeping:** The unique inclusion of an MCP (Model Context Protocol) section allows Claude to introspect its own environment, routes, and dependencies in real-time via specialized tools.

**Summary:** Defines framework architecture, coding patterns, and Bun-specific optimizations for the Dwex TypeScript framework.

**Source credibility:** Low star count indicates a niche project, but the documentation quality is professional and highly structured.

**Recency:** Very current; actively utilizes the latest Model Context Protocol (MCP) standards for AI interaction.

**Source:** [dwexjs/dwex/packages/create-dwex/templates/base/CLAUDE.md.ejs](https://github.com/dwexjs/dwex/blob/29eacd4c61126d2f234ef367d394a884111c2832/packages/create-dwex/templates/base/CLAUDE.md.ejs) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# <%= projectName %> - Dwex Framework

## Project Overview

This is a Dwex application - a modern, TypeScript-first framework for building web applications with Bun runtime. Dwex provides a decorator-based architecture inspired by frameworks like NestJS but optimized for Bun's performance.

## Framework Architecture

**Decorator-Based**: Dwex uses TypeScript decorators extensively for metadata and dependency injection:
- `@Module()` - Defines application modules with providers, controllers, and imports
- `@Controller()` - Marks classes as HTTP controllers
- `@Injectable()` - Marks classes as injectable services (singleton by default)
- `@Get()`, `@Post()`, `@Put()`, `@Delete()`, `@Patch()` - HTTP method decorators
- `@Param()`, `@Query()`, `@Body()`, `@Headers()` - Request data extractors
- `@UseGuards()` - Apply guards for authorization/authentication
- `@UseInterceptors()` - Apply interceptors for request/response transformation

**Dependency Injection**: Dwex has a built-in DI container with:
- Constructor injection (recommended)
- Three scopes: `SINGLETON` (default), `REQUEST`, `TRANSIENT`
- Automatic resolution of dependencies via reflect-metadata

**Module System**: Organize
```

</details>
