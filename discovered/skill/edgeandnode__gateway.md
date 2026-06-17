---
name: edgeandnode__gateway
source: https://github.com/edgeandnode/gateway/blob/4d78b65e93c0b12156cd7cb98a6e3a461f0ade34/SKILL.md
repo: edgeandnode/gateway
kind: skill
stars: 11
last_pushed: 2026-06-12T18:26:30Z
license: mit
score: 7
domains: [blockchain, agents-ai, cli-tools, data-access]
tags: [the-graph, x402, web3, subgraphs]
curated: 2026-06-14
curated_by: config-scout
---

# edgeandnode/gateway — skill

**Why it's worth keeping:** It provides concrete CLI commands and environment variable schemas that allow an agent to execute authenticated queries without manual API key handling.

**Summary:** Technical documentation for interacting with The Graph Gateway, specifically highlighting the x402 protocol designed for autonomous agent payments.

**Source credibility:** Niche project (11 stars) but demonstrates high-quality, professional documentation patterns.

**Recency:** Highly current; recently updated and uses modern web3/agentic payment standards.

**Source:** [edgeandnode/gateway/SKILL.md](https://github.com/edgeandnode/gateway/blob/4d78b65e93c0b12156cd7cb98a6e3a461f0ade34/SKILL.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# The Graph Gateway

Query blockchain data from The Graph Network's decentralized indexers.

## Environments

| Environment | Base URL | x402 Payment Network |
|-------------|----------|---------------------|
| Mainnet | `https://gateway.thegraph.com` | Base |
| Testnet | `https://testnet.gateway.thegraph.com` | Base Sepolia |

## Authentication

Two options for accessing the API:

### Option 1: API Key (best for humans)

Get an API key from [Subgraph Studio](https://thegraph.com/studio) and include it in requests.

**Endpoints:**
- `POST /api/subgraphs/id/{subgraph_id}`
- `POST /api/deployments/id/{deployment_id}`

**Header:** `Authorization: Bearer <API_KEY>`

### Option 2: x402 Payment (best for agents)

Pay per query with USDC on Base. No API key required. The x402 protocol handles payment negotiation automatically.

**Endpoints:**
- `POST /api/x402/subgraphs/id/{subgraph_id}`
- `POST /api/x402/deployments/id/{deployment_id}`

## Examples

### With API Key

```bash
curl -X POST https://gateway.thegraph.com/api/subgraphs/id/5zvR82QoaXYFyDEKLZ9t6v9adgnptxYpKpSbxtgVENFV \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{"query": "{ tokens(
```

</details>
