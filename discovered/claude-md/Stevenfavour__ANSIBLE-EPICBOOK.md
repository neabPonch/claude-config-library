---
name: Stevenfavour__ANSIBLE-EPICBOOK
source: https://github.com/Stevenfavour/ANSIBLE-EPICBOOK/blob/3fe5e8a65658816600a1374638e3390cf6f85666/Claude.md
repo: Stevenfavour/ANSIBLE-EPICBOOK
kind: claude-md
stars: 0
last_pushed: 2026-04-22T00:06:21Z
license: unknown
score: 8
domains: [infrastructure-as-code, devops, automation]
tags: [monorepo, terraform, ansible, multi-cloud]
curated: 2026-06-15
curated_by: config-scout
---

# Stevenfavour/ANSIBLE-EPICBOOK — claude-md

**Why it's worth keeping:** The 'Known Issues' section is excellent for preventing the AI from suggesting broken patterns; providing explicit CLI workflows ensures tool consistency.

**Summary:** Acts as a comprehensive project map that bridges high-level architecture with specific sub-directory instructions.

**Source credibility:** Low social proof (0 stars), but content shows high technical density consistent with actual DevOps work.

**Recency:** Highly current,-updated 2 months ago and utilizes modern multi-layered documentation strategies.

**Source:** [Stevenfavour/ANSIBLE-EPICBOOK/Claude.md](https://github.com/Stevenfavour/ANSIBLE-EPICBOOK/blob/3fe5e8a65658816600a1374638e3390cf6f85666/Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude.md – Repository Overview

## 📁 Repository Layout
```
Ansible-EpicBook/
├─ Terraform/                 # AWS infrastructure (Terraform) + Azure lab (Terraform)
│   ├─ main.tf               # Core AWS resources (VPC, subnets, SG, EC2, RDS)
│   ├─ variables.tf          # Variables for AWS resources
│   ├─ outputs.tf            # Exported outputs
│   ├─ sectret.auto.tfvars   # Auto‑generated secrets (do NOT commit)
│   ├─ terraform.tfvars      # User‑provided variable values
│   ├─ .terraform/           # Provider plugins (auto‑generated)
│   ├─ .ssh/                 # SSH key pair used by Terraform
│   ├─ CLAUDE.md             # Guidance for Claude when working in this folder
│   └─ theepicbook/          # Embedded Git repo with additional docs
│
├─ ansible-lab/              # Azure resources provisioned via Terraform
│   ├─ main.tf               # Azure RG, VNet, Subnet, NIC, VM, NSG
│   ├─ variables.tf          # Azure variable definitions
│   └─ outputs.tf            # Exported Azure outputs
│
├─ static-web/                # Ansible playbooks & roles for the web tier
│   ├─ ansible.cfg          # Minimal SSH config for Ansible
│   ├─ inventory.ini        # Host inventory us
```

</details>
