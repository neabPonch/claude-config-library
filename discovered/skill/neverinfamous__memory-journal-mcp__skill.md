---
name: neverinfamous__memory-journal-mcp__skill
source: https://github.com/neverinfamous/memory-journal-mcp/blob/6acf6e9a73b1aa3375484775ddd08a94c3ef5069/skills/azure/SKILL.md
repo: neverinfamous/memory-journal-mcp
kind: skill
stars: 18
last_pushed: 2026-06-12T23:48:35Z
license: mit
score: 7
domains: [cloud-infrastructure, devops, security]
tags: [azure, cloud-computing, best-practices]
curated: 2026-06-15
curated_by: config-scout
---

# neverinfamous/memory-journal-mcp — skill

**Why it's worth keeping:** Uses 'STOP' instructions to force retrieval-first behavior; provides high-leverage pattern preferences like Managed Identities and Bicep over ARM templates.

**Summary:** Provides architectural guardrails and security best practices for Microsoft Azure deployments.

**Source credibility:** Niche repository with specialized, well-structured content despite low star count.

**Recency:** Current; uses modern terminology like Azure Entra ID and prefers Bicep.

**Source:** [neverinfamous/memory-journal-mcp/skills/azure/SKILL.md](https://github.com/neverinfamous/memory-journal-mcp/blob/6acf6e9a73b1aa3375484775ddd08a94c3ef5069/skills/azure/SKILL.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: azure
description: |
  Microsoft Azure best practices. Use when deploying to Azure App Service, Azure Functions, AKS (Azure Kubernetes Service), Cosmos DB, configuring Azure Entra ID (Active Directory), or managing Azure Resource Manager (ARM/Bicep) templates. Do NOT trigger for generic "deploy my app" requests without clarifying the target platform.
---

# Microsoft Azure Best Practices

**STOP.** Your knowledge of Azure may be outdated. Prefer retrieval over pre-training for any version-sensitive Azure configuration. Fetch current documentation when in doubt.

Standards for deploying and managing workloads securely on Microsoft Azure.

## 1. Identity & Access (Azure Entra ID / Active Directory)

- **Managed Identities**: Use System-Assigned or User-Assigned Managed Identities for Azure resources (VMs, App Services, Functions) to authenticate to other Azure services (Key Vault, SQL, Storage) without managing credentials.
- **RBAC**: Use Azure Role-Based Access Control. Assign roles to Entra ID Groups rather than individual users to simplify lifecycle management.
- **Key Vault**: Never store secrets in application configuration files. Store them in Azure Key Vault and ref
```

</details>
