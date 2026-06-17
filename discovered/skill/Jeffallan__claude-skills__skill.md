---
name: Jeffallan__claude-skills__skill
source: https://github.com/Jeffallan/claude-skills/blob/e8be415bc94d8d6ebddc2fb50e5d03c6e27d4319/skills/rails-expert/SKILL.md
repo: Jeffallan/claude-skills
kind: skill
stars: 9915
last_pushed: 2026-05-20T13:35:05Z
license: mit
score: 9
domains: [backend, web-development]
tags: [rails, ruby, hotwire, fullstack]
curated: 2026-06-15
curated_by: config-scout
---

# Jeffallan/claude-skills — skill

**Why it's worth keeping:** The 'Common Patterns' section provides ground-truth examples to guide code generation, while the 'Constraints' establish critical architectural guardrails like N+1 prevention and service object usage.

**Summary:** A highly structured specialist skill for Rails 7+ development that enforces modern web patterns like Hotwire and Sidekiq.

**Source credibility:** High; a popular repository with significant social proof (9.9k stars) and recent maintenance.

**Recency:** Very current; explicitly targets modern Rails 7+, Turbo, and Hotwire workflows.

**Source:** [Jeffallan/claude-skills/skills/rails-expert/SKILL.md](https://github.com/Jeffallan/claude-skills/blob/e8be415bc94d8d6ebddc2fb50e5d03c6e27d4319/skills/rails-expert/SKILL.md) · 9915★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: rails-expert
description: Rails 7+ specialist that optimizes Active Record queries with includes/eager_load, implements Turbo Frames and Turbo Streams for partial page updates, configures Action Cable for WebSocket connections, sets up Sidekiq workers for background job processing, and writes comprehensive RSpec test suites. Use when building Rails 7+ web applications with Hotwire, real-time features, or background job processing. Invoke for Active Record optimization, Turbo Frames/Streams, Action Cable, Sidekiq, RSpec Rails.
license: MIT
metadata:
  author: https://github.com/Jeffallan
  version: "1.1.0"
  domain: backend
  triggers: Rails, Ruby on Rails, Hotwire, Turbo Frames, Turbo Streams, Action Cable, Active Record, Sidekiq, RSpec Rails
  role: specialist
  scope: implementation
  output-format: code
  related-skills: fullstack-guardian, database-optimizer
---

# Rails Expert

## Core Workflow

1. **Analyze requirements** — Identify models, routes, real-time needs, background jobs
2. **Scaffold resources** — `rails generate model User name:string email:string`, `rails generate controller Users`
3. **Run migrations** — `rails db:migrate` and verify schema with `rails
```

</details>
