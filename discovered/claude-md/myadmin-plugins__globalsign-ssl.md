---
name: myadmin-plugins__globalsign-ssl
source: https://github.com/myadmin-plugins/globalsign-ssl/blob/d4944550049acb9929e298551830c78c56263f9d/CLAUDE.md
repo: myadmin-plugins/globalsign-ssl
kind: claude-md
stars: 6
last_pushed: 2026-05-02T02:39:46Z
license: unknown
score: 8
domains: [php, soap-api, backend-plugin]
tags: [php, soap, plugin-architecture]
curated: 2026-06-15
curated_by: config-scout
---

# myadmin-plugins/globalsign-ssl — claude-md

**Why it's worth keeping:** The 'Key Patterns' section is excellent; it details specific API request structures, auth requirements, and state transition logic (e.g., order flow) that prevents an agent from making logical errors.

**Summary:** Provides high-density architectural mappings and business logic flows for a SOAP-based PHP plugin. It effectively bridges the gap between code structure and operational workflows.

**Source credibility:** Small/specialized repository with active maintenance.

**Recency:** Current; utilizes modern project-specific tooling integration.

**Source:** [myadmin-plugins/globalsign-ssl/CLAUDE.md](https://github.com/myadmin-plugins/globalsign-ssl/blob/d4944550049acb9929e298551830c78c56263f9d/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# MyAdmin GlobalSign SSL Plugin

Integrates GlobalSign SOAP API for SSL certificate ordering, renewal, and lifecycle management within the MyAdmin billing system.

## Commands

```bash
composer install                          # install dependencies
composer exec phpunit                     # run unit tests (config: phpunit.xml.dist)
composer exec phpunit tests/unit          # run unit suite only
composer exec phpunit -- --coverage-text  # run with coverage report
```

```bash
# Run a specific test file
composer exec phpunit tests/unit/GlobalSignClassTest.php
composer exec phpunit tests/unit/PluginClassTest.php
```

```bash
# Verify SOAP extension is loaded (required by this plugin)
php -m | grep soap
# Check composer autoload is up to date
composer dump-autoload
```

## Architecture

**Namespace**: `Detain\MyAdminGlobalSign\` → `src/` (PSR-4 via `composer.json`)

**Core classes**:
- `src/GlobalSign.php` — SOAP API client. Wraps three SOAP clients (`functionsClient`, `queryClient`, `accountClient`) for GlobalSign endpoints. Handles order creation, renewal, CSR validation, approver lists, and certificate queries.
- `src/Plugin.php` — MyAdmin plugin. Registers event hooks via `getHoo
```

</details>
