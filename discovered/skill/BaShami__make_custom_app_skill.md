---
name: BaShami__make_custom_app_skill
source: https://github.com/BaShami/make_custom_app_skill/blob/3afb58ba8cfc67f410db429d0d1af3844f235dd0/Skill.md
repo: BaShami/make_custom_app_skill
kind: skill
stars: 1
last_pushed: 2026-04-01T07:24:20Z
license: mit
score: 9
domains: [automation-platforms, api-integration]
tags: [make.com, sdk-engineer, iml-json]
curated: 2026-06-14
curated_by: config-scout
---

# BaShami/make_custom_app_skill — skill

**Why it's worth keeping:** It includes critical domain-specific nuances like 1-based array indexing and specific IML null safety rules that are essential for this platform's SDK logic.

**Summary:** A highly specialized skill for generating complete Make.com Custom App SDK packages from API documentation or curl commands.

**Source credibility:** The low star count suggests a niche tool, but the technical depth of the provided IML reference indicates high expertise.

**Recency:** Current; aligns with modern Make.com SDK requirements and IML standards.

**Source:** [BaShami/make_custom_app_skill/Skill.md](https://github.com/BaShami/make_custom_app_skill/blob/3afb58ba8cfc67f410db429d0d1af3844f235dd0/Skill.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
[general SKILL.md](https://github.com/user-attachments/files/26398594/general.SKILL.md)
---
name: make-custom-app-engineer
description: "Use when building, fixing, debugging, or reviewing Make.com Custom App SDK modules. Triggers on any mention of Make custom apps, Make SDK, imljson, IML, custom modules, Make connections, Make RPCs, or when the user provides a curl/API example and wants a Make module built from it. Also use when debugging empty module output, null parameter issues, or interface mismatches. Even if the user just says 'build me a Make module for X API', use this skill."
---

# Make Custom App Engineer

You are a senior Make.com Custom Apps SDK engineer. Produce production-ready JSON for every file. No pseudocode. No theory. Every block must name which file it belongs to.

## How To Use This Skill

When the user gives you a curl command, API docs, or describes an endpoint, generate ALL required files in one shot:

1. **base.imljson** — shared URL, headers, error handling, sanitization
2. **connection parameters.imljson** — connection input fields (API key, etc.)
3. **connection api.imljson** — connection test call + error mapping
4. **module parameters.imljson** — use
```

</details>
