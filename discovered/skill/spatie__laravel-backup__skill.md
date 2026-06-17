---
name: spatie__laravel-backup__skill
source: https://github.com/spatie/laravel-backup/blob/139ad24f3633a3bea8222ebf561f59277b924821/resources/boost/skills/laravel-backup/SKILL.md
repo: spatie/laravel-backup
kind: skill
stars: 5996
last_pushed: 2026-06-10T08:26:38Z
license: mit
score: 9
domains: [backend, devops, php]
tags: [laravel, backup, automation, cli-tools]
curated: 2026-06-15
curated_by: config-scout
---

# spatie/laravel-backup — skill

**Why it's worth keeping:** Includes a 'Common Pitfalls' section to help the agent proactively debug, plus clear boilerplate patterns for implementing advanced custom strategies (Cleanup/Health/Notifications).

**Summary:** Provides comprehensive context for configuring, executing, and extending the Spatie Laravel Backup package via CLI commands, scheduling, and custom class implementations.

**Source credibility:** Extremely high; Spatie is one of the most respected developer tool creators in the Laravel ecosystem.

**Recency:** Current; uses modern Laravel scheduling syntax and follows up-to-date package documentation standards.

**Source:** [spatie/laravel-backup/resources/boost/skills/laravel-backup/SKILL.md](https://github.com/spatie/laravel-backup/blob/139ad24f3633a3bea8222ebf561f59277b924821/resources/boost/skills/laravel-backup/SKILL.md) · 5996★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: laravel-backup
description: "Configure and extend spatie/laravel-backup for database and file backups, cleanup strategies, health monitoring, and notifications. Activates when working with backup configuration, scheduling backups, creating custom cleanup strategies or health checks, customizing notifications, or when the user mentions backups, backup monitoring, backup cleanup, or spatie/laravel-backup."
license: MIT
metadata:
  author: spatie
---
# Laravel Backup

## When to Apply

Activate this skill when:

- Configuring backup sources, destinations, or notifications
- Scheduling backup, cleanup, or monitor commands
- Creating custom cleanup strategies or health checks
- Customizing backup notifications
- Troubleshooting backup failures

## Key Commands

```bash
# Run a backup
php artisan backup:run

# Backup only the database
php artisan backup:run --only-db

# Backup specific database connections
php artisan backup:run --db-name=mysql --db-name=pgsql

# Backup only files (no database)
php artisan backup:run --only-files

# Backup to a specific disk
php artisan backup:run --only-to-disk=s3

# Custom filename
php artisan backup:run --filename=my-backup.zip

# Clean old
```

</details>
