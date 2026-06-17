---
name: fukuball__jieba-php
source: https://github.com/fukuball/jieba-php/blob/052abb73f5f94267efd455ce5384b1c8bdd09ae2/CLAUDE.md
repo: fukuball/jieba-php
kind: claude-md
stars: 1379
last_pushed: 2025-12-16T03:39:39Z
license: mit
score: 9
domains: [backend-api, data-processing, nlp]
tags: [php, architecture-documentation, resource-management]
curated: 2026-06-15
curated_by: config-scout
---

# fukuball/jieba-php — claude-md

**Why it's worth keeping:** The inclusion of 'Initialization Patterns' and explicit 'Memory Requirements' provides critical operational guardrails that prevent AI-driven runtime failures.

**Summary:** Provides deep architectural context including initialization patterns, resource requirements, and specific security constraints.

**Source credibility:** High; 1379 stars indicates a widely-used, stable PHP component.

**Recency:** Current; last pushed within the last 6 months.

**Source:** [fukuball/jieba-php/CLAUDE.md](https://github.com/fukuball/jieba-php/blob/052abb73f5f94267efd455ce5384b1c8bdd09ae2/CLAUDE.md) · 1379★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Common Commands

### Testing
- Run all tests: `./vendor/bin/phpunit`
- Run tests with coverage: `./vendor/bin/phpunit --coverage-clover=build/logs/clover.xml`
- Run specific test: `./vendor/bin/phpunit test/JiebaTest.php`
- Run custom POS tag tests: `./vendor/bin/phpunit test/CustomPosTagTest.php`
- Run security tests: `./vendor/bin/phpunit test/SecurityTest.php`
- Run user dictionary tests: `./vendor/bin/phpunit test/UserDictTest.php`
- Run memory management tests: `./vendor/bin/phpunit test/MemoryManagementTest.php`

### Code Quality
- Code style check: `./vendor/bin/phpcs`
- PSR2 standard check: `./vendor/bin/phpcs --standard=PSR2 --extensions=php --ignore="*/test/*" ./src/class`
- Code linting: `./vendor/bin/phpcs --standard=PSR2 src/`

### Demo Scripts
- Basic segmentation: `php src/cmd/demo.php`
- Keyword extraction: `php src/cmd/demo_extract_tags.php`
- Part-of-speech tagging: `php src/cmd/demo_posseg.php`
- Custom dictionary: `php src/cmd/demo_user_dict.php`
- Tokenization with positions: `php src/cmd/demo_tokenize.php`
- **Custom POS tagging**: `php src/c
```

</details>
