---
name: eze-is__web-access
source: https://github.com/eze-is/web-access/blob/7af34af6a25940d917905f0e5f2a7ef056952971/SKILL.md
repo: eze-is/web-access
kind: skill
stars: 7565
last_pushed: 2026-05-16T05:22:35Z
license: unknown
score: 9
domains: [agents-ai, web-automation, cli-tools]
tags: [CDP, browser-control, agentic-workflows, scraping]
curated: 2026-06-14
curated_by: config-scout
---

# eze-is/web-access — skill

**Why it's worth keeping:** It provides a high-level 'Browsing Philosophy' for goal-oriented decision making and includes advanced strategies like parallel sub-agent task division and media/video frame extraction.

**Summary:** A sophisticated web-browsing protocol that uses a local CDP proxy to allow an agent to interact with the user's actual browser session, including authenticated states and dynamic content.

**Source credibility:** Highly credible with 7.5k+ stars and active maintenance.

**Recency:** Extremely current, requiring Node.js 22+ and reflecting modern web automation needs.

**Source:** [eze-is/web-access/SKILL.md](https://github.com/eze-is/web-access/blob/7af34af6a25940d917905f0e5f2a7ef056952971/SKILL.md) · 7565★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: web-access
license: MIT
github: https://github.com/eze-is/web-access
description:
  所有联网操作必须通过此 skill 处理，包括：搜索、网页抓取、登录后操作、网络交互等。
  触发场景：用户要求搜索信息、查看网页内容、访问需要登录的网站、操作网页界面、抓取社交媒体内容（小红书、微博、推特等）、读取动态渲染页面、以及任何需要真实浏览器环境的网络任务。
metadata:
  author: 一泽Eze
  version: "2.5.3"
---

# web-access Skill

## 前置检查

在开始联网操作前，先检查 CDP 模式可用性：

```bash
node "${CLAUDE_SKILL_DIR}/scripts/check-deps.mjs"
```

**Node.js 22+** 必需（使用原生 WebSocket）。

按脚本输出处理：
- `exit 0` → 继续
- `exit 2` → 需询问用户偏好，写入 `${CLAUDE_SKILL_DIR}/config.env` 的 `WEB_ACCESS_BROWSER`
- `exit 1` → 按 stdout 错误信息处理。若提示包含「Agent 处理顺序」，按其步骤执行（如先用系统命令打开浏览器后重跑），自动可解则不打扰用户；仍失败再向用户求助

支持参数 `--browser <chrome|edge>` 表达本次临时覆盖（不写 config.env）。

切换浏览器时，proxy 是长驻进程，需先 `pkill -f cdp-proxy.mjs` 再重跑 check-deps。

检查通过后并必须在回复中向用户直接展示以下须知，再启动 CDP Proxy 执行操作：

```
温馨提示：部分站点对浏览器自动化操作检测严格，存在账号封禁风险。已内置防护措施但无法完全避免，Agent 继续操作即视为接受。
```

## 浏览哲学

**像人一样思考，兼顾高效与适应性的完成任务。**

执行任务时不会过度依赖固有印象所规划的步骤，而是带着目标进入，边看边判断，遇到阻碍就解决，发现内容不够就深入——全程围绕「我要达成什么」做决策。这个 skill 的所有行为都应遵循这个逻辑。

**① 拿到请求** — 先明确用户要做什么，定义成功标准：什么算完成了？需要获取什么信息、执行什么操作、达到什么结果？这是后续所有判断的锚点。

**② 选择起点** — 根据任务性质、平台特征、达成条件，选一个最可能直达的方式作为第一步去验证。一次成功当然最好；不成功则在③中调整。比如，需要操作页面、需要登录态、已知静态方式不可达的平台（小红书、微信公众号等）→ 直接 CDP

**③
```

</details>
