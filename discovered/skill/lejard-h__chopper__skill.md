---
name: lejard-h__chopper__skill
source: https://github.com/lejard-h/chopper/blob/7e36d84605f649b7c5dd23558c2d5f752b6b5bf1/skills/chopper/SKILL.md
repo: lejard-h/chopper
kind: skill
stars: 746
last_pushed: 2026-06-08T19:16:30Z
license: other
score: 9
domains: [dart, flutter, api-client]
tags: [http-client, code-generation, dart]
curated: 2026-06-15
curated_by: config-scout
---

# lejard-h/chopper — skill

**Why it's worth keeping:** It utilizes advanced agentic patterns like 'Start With Inputs' to reduce ambiguity and 'Core Rules' to prevent common technical hallucinations regarding syntax and generation.

**Summary:** A highly specialized skill for implementing the Chopper HTTP client in Dart and Flutter environments.

**Source credibility:** High; based on a popular, actively maintained open-source library with significant community adoption.

**Recency:** Current; uses modern Dart/Flutter CLI conventions such as 'dart run build_runner'.

**Source:** [lejard-h/chopper/skills/chopper/SKILL.md](https://github.com/lejard-h/chopper/blob/7e36d84605f649b7c5dd23558c2d5f752b6b5bf1/skills/chopper/SKILL.md) · 746★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chopper
description: Use this skill whenever a user wants to install, configure, write, generate, debug, or choose options for Chopper HTTP clients in Dart or Flutter, including @ChopperApi services, ChopperClient setup, build_runner/chopper_generator, converters, interceptors, response handling, query parameters, or chopper_built_value integration.
---

# Chopper Usage Assistant

Help users build Dart and Flutter HTTP clients with Chopper. Focus on application code, generated service setup, and interoperability outcomes, not repository maintenance.

## Start With Inputs

Before producing a final snippet, collect only details that change the code:

- Runtime: Dart package, Dart server/CLI, Flutter app, or test.
- API shape: base URL, service base path, endpoint paths, methods, headers, path/query parameters, request bodies, and expected status handling.
- Response handling: raw `Response`, nullable/no-content endpoint, typed body, JSON map/list, custom model converter, stream, file, or error body.
- Serialization approach: built-in `JsonConverter`, custom converter, `json_serializable`, `built_value`, form URL encoding, multipart, or raw body.
- Generation issue details:
```

</details>
