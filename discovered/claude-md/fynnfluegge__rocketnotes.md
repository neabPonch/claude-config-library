---
name: fynnfluegge__rocketnotes
source: https://github.com/fynnfluegge/rocketnotes/blob/e1638f4877e7bb53727c7e2c6f86e5a267210cec/CLAUDE.md
repo: fynnfluegge/rocketnotes
kind: claude-md
stars: 1335
last_pushed: 2026-04-23T07:57:04Z
license: apache-2.0
score: 9
domains: [ai-agents, fullstack, cloud-infrastructure, backend-api]
tags: [rag, aws-sam, polyglot, angular, python]
curated: 2026-06-15
curated_by: config-scout
---

# fynnfluegge/rocketnotes — claude-md

**Why it's worth keeping:** The detailed breakdown of the dual-mode vector storage (ChromaDB vs S3) and explicit toolchain instructions (using uv) prevents common LLM errors in environment configuration.

**Summary:** Provides deep architectural context for a polyglot fullstack application using Angular, Go, and Python. It excels at explaining the environmental switching logic between local development and AWS production.

**Source credibility:** Highly credible; high star count (1.3k+) and recent activity suggest a production-ready, well-maintained project.

**Recency:** Very current; uses modern tools like Angular 18 and the 'uv' Python package manager.

**Source:** [fynnfluegge/rocketnotes/CLAUDE.md](https://github.com/fynnfluegge/rocketnotes/blob/e1638f4877e7bb53727c7e2c6f86e5a267210cec/CLAUDE.md) · 1335★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Rocketnotes is an AI-powered markdown note-taking application with semantic search, chat capabilities, and document archiving. It features a serverless RAG pipeline built with langchain, langgraph, and S3-based vector storage, supporting both cloud and local deployment.

## Architecture

The project follows a microservices architecture with three main components:

- **Frontend (webapp/)**: Angular 18 + TypeScript application with Electron support
- **Go Handlers (handler-crud/)**: Lambda functions for document CRUD operations, user management, and search
- **Python Handlers (handler-ai/)**: AI-powered features including semantic search, chat, vector embeddings, and agentic archiving
- **Infrastructure**: AWS SAM template with DynamoDB, S3, and Lambda functions

### Key Directories

- `webapp/src/app/component/`: Angular components (editor, navigation, zettelkasten, dialogs)
- `webapp/src/app/service/`: Angular services for API communication
- `handler-crud/`: Individual Go Lambda handlers for basic CRUD operations
- `handler-ai/rocketnotes_handle
```

</details>
