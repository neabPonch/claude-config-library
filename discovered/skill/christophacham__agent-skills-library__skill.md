---
name: christophacham__agent-skills-library__skill
source: https://github.com/christophacham/agent-skills-library/blob/8dd0b12e7dbd3a3cf9d971610fedbcd261128457/skills/backend-dev/azure-mgmt-apimanagement-dotnet/SKILL.md
repo: christophacham/agent-skills-library
kind: skill
stars: 57
last_pushed: 2026-03-03T14:59:53Z
license: mit
score: 9
domains: [cloud-infrastructure, backend-api, devops]
tags: [azure, dotnet, apim, iac]
curated: 2026-06-15
curated_by: config-scout
---

# christophacham/agent-skills-library — skill

**Why it's worth keeping:** The file includes highly actionable 'Core Workflows' that chain multiple resources together, alongside a clear object hierarchy that allows an agent to navigate complex cloud structures.

**Summary:** Provides a complete technical blueprint for managing Azure API Management via the .NET SDK, covering resource hierarchies and end-to-end workflows.

**Source credibility:** High; demonstrates deep domain expertise with structured, professional-grade documentation patterns.

**Recency:** Highly current, including recent SDK versions and up-to-date best practices.

**Source:** [christophacham/agent-skills-library/skills/backend-dev/azure-mgmt-apimanagement-dotnet/SKILL.md](https://github.com/christophacham/agent-skills-library/blob/8dd0b12e7dbd3a3cf9d971610fedbcd261128457/skills/backend-dev/azure-mgmt-apimanagement-dotnet/SKILL.md) · 57★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: azure-mgmt-apimanagement-dotnet
description: Azure Resource Manager SDK for API Management in .NET.
risk: unknown
source: community
date_added: '2026-02-27'
---

# Azure.ResourceManager.ApiManagement (.NET)

Management plane SDK for provisioning and managing Azure API Management resources via Azure Resource Manager.

> **⚠️ Management vs Data Plane**
> - **This SDK (Azure.ResourceManager.ApiManagement)**: Create services, APIs, products, subscriptions, policies, users, groups
> - **Data Plane**: Direct API calls to your APIM gateway endpoints

## Installation

```bash
dotnet add package Azure.ResourceManager.ApiManagement
dotnet add package Azure.Identity
```

**Current Version**: v1.3.0

## Environment Variables

```bash
AZURE_SUBSCRIPTION_ID=<your-subscription-id>
# For service principal auth (optional)
AZURE_TENANT_ID=<tenant-id>
AZURE_CLIENT_ID=<client-id>
AZURE_CLIENT_SECRET=<client-secret>
```

## Authentication

```csharp
using Azure.Identity;
using Azure.ResourceManager;
using Azure.ResourceManager.ApiManagement;

// Always use DefaultAzureCredential
var credential = new DefaultAzureCredential();
var armClient = new ArmClient(credential);

// Get subscription
var
```

</details>
