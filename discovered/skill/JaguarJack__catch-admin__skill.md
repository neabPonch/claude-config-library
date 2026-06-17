---
name: JaguarJack__catch-admin__skill
source: https://github.com/JaguarJack/catch-admin/blob/e282d6fbfb28dd18b52587cd7d1795472ea7cf9f/.claude/skills/curd/SKILL.md
repo: JaguarJack/catch-admin
kind: skill
stars: 915
last_pushed: 2026-05-30T02:47:16Z
license: apache-2.0
score: 9
domains: [backend-api, fullstack-scaffolding, php-laravel]
tags: [crud, orchestration, scaffolding, laravel]
curated: 2026-06-15
curated_by: config-scout
---

# JaguarJack/catch-admin — skill

**Why it's worth keeping:** Uses an advanced 'orchestration' pattern with explicit pre-checks, output contracts, and post-generation validation steps. The template includes rigorous logic for field type mapping and cross-layer dependency management.

**Summary:** An orchestration-level skill that generates complete full-stack CRUD modules from a database definition. It uses a multi-step sub-skill pipeline to ensure consistency across migrations, models, controllers, and frontend views.

**Source credibility:** High; sourced from a specialized, starred PHP framework repository (CatchAdmin).

**Recency:** 

**Source:** [JaguarJack/catch-admin/.claude/skills/curd/SKILL.md](https://github.com/JaguarJack/catch-admin/blob/e282d6fbfb28dd18b52587cd7d1795472ea7cf9f/.claude/skills/curd/SKILL.md) · 915★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: curd
description: Generates complete CRUD module from database table definition. Orchestrates 9 sub-skills. Use when user says "create CRUD", "generate module from table", or provides a table structure.
globs:
  - "modules/**/*.php"
  - "web/src/views/**/*.vue"
---

# CatchAdmin CRUD Generator

**一键生成完整 CRUD 模块** - 从数据表定义到前后端完整实现。

## Sub-Skills (9 个子 Skills)

| Step | Skill | 生成文件 |
|------|-------|----------|
| 1 | `01-parse-table` | - (解析输入) |
| 2 | `02-migration` | `database/migrations/*.php` |
| 3 | `03-model` | `Models/{Model}.php` |
| 4 | `04-controller` | `Http/Controllers/{Model}Controller.php` |
| 5 | `05-request` | `Http/Requests/{Model}Request.php` |
| 6 | `06-routes` | `routes/route.php` |
| 7 | `07-export` | `Export/{Model}.php` |
| 8 | `08-import` | `Import/{Model}.php` |
| 9 | `09-vue-pages` | `index.vue` + `create.vue` |

---

## Input: Table Definition

```
Table: products
Fields:
- id (primary key)
- name (string, 100, required)
- category_id (foreign key -> categories)
- description (text, nullable)
- price (decimal 10,2, required)
- stock (integer, default 0)
- status (tinyint, default 1)
```

---

## Output: Complete Module Structure

```
modules/{Mo
```

</details>
