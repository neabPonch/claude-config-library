---
name: HToTH__DeFiHackLabs-skill__logic-flaw-skill
source: https://github.com/HToTH/DeFiHackLabs-skill/blob/b7cb0764f388405c05954bd3e9652559f5a9849d/sub-skills/logic-flaw-skill.md
repo: HToTH/DeFiHackLabs-skill
kind: skill
stars: 11
last_pushed: 2026-01-30T02:21:04Z
license: unknown
score: 9
domains: [security, blockchain, smart-contracts]
tags: [defi, vulnerability-analysis, solidity, security-audit]
curated: 2026-06-16
curated_by: config-scout
---

# HToTH/DeFiHackLabs-skill — skill

**Why it's worth keeping:** The 'Vulnerable Code vs. Fixed Code' structure provides perfect training examples for an agent to identify bugs, while the inclusion of a Foundry PoC template makes it immediately actionable.

**Summary:** A highly specialized security auditing skill focusing on DeFi logic flaw patterns, specific attack vectors, and their mitigations.

**Source credibility:** Moderate; appears to be a niche security research repository with high-quality technical content.

**Recency:** Very current; includes 2024 case studies and up-to-date solidity patterns.

**Source:** [HToTH/DeFiHackLabs-skill/sub-skills/logic-flaw-skill.md](https://github.com/HToTH/DeFiHackLabs-skill/blob/b7cb0764f388405c05954bd3e9652559f5a9849d/sub-skills/logic-flaw-skill.md) · 11★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: logic-flaw-vulnerability
description: Logic flaw vulnerability analysis covering 39 real cases with $109M total loss. Use when analyzing LP share calculation errors, reward distribution bugs, emergency withdrawal flaws, or collateral valuation errors. Includes attack patterns for share manipulation, reward exploitation, and PoC templates for logic flaw attacks.
---

# Logic Flaw 漏洞分析

## 快速识别

### 核心特征
- ✓ LP 份额计算使用 `balanceOf()` 而非 `reserves`
- ✓ 奖励/费用领取缺少已领取记录
- ✓ 紧急提款不更新内部账户
- ✓ 抵押品估值使用可操纵的价格源
- ✓ 状态更新不一致或缺失

### 快速检查清单 (5 分钟)
- [ ] 检查 LP 份额计算是否使用 `balanceOf()`
- [ ] 验证奖励领取是否记录已领取状态
- [ ] 检查紧急提款是否更新所有相关状态
- [ ] 确认价格源是否可被操纵
- [ ] 验证状态更新的一致性

### 本质公式
```
逻辑缺陷 = 错误的核心算法 × 可重复利用 × 高价值目标
```

## 漏洞分类

### 主要类型

**A. LP Share Calculation Flaw (份额计算缺陷)** - 2.6%
- 使用 `balanceOf()` 而非 `reserves` 计算份额
- 典型案例: Spartan ($30.5M)

**B. Repeated Reward Claim (重复奖励领取)** - 2.6%
- 费用/奖励领取缺少已领取记录
- 典型案例: Popsicle ($20M)

**C. Emergency Withdraw Exploit (紧急提款漏洞)** - 2.6%
- 紧急提款不更新内部账户
- 典型案例: bEarn ($11M)

**D. Collateral Valuation Error (抵押品估值错误)** - 多个子类型
- 价格操纵、清算逻辑缺陷等
- 典型案例: HedgeyFinance ($48M)


## 核心攻击模式

### 模式 1: LP 份额操纵

```solidity
// ❌ 漏洞代码
function calcLiquidityShare(uint25
```

</details>
