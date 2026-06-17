---
name: zane-ops__zane-ops
source: https://github.com/zane-ops/zane-ops/blob/3b4e6e5beb60e3df444004206cd23682fc8fe4da/CLAUDE.md
repo: zane-ops/zane-ops
kind: claude-md
stars: 1338
last_pushed: 2026-06-14T19:57:40Z
license: mit
score: 9
domains: [backend-api, devops, web-frontend]
tags: [personality-control, test-driven-development, workflow-strictness]
curated: 2026-06-14
curated_by: config-scout
---

# zane-ops/zane-ops — claude-md

**Why it's worth keeping:** The personality constraints are excellent for reducing 'AI noise,' while the specific command catalogs and architecture walkthroughs provide high-signal context for agentic task execution.

**Summary:** Establishes strict communication protocols to minimize AI verbosity/ego and enforces a rigorous test-first development workflow.

**Source credibility:** High; based on a popular (1.3k+ stars) and actively maintained open-source PaaS project.

**Recency:** Extremely current, featuring modern stacks like Django 5.2, React 19, and the uv package manager.

**Source:** [zane-ops/zane-ops/CLAUDE.md](https://github.com/zane-ops/zane-ops/blob/3b4e6e5beb60e3df444004206cd23682fc8fe4da/CLAUDE.md) · 1338★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## AI Chatbot Answer style

I DO NOT WANT YOU TO SAY : "AH ! I KNOW THE ISSUE !" OR "YOU ARE ABSOLUTELY RIGHT" OR SOMETHING SIMILAR. we try to debug the things together and I don't
want you to act as all knowing, please respond simply and unless you are
100% sure, don't respond like you figured it out, even if you are sure, be humble.

Be EXTREMELY concise. Short responses only. No blabbering.

## Code style

We use a **test-first approach**. When implementing features:
1. Write tests FIRST - nothing else
2. Tests will be validated and run by the human
3. If asked to "write tests", write ONLY tests - no implementation
4. Only implement the feature when explicitly asked to continue or implement
4. Never, EVER Import files at the top of functions & methods, always import them at the top of the file
5. look for built-in or installed libraries before doing something by hand

## About ZaneOps

ZaneOps is a self-hosted, open-source PaaS (Platform as a Service) for deploying web apps, static sites, databases, and services. It's an alternative to Heroku, Railway, and Render,
```

</details>
