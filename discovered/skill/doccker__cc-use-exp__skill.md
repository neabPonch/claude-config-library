---
name: doccker__cc-use-exp__skill
source: https://github.com/doccker/cc-use-exp/blob/05c0807431d128530cc2e39fa67e2c1cec668f82/.gemini/skills/multi-tenant-safety/SKILL.md
repo: doccker/cc-use-exp
kind: skill
stars: 805
last_pushed: 2026-06-10T07:19:36Z
license: other
score: 9
domains: [backend-api, security, software-architecture]
tags: [multi-tenancy, security-audit, java, spring]
curated: 2026-06-16
curated_by: config-scout
---

# doccker/cc-use-exp — skill

**Why it's worth keeping:** Includes highly effective 'Grep/Audit' signals that allow an agent to detect subtle architectural bypasses (like findById bypassing filters) and provides clear 'Wrong vs. Correct' code patterns.

**Summary:** Provides rigorous security protocols to prevent cross-tenant data leaks in multi-tenant architectures across backend and frontend layers.

**Source credibility:** High; the repository is well-maintained, highly starred, and contains deep, expert-level technical insights.

**Recency:** Very current, addressing modern JPA/Hibernate and Spring security pitfalls.

**Source:** [doccker/cc-use-exp/.gemini/skills/multi-tenant-safety/SKILL.md](https://github.com/doccker/cc-use-exp/blob/05c0807431d128530cc2e39fa67e2c1cec668f82/.gemini/skills/multi-tenant-safety/SKILL.md) · 805★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: multi-tenant-safety
description: >-
  当代码涉及多租户隔离（TenantContext、tenantId、租户拦截器/过滤器、X-Tenant-Code）时触发。
  防止租户越权访问、数据串租户等安全问题。
---
<instructions>

# 多租户隔离安全规范

当系统涉及多租户架构时，防止租户间数据越权访问。

---

## 陷阱 #1: 租户上下文来源信任错误

**场景**: 拦截器/过滤器从请求头（如 `X-Tenant-Code`）设置租户上下文，但未与认证 token 中的 tenantId 做一致性校验

### 问题根因

请求头可以被客户端任意伪造。如果后端只信任请求头中的租户标识，攻击者只需修改 header 就能访问其他租户的数据。

### 错误示例

```java
// ❌ 错误: 只信任请求头，未校验 token
@Override
public boolean preHandle(HttpServletRequest request, ...) {
    String tenantCode = request.getHeader("X-Tenant-Code");
    TenantMiniAppConfig config = configRepository.findByTenantCode(tenantCode);
    TenantContext.setTenantId(config.getTenantId());  // 直接信任 header
    return true;
}
// 攻击者拿着 tenantId=1 的 token，配上 X-Tenant-Code: OTHER_TENANT
// 就能读到其他租户的数据
```

### 正确做法

```java
// ✅ 正确: header 只做路由定位，必须与 token tenantId 校验一致
@Override
public boolean preHandle(HttpServletRequest request, ...) {
    String tenantCode = request.getHeader("X-Tenant-Code");
    TenantMiniAppConfig config = configRepository.findByTenantCode(tenantCode);

    // 从认证 token 中取出 tenantId（真相源）
    Long tokenTenantId = (Long) request.getAttribute("tokenTenantId");
    if (tokenTenantId != nul
```

</details>
