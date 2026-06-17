---
name: eeeeeeeeee-code__e0e1-wx
source: https://github.com/eeeeeeeeee-code/e0e1-wx/blob/1f8dded6a3e8c3c76806fb504999dc45ed61eac0/SKILL.md
repo: eeeeeeeeee-code/e0e1-wx
kind: skill
stars: 2063
last_pushed: 2026-05-26T09:56:51Z
license: unknown
score: 9
domains: [security, pentesting, automation]
tags: [wechat-miniapp, red-teaming, runtime-analysis]
curated: 2026-06-14
curated_by: config-scout
---

# eeeeeeeeee-code/e0e1-wx — skill

**Why it's worth keeping:** It features highly specific domain intelligence, such as the 'Detail routing protocol' for IDOR testing and precise instructions for injecting scripts into page-frame contexts to bypass context limitations.

**Summary:** An advanced automation skill for WeChat Mini-Program security auditing that utilizes CDP-based runtime injection and priority-driven vulnerability scanning.

**Source credibility:** High popularity indicated by 2k+ stars; represents a specialized security research toolset.

**Recency:** Highly current, reflecting modern WeChat debugging and runtime inspection techniques.

**Source:** [eeeeeeeeee-code/e0e1-wx/SKILL.md](https://github.com/eeeeeeeeee-code/e0e1-wx/blob/1f8dded6a3e8c3c76806fb504999dc45ed61eac0/SKILL.md) · 2063★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: miniapp-security-core
description: Use when reviewing authorized WeChat mini-program or mini-app targets for authentication bypass, IDOR, undefined-path access, API abuse, decryption and signature analysis, runtime reverse engineering, route mapping, and sensitive data exposure, with file-submission attack surfaces intentionally excluded.
---

## ❌ 红线（违反即失败）

1. **未完整复述 Checklist** 就调用 MCP 工具
2. **自动重放支付、退款、提现、下单等资金类接口**（`build_replay_plan` 只生成计划，不自动发送）
3. **未经 `dryRun=false` 和 `requireConfirm=true` 就修改 Vuex state**
4. **把解密结果用于绕过服务端校验而非安全评估**

---

## ⚠️ 授权声明（必读）

> **本 skill 仅用于已获授权的安全评估、CTF 竞赛、合法渗透测试和防御性安全研究。**
> **目标小程序须为授权评估对象。禁止对未授权系统使用任何主动探测手段。使用者须自行承担法律责任。**

---

## 评估流程总览

| Phase | 目标 | 核心工具 | 输出 |
|-------|------|---------|------|
| 0. 环境搭建 | CDP 连接 + Hook 注入 | `connection_ops` / `network_ops` | 流量采集就绪 |
| 1. 侦察 | 路由 + 接口资产盘点 | `runtime_ops` / `debugger_ops` | 接口清单（含路由标注）|
| 2. 渗透线索 | IDOR / 认证绕过 / 资金接口 | `analysis_ops` / `runtime_ops(fetch)` | 风险候选清单 |
| 3. 解密分析 | 加密参数破解 + 密钥追踪 | `decrypt_ops` / `debugger_ops` | 明文数据 |
| 4. 逆向审计 | 代码保护分析 + 硬编码凭据扫描 | `debugger_ops` / `reverse_ops` | 凭据泄露报告 |
| 5. State 检查 | Vuex 越权状态验证 | `runtime_ops` | 越权路径 |
| 6. 报告导出 | Mark
```

</details>
