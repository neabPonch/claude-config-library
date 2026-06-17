---
name: gys-dev__ansible-public-playbooks__deploy-website-skill
source: https://github.com/gys-dev/ansible-public-playbooks/blob/1f7f3a48aac51909bd87dcc447daf7ff60e965e4/skills/base/deploy-website-skill.md
repo: gys-dev/ansible-public-playbooks
kind: skill
stars: 5
last_pushed: 2026-02-24T04:15:23Z
license: unknown
score: 8
domains: [devops, web-deployment, security]
tags: [nginx, nodejs, deployment, production]
curated: 2026-06-16
curated_by: config-scout
---

# gys-dev/ansible-public-playbooks — skill

**Why it's worth keeping:** Includes ready-to-use, production-hardened configuration snippets for Nginx reverse proxies, PM2 process management, and system security via UFW.

**Summary:** A highly detailed deployment blueprint that provides a step-by-step technical runbook for setting up production web environments.

**Source credibility:** High-quality DevOps content sourced from a public Ansible repository.

**Recency:** 

**Source:** [gys-dev/ansible-public-playbooks/skills/base/deploy-website-skill.md](https://github.com/gys-dev/ansible-public-playbooks/blob/1f7f3a48aac51909bd87dcc447daf7ff60e965e4/skills/base/deploy-website-skill.md) · 5★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Deploy Website Skill

A comprehensive skill for deploying full production websites with automated environment setup, dependency management, and production serving.

## Usage
```bash
# Deploy a production website
/claude deploy-website --source /path/to/project --domain example.com --ssl

# Deploy with custom configuration
/claude deploy-website --source /path/to/project --domain example.com --ssl --pm2 --nginx --database
```

## Parameters

### Required
- `--source`: Path to the project source code
- `--domain`: Domain name for the production website

### Optional
- `--ssl`: Enable SSL/TLS certificates (Let's Encrypt)
- `--pm2`: Use PM2 for process management (Node.js applications)
- `--nginx`: Configure Nginx as reverse proxy
- `--database`: Set up database (MySQL/PostgreSQL)
- `--env`: Environment variables file (default: .env)
- `--branch`: Git branch to deploy (default: main)
- `--user`: Deployment user (default: deploy)

## Features

### Environment Setup
- Creates dedicated deployment user
- Configures SSH keys and permissions
- Sets up firewall (UFW) rules
- Installs system dependencies

### Dependency Management
- Node.js/NPM dependencies installation
- Python requirement
```

</details>
