---
name: phpstan__phpstan
source: https://github.com/phpstan/phpstan/blob/d53820c1be1b60fa3ace89acdc488c98f465b6fd/CLAUDE.md
repo: phpstan/phpstan
kind: claude-md
stars: 13997
last_pushed: 2026-06-15T17:11:31Z
license: mit
score: 7
domains: [cli-tools, php]
tags: [architecture, context-mapping, boundary-definition]
curated: 2026-06-15
curated_by: config-scout
---

# phpstan/phpstan — claude-md

**Why it's worth keeping:** The 'Making Changes' and 'Key Concepts' sections provide essential meta-instructions that prevent an agent from wasting effort editing the wrong repo. It also uses a high-density tree structure to map the project ecosystem.

**Summary:** Provides crucial architectural boundaries by distinguishing the distribution repository from the actual source code repository.

**Source credibility:** Extremely high; PHPStan is a major industry-standard static analysis tool with massive community adoption.

**Recency:** Current; reflects modern multi-architecture CI/CD and cross-repository dependencies.

**Source:** [phpstan/phpstan/CLAUDE.md](https://github.com/phpstan/phpstan/blob/d53820c1be1b60fa3ace89acdc488c98f465b6fd/CLAUDE.md) · 13997★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# PHPStan - PHP Static Analysis Tool

## Project Overview

PHPStan finds errors in PHP code without running it. It catches bugs before tests are written, moving PHP closer to compiled languages. This is the **distribution repository** — the compiled PHAR and supporting infrastructure. The actual source code lives at [phpstan/phpstan-src](https://github.com/phpstan/phpstan-src).

- **Website:** https://phpstan.org/
- **Documentation:** https://phpstan.org/user-guide/getting-started
- **API Reference:** https://apiref.phpstan.org/

## Repository Structure

```
├── phpstan                    # CLI entry point (shell script loading the PHAR)
├── phpstan.phar               # Compiled PHAR archive (~26 MB)
├── phpstan.phar.asc           # GPG signature for the PHAR
├── bootstrap.php              # PHAR autoloader with PHP version polyfills
├── composer.json              # Package definition (requires PHP ^7.4|^8.0)
├── .phar-checksum             # MD5 + SHA1 checksums for reproducible builds
├── conf/
│   └── bleedingEdge.neon      # Bleeding edge configuration profile
├── e2e/                       # End-to-end tests (~67 test scenarios)
├── docker/                    # Dockerfiles for
```

</details>
