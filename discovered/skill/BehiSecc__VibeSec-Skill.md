---
name: BehiSecc__VibeSec-Skill
source: https://github.com/BehiSecc/VibeSec-Skill/blob/0590993b35ad51961f65a4d01cf1196dfead05bb/SKILL.md
repo: BehiSecc/VibeSec-Skill
kind: skill
stars: 948
last_pushed: 2026-02-17T14:03:16Z
license: apache-2.0
score: 9
domains: [web-security, backend-api]
tags: [owasp, secure-coding, web-app]
curated: 2026-06-15
curated_by: config-scout
---

# BehiSecc/VibeSec-Skill — skill

**Why it's worth keeping:** It includes actionable implementation patterns (like using 404s to prevent enumeration) and highly specific checklists for XSS/CSRF sources.

**Summary:** A professional security directive that instructs Claude to adopt a 'bug hunter' mindset when writing or auditing web applications.

**Source credibility:** High popularity with ~950 stars and highly structured, expert-level security documentation.

**Recency:** 

**Source:** [BehiSecc/VibeSec-Skill/SKILL.md](https://github.com/BehiSecc/VibeSec-Skill/blob/0590993b35ad51961f65a4d01cf1196dfead05bb/SKILL.md) · 948★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: VibeSec-Skill
description: This skill helps Claude write secure web applications. Use this when working on any web application or when a user requests a scan or audit to ensure security best practices are followed.
---

# Secure Coding Guide for Web Applications

## Overview

This guide provides comprehensive secure coding practices for web applications. As an AI assistant, your role is to approach code from a **bug hunter's perspective** and make applications **as secure as possible** without breaking functionality.

**Key Principles:**
- Defense in depth: Never rely on a single security control
- Fail securely: When something fails, fail closed (deny access)
- Least privilege: Grant minimum permissions necessary
- Input validation: Never trust user input, validate everything server-side
- Output encoding: Encode data appropriately for the context it's rendered in

---

## Access Control Issues

Access control vulnerabilities occur when users can access resources or perform actions beyond their intended permissions.

### Core Requirements

For **every data point and action** that requires authentication:

1. **User-Level Authorization**
   - Each user must only access/mo
```

</details>
