---
name: alirezarezvani__claude-code-tresor__skill
source: https://github.com/alirezarezvani/claude-code-tresor/blob/4b680504d29a205380436e9970eccf8faa28d21d/skills/documentation/api-documenter/SKILL.md
repo: alirezarezvani/claude-code-tresor
kind: skill
stars: 731
last_pushed: 2026-05-19T02:11:20Z
license: mit
score: 9
domains: [backend-api, devops, documentation]
tags: [openapi, swagger, automation, api-design]
curated: 2026-06-15
curated_by: config-scout
---

# alirezarezvani/claude-code-tresor — skill

**Why it's worth keeping:** Provides structured 'Detection Logic' for framework recognition and defines explicit 'Activation Triggers' that turn a passive tool into an autonomous maintenance agent.

**Summary:** Automates the generation of OpenAPI/Swagger specifications by scanning code routes, controllers, and docstrings across multiple web frameworks.

**Source credibility:** High popularity with 731 stars on GitHub.

**Recency:** Highly relevant to current modern web development stacks like FastAPI and Express.js.

**Source:** [alirezarezvani/claude-code-tresor/skills/documentation/api-documenter/SKILL.md](https://github.com/alirezarezvani/claude-code-tresor/blob/4b680504d29a205380436e9970eccf8faa28d21d/skills/documentation/api-documenter/SKILL.md) · 731★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: api-documenter
description: Auto-generate API documentation from code and comments. Use when API endpoints change, or user mentions API docs. Creates OpenAPI/Swagger specs from code. Triggers on API file changes, documentation requests, endpoint additions.
allowed-tools: Read, Write, Grep
---

# API Documenter Skill

Auto-generate API documentation from code.

## When I Activate

- ✅ API endpoints added/modified
- ✅ User mentions API docs, OpenAPI, or Swagger
- ✅ Route files changed
- ✅ Controller files modified
- ✅ Documentation needed

## What I Generate

### OpenAPI 3.0 Specifications
- Endpoint descriptions
- Request/response schemas
- Authentication requirements
- Example payloads
- Error responses

### Formats Supported
- OpenAPI 3.0 (JSON/YAML)
- Swagger 2.0
- API Blueprint
- RAML

## Examples

### Express.js Endpoint

```javascript
// You write:
/**
 * Get user by ID
 * @param {string} id - User ID
 * @returns {User} User object
 */
app.get('/api/users/:id', async (req, res) => {
  const user = await User.findById(req.params.id);
  res.json(user);
});

// I auto-generate OpenAPI spec:
paths:
  /api/users/{id}:
    get:
      summary: Get user by ID
      parameter
```

</details>
