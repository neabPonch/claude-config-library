---
name: shakenfist__kerbside-patches__claude
source: https://github.com/shakenfist/kerbside-patches/blob/baf3aea4ffebedbe06cee4e6181839a93eaa45cf/kolla-ansible/_CLAUDE.md
repo: shakenfist/kerbside-patches
kind: claude-md
stars: 1
last_pushed: 2026-06-14T20:08:59Z
license: apache-2.0
score: 9
domains: [devops, infrastructure-as-code, cloud-computing, ansible, python]
tags: [openstack, ansible, deployment, automation]
curated: 2026-06-15
curated_by: config-scout
---

# shakenfist/kerbside-patches — claude-md

**Why it's worth keeping:** Uses hierarchical breakdowns of component categories and explicit 'How-To' workflows that instruct the AI on exact patterns for expansion and modification.

**Summary:** Provides deep architectural context and technical standards for a complex OpenStack deployment tool involving Python and Ansible.

**Source credibility:** Highly credible; based on an active, industry-standard OpenStack infrastructure project.

**Recency:** Very current; perfectly optimized for agentic tools like Claude Code that require structural/pattern guidance.

**Source:** [shakenfist/kerbside-patches/kolla-ansible/_CLAUDE.md](https://github.com/shakenfist/kerbside-patches/blob/baf3aea4ffebedbe06cee4e6181839a93eaa45cf/kolla-ansible/_CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Kolla Ansible - OpenStack Deployment Automation

This document provides context and guidelines for working with the Kolla
Ansible codebase, which is an OpenStack Foundation project for deploying
OpenStack clouds using containerized services orchestrated by Ansible.

## Project Overview

Kolla Ansible provides production-ready containers and deployment tools for
operating OpenStack clouds. It deploys OpenStack services and infrastructure
components in Docker/Podman containers using Ansible orchestration.

**Mission:** Enable operators (both inexperienced and experienced) to deploy
and manage OpenStack clouds quickly while allowing extensive customization.

## Architecture

### Directory Structure

- `ansible/` - Core Ansible playbooks, roles, and plugins
  - `site.yml` - Main orchestration playbook (1034 lines)
  - `roles/` - 80+ Ansible roles for OpenStack services and infrastructure
  - `group_vars/all/` - 60+ service-specific configuration files
  - `action_plugins/` - Config merge plugins
  - `filter_plugins/` - Custom Jinja2 filters
  - `library/` - Custom Ansible modules (kolla_container, etc.)
  - `module_utils/` - Container worker abstractions
- `kolla_ansible/` - Python p
```

</details>
