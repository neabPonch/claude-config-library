---
name: asuralyc__chuanyueh-system
source: https://github.com/asuralyc/chuanyueh-system/blob/27f9a85bdc0f938583df91b27a1db4bda24af4f7/CLAUDE.md
repo: asuralyc/chuanyueh-system
kind: claude-md
stars: 6
last_pushed: 2025-11-16T14:32:40Z
license: mit
score: 8
domains: [full-stack, web-app]
tags: [nestjs, vue3, monorepo, rbac]
curated: 2026-06-16
curated_by: config-scout
---

# asuralyc/chuanyueh-system — claude-md

**Why it's worth keeping:** The 'Common Patterns' and 'Permission System' sections are highly valuable as they teach the agent how to extend the system while respecting branch-scoping and RBAC rules.

**Summary:** A comprehensive guide for a full-stack monorepo featuring NestJS and Vue 3. It covers specific development commands, architectural patterns, and business logic workflows.

**Source credibility:** Moderate; a specialized management system with a clear, structured documentation style.

**Recency:** Current; utilizes modern stacks like Vue 3 Composition API and Prisma.

**Source:** [asuralyc/chuanyueh-system/CLAUDE.md](https://github.com/asuralyc/chuanyueh-system/blob/27f9a85bdc0f938583df91b27a1db4bda24af4f7/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a **川岳員工及會員管理系統 (Chuanyueh Employee and Member Management System)** that provides branch management, employee management, member management, and role-based access control for businesses with multiple locations.

## Architecture

**Monorepo Structure:**
- `store-management-api/` - NestJS backend API with Prisma ORM
- `store-management-client/` - Vue 3 + TypeScript frontend with Element Plus
- `tech_architecture_doc.md` - Comprehensive technical architecture documentation

**Tech Stack:**
- **Backend**: NestJS + TypeScript, Prisma ORM, MySQL database, JWT authentication
- **Frontend**: Vue 3 + TypeScript, Vite build tool, Element Plus UI, Pinia state management, Vue Router
- **Database**: MySQL with Prisma schema for multi-tenant branch system

## Development Commands

### Backend (store-management-api/)
```bash
npm run start:dev          # Start development server with hot reload
npm run build              # Build for production
npm run start:prod         # Start production server
npm run lint               # Run ESLint
npm run test
```

</details>
