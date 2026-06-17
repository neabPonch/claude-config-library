---
name: HemmeligOrg__Hemmelig.app
source: https://github.com/HemmeligOrg/Hemmelig.app/blob/08511da63ae0b2017ec6c43fc6740b98cfc3c4e6/CLAUDE.md
repo: HemmeligOrg/Hemmelig.app
kind: claude-md
stars: 1215
last_pushed: 2026-06-12T22:20:09Z
license: other
score: 9
domains: [security, web-frontend, backend-api]
tags: [zero-knowledge, encryption, react, typescript]
curated: 2026-06-15
curated_by: config-scout
---

# HemmeligOrg/Hemmelig.app — claude-md

**Why it's worth keeping:** The 'Security Model' section is an excellent example of providing high-stakes constraints to prevent the AI from introducing security regressions. The inclusion of specific encryption algorithms/iterations and full directory maps makes it highly effective for tool-use/navigation.

**Summary:** A highly detailed technical guide for a zero-knowledge secret-sharing application that provides critical architectural guardrails and project context.

**Source credibility:** High; comes from a popular (1200+ stars), actively maintained open-source project.

**Recency:** Very recent; uses cutting-edge technologies like React 19 and Tailwind v4.

**Source:** [HemmeligOrg/Hemmelig.app/CLAUDE.md](https://github.com/HemmeligOrg/Hemmelig.app/blob/08511da63ae0b2017ec6c43fc6740b98cfc3c4e6/CLAUDE.md) · 1215★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude AI Assistant Guidelines for Hemmelig.app

Welcome to Hemmelig.app! This guide will help you navigate our codebase and contribute effectively. Think of this document as your onboarding buddy - it covers everything you need to know to maintain code quality, security, and architectural consistency.

## What is Hemmelig?

Hemmelig.app is a secure secret-sharing application that lets users share encrypted messages that automatically self-destruct after being read. The name "Hemmelig" means "secret" in Norwegian - fitting, right?

### The Security Model You Must Understand

**CRITICAL: Zero-Knowledge Architecture**

This is the heart of Hemmelig. Before you write a single line of code, make sure you understand this:

- All encryption/decryption happens **client-side only** using the Web Crypto API
- The server **never** sees plaintext secrets - only encrypted blobs
- Decryption keys live in URL fragments (`#decryptionKey=...`), which browsers **never send to servers**
- This is our fundamental security promise to users - **do not compromise this under any circumstances**

### How Encryption Works

| Component          | Details
```

</details>
