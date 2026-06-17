---
name: aegntic__aegntic-MCP
source: https://github.com/aegntic/aegntic-MCP/blob/00e395862cc6c965a3a342b2e74ca3b44c5f0567/CLAUDE.md
repo: aegntic/aegntic-MCP
kind: claude-md
stars: 8
last_pushed: 2025-10-27T02:15:10Z
license: other
score: 9
domains: [agents-ai, rag-systems, data-engineering]
tags: [obsidian, graph-database, vector-db, python, nodejs]
curated: 2026-06-16
curated_by: config-scout
---

# aegntic/aegntic-MCP — claude-md

**Why it's worth keeping:** The highly structured command sections (categorized by functional domain) and the detailed 'Retrieval Layers' explain the underlying logic, allowing Claude to understand intent rather than just syntax. Including specific performance metrics provides a benchmark for agentic troubleshooting.

**Summary:** This file provides comprehensive operational guidance for a complex RAG system involving multiple databases and specialized scripts. It acts as both a developer's manual and an agent-specific execution guide.

**Source credibility:** Moderate; 8 stars suggests niche utility, though maintenance has slowed in recent months.

**Recency:** Highly relevant as it explicitly targets Claude Code and handles complex local environments typical of modern AI workflows.

**Source:** [aegntic/aegntic-MCP/CLAUDE.md](https://github.com/aegntic/aegntic-MCP/blob/00e395862cc6c965a3a342b2e74ca3b44c5f0567/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## System Overview

This is an elite Obsidian RAG (Retrieval-Augmented Generation) system that transforms Obsidian vaults into AI-paired cognitive workflow engines. The system implements multi-layered knowledge architecture with hierarchical context management and automated knowledge graph construction.

## Commands

### Development and Setup
```bash
# Initialize new vault with elite structure
npm run setup /path/to/your/vault

# Start development environment (RAG engine + web interface)
npm run dev

# Start only the RAG engine
npm run dev:rag

# Start only the web interface
npm run dev:web

# Build for production
npm run build

# Run tests
npm run test

# Lint code
npm run lint
```

### Database Management
```bash
# Start both databases (Qdrant + Neo4j)
npm run start:databases

# Start Neo4j knowledge graph database
npm run start:neo4j

# Stop Neo4j database
npm run stop:neo4j

# Reset Neo4j database (clear all data)
npm run reset:neo4j

# Stop all databases
npm run stop:databases

# Setup Graphiti dependencies
npm run setup:graphiti
```

### RAG Engine Operations
`
```

</details>
