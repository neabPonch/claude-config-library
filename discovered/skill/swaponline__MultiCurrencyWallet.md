---
name: swaponline__MultiCurrencyWallet
source: https://github.com/swaponline/MultiCurrencyWallet/blob/9eae354d059198911e490bc7cd6849a2bd51fb1b/SKILL.md
repo: swaponline/MultiCurrencyWallet
kind: skill
stars: 540
last_pushed: 2026-05-27T00:48:46Z
license: mit
score: 9
domains: [blockchain, web-frontend, devops]
tags: [crypto-wallet, configuration-guide, deployment-workflows]
curated: 2026-06-14
curated_by: config-scout
---

# swaponline/MultiCurrencyWallet — skill

**Why it's worth keeping:** The document contains specific 'how-to' sequences for extending core features (like EVM chains) and maps high-level architecture to specific file paths, which is critical for agentic task execution.

**Summary:** A high-density technical manual detailing the configuration, extension, and deployment of a multi-chain crypto wallet. It provides clear procedural recipes for adding new blockchain networks or dApps to the system.

**Source credibility:** High; active open-source project with significant community interest (540 stars).

**Recency:** Very current, utilizing modern web3 stacks like Wagmi v2 and Viem.

**Source:** [swaponline/MultiCurrencyWallet/SKILL.md](https://github.com/swaponline/MultiCurrencyWallet/blob/9eae354d059198911e490bc7cd6849a2bd51fb1b/SKILL.md) · 540★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# SKILL.md — MCW Setup & Operations Guide

Полное руководство по локальной разработке, конфигурации и деплою MultiCurrencyWallet.

---

## Quick Start (Local Dev)

```bash
# 1. Установить зависимости
npm install

# 2. Запустить dev-сервер (testnet, localhost:9001)
npm run dev

# 3. Открыть браузер
open http://localhost:9001
```

Dev-сервер использует **testnet** конфиг. MetaMask нужно переключить на Sepolia/BSC Testnet.

---

## Config System

Конфиги выбираются через `CONFIG` env variable при сборке.

```
src/front/config/
├── mainnet/          # Production config
│   ├── evmNetworks.js  — chainId, networkVersion, chainName для каждой EVM-сети
│   ├── web3.js         — RPC endpoint URLs
│   ├── api.js          — Explorer API keys, WalletConnect Project ID, Infura key
│   └── link.js         — Block explorer URLs для отображения
└── testnet/          # Testnet config (same structure)
```

**Добавить новую EVM chain:**
1. `mainnet/web3.js` — добавь `newchain_provider: 'https://rpc.newchain.io'`
2. `mainnet/evmNetworks.js` — добавь объект с `currency, chainId, networkVersion, chainName, rpcUrls, blockExplorerUrls`
3. `mainnet/link.js` — добавь explorer URL
4. `mainnet/api.js` — добав
```

</details>
