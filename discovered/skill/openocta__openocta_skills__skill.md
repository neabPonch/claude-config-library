---
name: openocta__openocta_skills__skill
source: https://github.com/openocta/openocta_skills/blob/901881964772ec3df5fe7c0589e0252ec13fa953/%E7%AD%89%E4%BF%9D%E6%B5%8B%E8%AF%84skill/skill.md
repo: openocta/openocta_skills
kind: skill
stars: 119
last_pushed: 2026-06-12T09:38:07Z
license: mit
score: 9
domains: [security, compliance, cli-tools]
tags: [mlps-2.0, audit, pentesting]
curated: 2026-06-15
curated_by: config-scout
---

# openocta/openocta_skills — skill

**Why it's worth keeping:** It provides a professional 'Interview -> Verify -> Test' workflow and includes granular, battle-tested shell command sequences for asset discovery and system hardening audits.

**Summary:** A highly structured, phase-based playbook for conducting MLPS 2.0 (China compliance) security assessments using Kali Linux tools.

**Source credibility:** High; specialized repository with significant community traction and structured technical depth.

**Recency:** Current; utilizes modern security toolchains like masscan, ffuf, and nmap.

**Source:** [openocta/openocta_skills/等保测评skill/skill.md](https://github.com/openocta/openocta_skills/blob/901881964772ec3df5fe7c0589e0252ec13fa953/%E7%AD%89%E4%BF%9D%E6%B5%8B%E8%AF%84skill/skill.md) · 119★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "djbh-assessment"
description: "Invoke for 等保2.0 full-lifecycle assessment on corporate networks on Kali Linux: classification, gap analysis, baseline audit, vuln scanning, penetration testing, and compliance reporting per GB/T 22239-2019."
---

# 网络安全等级保护测评技能（等保2.0）

本技能在Kali Linux环境中执行等保2.0（GB/T 22239-2019）全流程测评，覆盖安全通用要求与云计算/工控/物联网/大数据/移动互联扩展要求。

## 等保级别速查

| 等级 | 名称 | 典型对象 | 测评周期 |
|------|------|----------|----------|
| 第一级 | 自主保护级 | 小型企业内网 | 不定级 |
| 第二级 | 指导保护级 | 一般企业门户/邮件 | 每两年一次 |
| 第三级 | 监督保护级 | 政务/金融/运营商 | 每年一次 |
| 第四级 | 强制保护级 | 国家重要信息系统 | 每半年一次 |
| 第五级 | 专控保护级 | 国家核心机密系统 | 视情况而定 |

> 本技能以**第二级和第三级**为主，这也是企业最常见的等保测评级别。

## 等保2.0安全域全景图

```
┌──────────────────────────────────────────────────────────────┐
│                         安全管理要求                           │
│  安全管理制度 │ 安全管理机构 │ 安全管理人员 │ 建设管理 │ 运维管理 │
├──────────────────────────────────────────────────────────────┤
│                         安全技术要求                           │
│  物理环境 → 通信网络 → 区域边界 → 计算环境 → 管理中心          │
├──────────────────────────────────────────────────────────────┤
│                     等保2.0扩展要求（按需）                     │
│  云计算安全 │ 移动互联安全 │ 物联网安全 │ 工控安全 │ 大数据安全  │
└──────────────────────
```

</details>
