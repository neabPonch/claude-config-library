---
name: ceb10n__pydantic-settings-aws__skill
source: https://github.com/ceb10n/pydantic-settings-aws/blob/b1532b9a513a5d854645b8ffe5f5a393c0f942b0/pydantic_settings_aws/.agents/skills/SKILL.md
repo: ceb10n/pydantic-settings-aws
kind: skill
stars: 24
last_pushed: 2026-04-08T13:15:16Z
license: mit
score: 9
domains: [backend, cloud-infrastructure, python]
tags: [pydantic, aws, configuration]
curated: 2026-06-15
curated_by: config-scout
---

# ceb10n/pydantic-settings-aws — skill

**Why it's worth keeping:** It uses a decision matrix for base class selection, includes 'Critical Rules' to prevent common import errors, and demonstrates advanced routing via `Annotated` types.

**Summary:** Provides structured instructions for implementing type-safe settings loading from AWS Secrets Manager and SSM using Pydantic.

**Source credibility:** A specialized library with professional-grade documentation structure and recent activity.

**Recency:** Current; follows modern Pydantic v2 standards and was updated recently.

**Source:** [ceb10n/pydantic-settings-aws/pydantic_settings_aws/.agents/skills/SKILL.md](https://github.com/ceb10n/pydantic-settings-aws/blob/b1532b9a513a5d854645b8ffe5f5a393c0f942b0/pydantic_settings_aws/.agents/skills/SKILL.md) · 24★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# pydantic-settings-aws skill

## Overview

`pydantic-settings-aws` extends [Pydantic Settings](https://docs.pydantic.dev/latest/concepts/pydantic_settings/) to load settings from AWS Secrets Manager and AWS Systems Manager Parameter Store.

- Version: 1.0.0b1
- Requires: Python >= 3.10, pydantic >= 2.0.1, pydantic-settings >= 2.0.2, boto3 >= 1.27.0

## Critical rules

- Always use `AWSSettingsConfigDict` (from `pydantic_settings_aws`) instead of pydantic-settings' `SettingsConfigDict`. `AWSSettingsConfigDict` extends it and adds autocomplete and type safety for all AWS-specific keys.
- Never import `SettingsConfigDict` from `pydantic_settings` when using this library.
- The boto3 client cache is thread-safe and safe for free-threaded Python (no-GIL) builds.

## Base classes

Choose the base class that matches your use case:

| Class | Use when |
| :---- | :------- |
| `SecretsManagerBaseSettings` | All settings come from a single Secrets Manager secret (JSON) |
| `ParameterStoreBaseSettings` | All settings come from SSM Parameter Store parameters |
| `AWSBaseSettings` | Settings come from both Secrets Manager and Parameter Store |

## AWSSettingsConfigDict keys

### boto3 session
```

</details>
