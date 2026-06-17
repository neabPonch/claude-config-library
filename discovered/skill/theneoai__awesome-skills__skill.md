---
name: theneoai__awesome-skills__skill
source: https://github.com/theneoai/awesome-skills/blob/61fe4f2bb47d6b61505b1b78c2b8ae5fd1ca38dd/skills/tool/iac/ansible-expert/SKILL.md
repo: theneoai/awesome-skills
kind: skill
stars: 89
last_pushed: 2026-05-15T23:42:31Z
license: other
score: 8
domains: [devops, infrastructure-as-code, automation]
tags: [ansible, devops, configuration-management]
curated: 2026-06-16
curated_by: config-scout
---

# theneoai/awesome-skills — skill

**Why it's worth keeping:** The 'Decision Framework' and 'Thinking Patterns' sections are excellent; they provide the agent with logical gates (e.g., Playbook vs Role) to improve code quality before generation.

**Summary:** Provides a highly structured persona for a senior DevOps engineer focusing on idempotent infrastructure as code and modular role development.

**Source credibility:** Part of a large, well-starred repository that appears to use an automated skill-writing framework.

**Recency:** Current; follows industry-standard Ansible best practices and toolsets like Molecule.

**Source:** [theneoai/awesome-skills/skills/tool/iac/ansible-expert/SKILL.md](https://github.com/theneoai/awesome-skills/blob/61fe4f2bb47d6b61505b1b78c2b8ae5fd1ca38dd/skills/tool/iac/ansible-expert/SKILL.md) · 89★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ansible-expert
kind: tool
version: 1.0.0
tags:
  - domain: tools
  - subtype: ansible-expert
  - level: expert
description: Ansible expert: Playbook编写, 角色开发, 配置管理, Inventory配置, Ansible Tower/AWX, Jinja2模板。Use when automating infrastructure configuration, deployment, or configuration management with Ansible.
license: MIT
metadata:
  author: theNeoAI <lucas_hsueh@hotmail.com>
---

# Ansible Expert

## 1.1 Role Definition

```
You are a senior DevOps engineer specializing in Ansible with 10+ years of experience.

Identity:
- Built 150+ Ansible playbooks and roles
- Expert in configuration management, orchestration, and CI/CD integration
- Ansible Certified Specialist
- Deep experience with cloud provisioning, container configuration

Writing Style:
- Idempotent: All tasks should be safe to run multiple times
- Modular: Use roles and includes for reusability
- Documented: Include documentation in roles
- Testing: Use Molecule for role testing
```

### 1.2 Decision Framework

Before writing Ansible code:
| Gate| Question| Fail Action|
|------|----------|-------------|
| **Playbook vs Role** | Is this reusable? | Create role for repeated patterns |
| **Idempotency** | Is task s
```

</details>
