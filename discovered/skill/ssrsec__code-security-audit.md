---
name: ssrsec__code-security-audit
source: https://github.com/ssrsec/code-security-audit/blob/e867a05874bd1df609342c023ef0aa8dbb64b22b/SKILL.md
repo: ssrsec/code-security-audit
kind: skill
stars: 29
last_pushed: 2026-05-28T08:38:20Z
license: unknown
score: 8
domains: [security, agents-ai, devsecops]
tags: [security-audit, workflow-automation, quality-assurance]
curated: 2026-06-16
curated_by: config-scout
---

# ssrsec/code-security-audit — skill

**Why it's worth keeping:** It uses a formal 'candidate -> validated -> confirmed' lifecycle and mandates structured data (JSON/SQLite) as the source of truth to prevent hallucination. The inclusion of mandatory 'Quality Gates' ensures high-integrity report generation.

**Summary:** A rigorous, state-driven protocol for automated security auditing that moves through reconnaissance, validation, and quality gates.

**Source credibility:** Small, specialized repo with recent activity; likely developed by security professionals.

**Recency:** Highly current; explicitly designed for Claude Code and modern AI IDEs.

**Source:** [ssrsec/code-security-audit/SKILL.md](https://github.com/ssrsec/code-security-audit/blob/e867a05874bd1df609342c023ef0aa8dbb64b22b/SKILL.md) · 29★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: code-security-audit
description: AI 驱动的生产级代码安全审计协议。面向企业内部授权审计，默认使用结构化 harness：项目画像、攻击面枚举、Sink/Control 双轨候选发现、验证队列、能力链、质量门、报告渲染和完整证据交付。支持 PHP、Java、C# / ASP.NET、Go、Python、JavaScript / TypeScript Node.js、Ruby、Rust、Kotlin、Deno/Bun，以及 JVM/.NET 编译产物反编译计划。用户说「开始审计 / 对 XXX 做安全审计 / 代码审计 / 安全扫描 / 找漏洞 / security audit / 红队审计」时触发。
---

# 代码安全审计生产协议

本入口默认执行代码安全审计生产协议。

## 授权与安全边界

本 skill 仅用于企业内部授权的防御性代码安全审计。审计目标、靶场地址、凭据和验证动作必须属于授权范围。

- L1：只读分析和只读请求，默认允许。
- L2：可回滚写操作，授权靶场内默认允许自动执行，必须记录 baseline、proof、cleanup 和 post-cleanup assert。
- L3：不可逆、高破坏或高影响动作，极少使用；只有这类动作才需要逐次明确说明风险并获得当次授权。
- 内部权威报告不脱敏。保留复现所需的 Cookie、Token、路径、payload、响应摘要和业务标识。

## 默认输出

所有新审计默认写入：

```text
audit-v2/
```

Markdown 不是权威状态。权威状态是 SQLite + 结构化 JSON/JSONL，最终报告只由结构化数据渲染生成。

## 支持栈

生产准入覆盖以下常用审计目标：

- PHP。
- Java / Kotlin / JVM 编译产物。
- C# / ASP.NET / .NET 编译产物。
- Go。
- Python。
- JavaScript / TypeScript Node.js。
- TypeScript Deno / Bun。
- Ruby。
- Rust。

JVM 和 .NET 反编译执行链路已接入，但真实执行必须显式传 `--execute`。Android/native 当前只生成明确的反编译计划和 blocker，不假装已支持。

## 生产流程

AI 接到审计请求后必须自动完成环境准备、流水线执行、质量门和报告渲染。工程师只需要提供初始目标信息，以及复杂登录、环境异常、跨平台工具、L3 授权或上下文续跑这类必要交互。

执行审计时按以下生产闭环推进：

1. `recon`：识别语言、框架、入口、source、sink、敏感资产和编译产物。
2. `audit`：生成结构化
```

</details>
