---
name: forcedotcom__SalesforceMobileSDK-Android__skill
source: https://github.com/forcedotcom/SalesforceMobileSDK-Android/blob/5184617db4cb93879c7118c6b9e0eab854959c9f/.claude/skills/update-sqlcipher/SKILL.md
repo: forcedotcom/SalesforceMobileSDK-Android
kind: skill
stars: 358
last_pushed: 2026-06-13T00:03:09Z
license: other
score: 9
domains: [android-dev, security, database]
tags: [sqlcipher, dependency-management, regression-testing]
curated: 2026-06-16
curated_by: config-scout
---

# forcedotcom/SalesforceMobileSDK-Android — skill

**Why it's worth keeping:** It goes beyond simple version bumping by providing specific pattern matching, historical breaking change warnings, and precise test validation requirements.

**Summary:** A highly detailed procedural skill for updating the SQLCipher dependency within an Android SDK.

**Source credibility:** High; based on a well-maintained, enterprise-grade Salesforce mobile SDK.

**Recency:** Very current, featuring recent/near-future versioning context.

**Source:** [forcedotcom/SalesforceMobileSDK-Android/.claude/skills/update-sqlcipher/SKILL.md](https://github.com/forcedotcom/SalesforceMobileSDK-Android/blob/5184617db4cb93879c7118c6b9e0eab854959c9f/.claude/skills/update-sqlcipher/SKILL.md) · 358★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Update SQLCipher Skill

This skill automates the process of updating the SQLCipher library version in the SalesforceMobileSDK-Android project.

## When to Use
Use this skill when you need to:
- Update SQLCipher to a newer version for security patches or new features
- Track changes in SQLCipher's OpenSSL provider version
- Handle API changes in new SQLCipher versions

## Background
SQLCipher is an open-source extension to SQLite that provides transparent 256-bit AES encryption of database files. The SDK uses it in the SmartStore library for secure local data storage.

## Parameters
- `NEW_VERSION`: The new SQLCipher version (e.g., "4.10.0", "4.11.0")
- `OLD_VERSION`: The current SQLCipher version (default: check build.gradle.kts)
- `NEW_PROVIDER_VERSION`: The cipher provider version bundled with the new SQLCipher (check SQLCipher release notes)

## Process

### 1. Research the New Version

Before starting, check the SQLCipher release notes:
- Visit: https://github.com/sqlcipher/sqlcipher/releases
- Review changes, breaking changes, and new features
- Note the provider version included (important for tests)
- Check for API changes that might affect the SDK

**Key things to look fo
```

</details>
