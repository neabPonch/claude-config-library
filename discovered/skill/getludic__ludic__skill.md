---
name: getludic__ludic__skill
source: https://github.com/getludic/ludic/blob/4b3e544b8d71c719f9cc4079510b83feb5cd59c0/skills/ludic-web/SKILL.md
repo: getludic/ludic
kind: skill
stars: 889
last_pushed: 2026-06-08T20:14:24Z
license: mit
score: 9
domains: [web-development, python, security]
tags: [html-templates, fastapi, django, htmx, security]
curated: 2026-06-15
curated_by: config-scout
---

# getludic/ludic — skill

**Why it's worth keeping:** The skill description includes an expert security instruction to trigger on absolute URL generation to prevent host header poisoning. This transforms a documentation file into a proactive security auditing rule for the agent.

**Summary:** A specialized guide for integrating Ludic components into Starlette, FastAPI, and Django web applications. It covers type-safe endpoints, htmx response patterns, and request handling.

**Source credibility:** High; the source repo is well-starred (889) and actively maintained.

**Recency:** Very recent/current, aligned with modern ASGI and FastAPI ecosystems.

**Source:** [getludic/ludic/skills/ludic-web/SKILL.md](https://github.com/getludic/ludic/blob/4b3e544b8d71c719f9cc4079510b83feb5cd59c0/skills/ludic-web/SKILL.md) · 889★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ludic-web
description: >-
  Build web apps with Ludic's web integration — Starlette-based LudicApp,
  typed Endpoint classes, and the FastAPI / Django integrations. Use this
  skill whenever the user is wiring Ludic components into HTTP handlers:
  routing requests with LudicApp, declaring async endpoints that return
  components, subclassing ludic.web.endpoints.Endpoint, parsing form data
  or query params, returning htmx partials, handling redirects, mounting
  Ludic inside an existing FastAPI or Django app, or generating URLs from
  a request (request.url_for / request.url_path_for). Always trigger this
  skill on any code that generates absolute URLs from request data — there
  is a host header poisoning class of vulnerability that affects every
  Ludic web app and needs explicit guarding. Also trigger on questions
  about LudicRequest, LudicResponse, the Starlette/FastAPI/Django bridge,
  or htmx response patterns (HX-Trigger, HX-Redirect, HX-Push-Url
  headers). For pure component authoring without an HTTP layer, use the
  companion `ludic-components` skill.
metadata:
  type: framework-guide
  framework: ludic
  version: "1.x"
---

# Ludic Web

This skill covers the
```

</details>
