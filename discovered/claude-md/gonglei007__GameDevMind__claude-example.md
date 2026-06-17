---
name: gonglei007__GameDevMind__claude-example
source: https://github.com/gonglei007/GameDevMind/blob/bbeb6a959f53df361d6dc97433e88412b0fe2dfd/CLAUDE.md.example
repo: gonglei007/GameDevMind
kind: claude-md
stars: 6351
last_pushed: 2026-05-09T05:12:23Z
license: mit
score: 9
domains: [game-development, engine-architecture]
tags: [unity, unreal, performance, template]
curated: 2026-06-15
curated_by: config-scout
---

# gonglei007/GameDevMind — claude-md

**Why it's worth keeping:** It includes engine-specific 'Common Traps' and quantitative 'Performance Budgets,' providing the guardrails necessary to prevent LLMs from writing high-latency or memory-leaking code.

**Summary:** A comprehensive technical specification and operational template designed specifically for game development environments like Unity or Unreal Engine.

**Source credibility:** High; derived from a widely-recognized game development knowledge base with 6k+ stars.

**Recency:** Current; includes modern engine versions and industry-standard build/deployment workflows.

**Source:** [gonglei007/GameDevMind/CLAUDE.md.example](https://github.com/gonglei007/GameDevMind/blob/bbeb6a959f53df361d6dc97433e88412b0fe2dfd/CLAUDE.md.example) · 6351★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 使用方法：复制此文件到你的游戏项目根目录，重命名为 CLAUDE.md
# 根据你的项目修改标记为 【TODO】 的部分
#
# =============================================================================
# 游戏开发项目 Claude Code 项目记忆
# 【TODO: 项目名称】
# =============================================================================

---

## 项目概述

【TODO: 一句话描述你的游戏项目】

- **游戏类型**：【TODO: FPS / RPG / MOBA / 卡牌 / 休闲 / 开放世界 / ...】
- **引擎**：【TODO: Unity 2022 LTS / Unreal Engine 5.x / 自研引擎】
- **目标平台**：【TODO: PC / iOS+Android / 主机 / 全平台】
- **团队规模**：【TODO: N 人，程序 N 人】
- **网络模式**：【TODO: 单机 / 联机 P2P / 专用服务器 / 混合】

---

## 项目架构

```
【TODO: 简要架构图或描述】

例：
┌─────────────┐    ┌──────────────┐    ┌─────────────┐
│   Client    │◄──►│  Game Server │◄──►│    DB/Redis │
│  (Unity)    │    │   (C++/ASIO) │    └─────────────┘
└─────────────┘    └──────────────┘

客户端分层：
  Presentation (UI) → Gameplay Logic → Engine/Systems → Platform

服务器分层：
  Gateway → Lobby → Game Room → Persistence
```

- **核心设计模式**：【TODO: ECS / MVC / MVP / 组件化 / GameObject-Actor】
- **DI/IoC**：【TODO: Zenject / VContainer / 无】
- **资源管理**：【TODO: Addressables / AssetManager / AssetBundle】
- **UI 框架**：【TODO: UGUI + 自研框架 / UI Toolkit / CommonUI / MVVM】
- **数据配置**：【TODO: ScriptableObject / DataTable / Excel →
```

</details>
