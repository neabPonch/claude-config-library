---
name: dykyi-roman__awesome-claude-code__skill
source: https://github.com/dykyi-roman/awesome-claude-code/blob/2897d0739800316076869d48b6819f7dd3b64fa4/skills/check-cors-security/SKILL.md
repo: dykyi-roman/awesome-claude-code
kind: skill
stars: 80
last_pushed: 2026-02-22T19:56:16Z
license: mit
score: 9
domains: [security, backend-api, php]
tags: [cors, security-audit, owasp, php]
curated: 2026-06-15
curated_by: config-scout
---

# dykyi-roman/awesome-claude-code — skill

**Why it's worth keeping:** The inclusion of actionable grep patterns for discovery and a strictly defined output format makes it highly effective for autonomous agents. The 'vulnerable vs. correct' code examples provide excellent pattern-matching context.

**Summary:** A specialized security audit tool designed to detect CORS misconfigurations in PHP environments. It includes specific code patterns, search commands, and severity levels.

**Source credibility:** Strong; specialized PHP architecture toolkit with significant community interest (80 stars).

**Recency:** Highly relevant to current security standards and modern PHP practices.

**Source:** [dykyi-roman/awesome-claude-code/skills/check-cors-security/SKILL.md](https://github.com/dykyi-roman/awesome-claude-code/blob/2897d0739800316076869d48b6819f7dd3b64fa4/skills/check-cors-security/SKILL.md) · 80★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: check-cors-security
description: Audits CORS configuration security. Detects wildcard origins, credentials with wildcards, dynamic origin reflection, missing preflight handling, and overly permissive policies.
---

# CORS Security Audit (A05:2021)

Analyze PHP code for CORS misconfiguration vulnerabilities.

## Detection Patterns

### 1. Wildcard Origin

```php
// CRITICAL: Allows any website to make requests
header('Access-Control-Allow-Origin: *');

// In framework config:
'allowed_origins' => ['*'], // Any origin!
```

### 2. Credentials with Wildcard

```php
// CRITICAL: Browser ignores this (spec violation), but shows misconfiguration intent
header('Access-Control-Allow-Origin: *');
header('Access-Control-Allow-Credentials: true');
// Cannot use * with credentials — forces dynamic origin reflection
```

### 3. Dynamic Origin Reflection (Dangerous)

```php
// CRITICAL: Reflects any Origin header — equivalent to wildcard with credentials
class CorsMiddleware
{
    public function handle(Request $request, Response $response): Response
    {
        $origin = $request->headers->get('Origin');
        $response->headers->set('Access-Control-Allow-Origin', $origin); // Ref
```

</details>
