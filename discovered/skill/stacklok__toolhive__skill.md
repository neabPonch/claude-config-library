---
name: stacklok__toolhive__skill
source: https://github.com/stacklok/toolhive/blob/3ebb76bea4d158917d222fe07b910447bc659b95/.claude/skills/deploy-otel/SKILL.md
repo: stacklok/toolhive
kind: skill
stars: 1883
last_pushed: 2026-06-16T16:38:31Z
license: apache-2.0
score: 8
domains: [devops, infrastructure, observability]
tags: [kubernetes, otel, kind, helm]
curated: 2026-06-16
curated_by: config-scout
---

# stacklok/toolhive — skill

**Why it's worth keeping:** Employs rigorous prerequisite validation and provides explicit post-deployment access instructions via port-forwarding commands.

**Summary:** Deploys a complete OpenTelemetry observability stack (Prometheus, Grafana, Tempo) to a Kind Kubernetes cluster.

**Source credibility:** High; source repo is highly starred and actively maintained.

**Recency:** Current; uses modern standards for local Kubernetes development and observability stacks.

**Source:** [stacklok/toolhive/.claude/skills/deploy-otel/SKILL.md](https://github.com/stacklok/toolhive/blob/3ebb76bea4d158917d222fe07b910447bc659b95/.claude/skills/deploy-otel/SKILL.md) · 1883★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: deploy-otel
description: Deploy the OpenTelemetry observability stack (Prometheus, Grafana, OTEL Collector) to a Kind cluster for testing toolhive telemetry. Use when you need to set up monitoring, metrics collection, or observability infrastructure.
allowed-tools: Bash, Read
---

# Deploy OTEL Observability Stack

Deploy a complete OpenTelemetry observability stack to a Kind cluster for testing ToolHives telemetry capabilities.

## Steps

### 1. Verify Prerequisites

Check that required tools are installed:

```bash
echo "Checking prerequisites..."
command -v kind >/dev/null 2>&1 || { echo "ERROR: kind is not installed"; exit 1; }
command -v helm >/dev/null 2>&1 || { echo "ERROR: helm is not installed"; exit 1; }
command -v kubectl >/dev/null 2>&1 || { echo "ERROR: kubectl is not installed"; exit 1; }
echo "All prerequisites met."
```

### 2. Create Kind Cluster

Create the Kind cluster if it doesn't exist:

```bash
CLUSTER_NAME="toolhive"

if kind get clusters 2>/dev/null | grep -q "^${CLUSTER_NAME}$"; then
  echo "Kind cluster '${CLUSTER_NAME}' already exists"
else
  echo "Creating Kind cluster '${CLUSTER_NAME}'..."
  kind create cluster --name ${CLUSTER_NAME}
fi

# Ex
```

</details>
