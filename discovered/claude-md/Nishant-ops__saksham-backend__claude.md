---
name: Nishant-ops__saksham-backend__claude
source: https://github.com/Nishant-ops/saksham-backend/blob/7eae3c6e94950173bd529ac584f1ac3f0d69dba5/lambda_functions/CLAUDE.md
repo: Nishant-ops/saksham-backend
kind: claude-md
stars: 0
last_pushed: 2025-12-26T16:20:18Z
license: unknown
score: 9
domains: [backend-api, cloud-infrastructure, ai-processing]
tags: [aws-lambda, state-machine, microservices, python]
curated: 2026-06-15
curated_by: config-scout
---

# Nishant-ops/saksham-backend — claude-md

**Why it's worth keeping:** Defines a critical status-driven state machine for progress tracking and includes specific 'CRITICAL' instructions to prevent async connection leaks in Lambda environments.

**Summary:** Provides deep architectural context for an AWS Lambda microservice, including its state machine, transaction patterns, and local development workflows.

**Source credibility:** Low public popularity (0 stars) but contains high-quality engineering patterns found in real production codebases.

**Recency:** Current; references recent LLM/AI toolsets like LlamaIndex and Gemini.

**Source:** [Nishant-ops/saksham-backend/lambda_functions/CLAUDE.md](https://github.com/Nishant-ops/saksham-backend/blob/7eae3c6e94950173bd529ac584f1ac3f0d69dba5/lambda_functions/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Lambda Functions Directory Overview

This directory contains AWS Lambda-compatible document and YouTube video processing functions. It operates as a **standalone microservice** separate from the main FastAPI application, designed to handle async background processing of learning resources.

## Development Commands

### Running Locally

```bash
# Run as FastAPI development server (for testing Lambda logic)
cd lambda_functions
python main.py
# Defaults to port 8002

# Test document processing endpoint
curl -X POST http://localhost:8002/process-document \
  -H "Content-Type: application/json" \
  -d '{"document_id": 123, "object_key": "path/to/file.pdf", "processing_strategy": "semantic"}'

# Test YouTube processing endpoint
curl -X POST http://localhost:8002/youtube/process \
  -H "Content-Type: application/json" \
  -d '{"video_id": "VIDEO_ID", "name": "Video Title"}'
```

### Testing Scripts

The directory contains various test scripts for development:

```bash
# Test YouTube chunking
python test_youtube_chunking.py

# Test semantic chunking
python test_semantic_c
```

</details>
