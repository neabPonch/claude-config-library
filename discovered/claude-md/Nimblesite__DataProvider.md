---
name: Nimblesite__DataProvider
source: https://github.com/Nimblesite/DataProvider/blob/8e3af366e20d1b8db548fdbf20c23314a6a1927a/CLAUDE.md
repo: Nimblesite/DataProvider
kind: claude-md
stars: 66
last_pushed: 2026-05-11T11:14:40Z
license: mit
score: 9
domains: [backend-api, systems-programming, cli-tools]
tags: [functional-programming, strict-typing, multi-agent-orchestration, source-generation]
curated: 2026-06-15
curated_by: config-scout
---

# Nimblesite/DataProvider — claude-md

**Why it's worth keeping:** Excellent use of 'Hard Rules' to override LLM defaults (e.g., preventing OOP in C#) and includes high-signal meta-instructions for token reduction and file locking.

**Summary:** Enforces a strict functional programming paradigm across C#, Rust, and TypeScript while providing advanced instructions for multi-agent orchestration.

**Source credibility:** The repo has active maintenance and highly specific architectural requirements typical of high-end systems tooling.

**Recency:** Current; it targets .NET 10.0 and addresses modern multi-agent coordination challenges.

**Source:** [Nimblesite/DataProvider/CLAUDE.md](https://github.com/Nimblesite/DataProvider/blob/8e3af366e20d1b8db548fdbf20c23314a6a1927a/CLAUDE.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DataProvider — Agent Instructions

⚠️ CRITICAL: **Reduce token usage.** Check file size before loading. Write less. Delete fluff and dead code. Alert user when context is loaded with pointless files. ⚠️ 

> Read this entire file before writing any code.
> These rules are NON-NEGOTIABLE. Violations will be rejected in review.

⚠️ NEVER KILL ANY VSCODE PROCESS ⚠️

<!-- agent-pmo:74cf183 -->

## Project Overview

DataProvider is a comprehensive .NET database access toolkit: source generation for SQL extension methods, the Lambda Query Language (LQL) transpiler, bidirectional offline-first sync, WebAuthn + RBAC auth, and an embeddable reporting platform. The LQL LSP is implemented in Rust with a VS Code extension in TypeScript. Healthcare sample applications live in a separate repo: [Nimblesite/ClinicalCoding](https://github.com/Nimblesite/ClinicalCoding).

**Primary language(s):** C# (.NET 10.0), Rust, TypeScript, F#
**Build command:** `make ci`
**Test command:** `make test`
**Lint command:** `make lint`

The LQL parser is ANTLR generated in Rust. We don't use manually generated parsers. Always upgrade to the latest version of ANTLR to make sure the parser is correct.

## Too Many C
```

</details>
