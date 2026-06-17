---
name: seanlgirgis__jobsearch__project-summary-for-claude
source: https://github.com/seanlgirgis/jobsearch/blob/5722b8b4ae4062d282e0dc312b0ab0e6ed3bc61e/docs/project_summary_for_claude.md
repo: seanlgirgis/jobsearch
kind: claude-md
stars: 0
last_pushed: 2026-05-27T17:11:50Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, data-pipelines]
tags: [rag, automation, workflow, python]
curated: 2026-06-16
curated_by: config-scout
---

# seanlgirgis/jobsearch — claude-md

**Why it's worth keeping:** The 'Data Architecture' section provides a perfect template for explaining how state moves through a file-based system to an AI agent. The 'Pipeline Scripts Detailed Breakdown' is an excellent way to provide high-level logic context without forcing the agent to scan every file first.

**Summary:** A comprehensive guide for an AI-driven job application pipeline that utilizes flat files and RAG instead of a traditional database. It details the environment setup, data flow, and functional purpose of every script in the system.

**Source credibility:** A personal project with low visibility, but the highly structured documentation indicates expert-level technical communication.

**Recency:** 

**Source:** [seanlgirgis/jobsearch/docs/project_summary_for_claude.md](https://github.com/seanlgirgis/jobsearch/blob/5722b8b4ae4062d282e0dc312b0ab0e6ed3bc61e/docs/project_summary_for_claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# JobSearch Project Summary for Claude

This document provides a complete, end-to-end summary of the JobSearch project. It is intended to give Claude complete context over the system's architecture, data flow, scripts, and environment setup.

## 1. Project Overview

The project is an AI-powered job application engine. It takes raw job postings and automates the process of checking for duplicates, scoring the job fit against a master career profile, tailoring a resume, researching the company, generating a custom cover letter, and tracking the application status. 

There is no traditional database. The system relies entirely on flat files (JSON, YAML, Markdown) and a local binary FAISS vector index.

## 2. Environment Setup (`env_setter.ps1`)

The environment is managed via a PowerShell script `env_setter.ps1` which activates the Virtual Environment and exports necessary environment variables. The script:
1. Activates the Python 3.12 virtual environment located at `C:\py_venv\JobSearch`.
2. Sets `PROJECT_ROOT` to the directory containing the script (`C:\jobsearch`).
3. Appends `src` to the `PYTHONPATH`.
4. Configures necessary storage paths mapping to folders within the project (`JO
```

</details>
