---
name: PhenoML__ClaudeFHIRSkill
source: https://github.com/PhenoML/ClaudeFHIRSkill/blob/f472b762acd0511da892963ec940431f5d57c58a/SKILL.md
repo: PhenoML/ClaudeFHIRSkill
kind: skill
stars: 50
last_pushed: 2026-06-02T19:31:23Z
license: apache-2.0
score: 8
domains: [healthcare, backend-api, data-modeling]
tags: [fhir, hl7, pydantic, fastapi, typescript]
curated: 2026-06-16
curated_by: config-scout
---

# PhenoML/ClaudeFHIRSkill — skill

**Why it's worth keeping:** It provides high-value code templates for Pydantic models and search parameter parsing, alongside a smart strategy for managing local specification caches to ensure consistency.

**Summary:** A specialized guide for building FHIR-compliant healthcare software, covering API design, resource modeling, and validation workflows.

**Source credibility:** A specialized niche repository with decent social proof (50 stars) and recent activity.

**Recency:** Highly relevant to current agentic development workflows requiring deep domain-specific architectural patterns.

**Source:** [PhenoML/ClaudeFHIRSkill/SKILL.md](https://github.com/PhenoML/ClaudeFHIRSkill/blob/f472b762acd0511da892963ec940431f5d57c58a/SKILL.md) · 50★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: fhir-software
description: Comprehensive FHIR (Fast Healthcare Interoperability Resources) software development assistant. Use when working with FHIR APIs, implementations, or healthcare data exchange. Supports FHIR R4, R4B, R5, Implementation Guides (IGs), FHIR Shorthand (FSH) authoring, SUSHI, GoFSH, validation, terminology, and SMART on FHIR. Ideal for building FHIR servers, clients, validators, IG authors, or healthcare applications that need to process FHIR resources.
---

# FHIR Software Development Skill

Expert guidance for building robust FHIR (Fast Healthcare Interoperability Resources) software systems with comprehensive package management, spec knowledge, and development workflows.

## Core Architecture

### 1. Package/Specification Management

**Local FHIR Package Cache:**
- Use `@fhir/package-loader` or equivalent for TypeScript/Node.js environments
- For Python: `fhir-package-loader` or custom implementation using `requests` + `json`
- Cache strategy: `~/.fhir/packages/` with version-specific directories
- Support packages: `hl7.fhir.r4.core`, `hl7.fhir.r5.core`, Implementation Guides

**Package Resolution Pattern:**
```typescript
// Load and cache FHIR pac
```

</details>
