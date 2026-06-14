---
name: myysophia__codex-config__readme-skill
source: https://github.com/myysophia/codex-config/blob/9e3619cef80a3d83268fd9c075648617705ea37b/readme_skill.md
repo: myysophia/codex-config
kind: skill
stars: 194
last_pushed: 2025-12-19T14:58:05Z
license: unknown
score: 8
domains: [agents-ai, cli-tools, automation]
tags: [autonomous-agent, state-management, task-decomposition]
curated: 2026-06-14
curated_by: config-scout
---

# myysophia/codex-config — skill

**Why it's worth keeping:** The 'task_list + progress' loop effectively solves context window drift by treating the disk as the source of truth for long-running tasks.

**Summary:** A stateful orchestration pattern that implements task decomposition and progress tracking via local Markdown files to facilitate multi-session autonomy.

**Source credibility:** Relatively strong community signal with 194 stars on a specialized configuration repo.

**Recency:** Current; specifically references modern @anthropic-ai/claude-code CLI capabilities.

**Source:** [myysophia/codex-config/readme_skill.md](https://github.com/myysophia/codex-config/blob/9e3619cef80a3d83268fd9c075648617705ea37b/readme_skill.md) · 194★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Autonomous Skill (自主技能) 使用指南

**Autonomous Skill** 是一个用于处理复杂、长时任务的工具。它允许 Codex 在“非交互模式”下连续运行多个会话，自动分解任务、执行代码、跟踪进度，直到目标完成。

## 核心功能

*   **自动任务分解**：通过“初始化者 (Initializer)”智能分析需求，生成详细的任务清单 (`task_list.md`)。
*   **自主循环执行**：通过“执行者 (Executor)”自动读取清单，逐项执行，并在一个会话结束后自动开启下一个会话。
*   **断点续传**：所有状态保存在磁盘上，支持随时中断和恢复。

## 快速开始

所有操作均通过 `run-session.sh` 脚本完成。

### 1. 启动新任务

只需描述你想做什么，脚本会自动生成任务名并开始执行。

```bash
# 进入脚本目录 (或者直接使用绝对路径)
cd skills/autonomous-skill/scripts/

# 启动任务
./run-session.sh "为待办事项应用构建一个 REST API"
```

### 2. 查看任务列表

查看当前所有任务的状态（进行中、已完成）。

```bash
./run-session.sh --list
```

### 3. 继续已有任务

如果任务被中断（例如按了 Ctrl+C），或者是分阶段进行的，可以使用 `--continue` 继续。

```bash
# 先查看任务名
./run-session.sh --list

# 继续指定任务
./run-session.sh --task-name build-rest-api --continue
```

## 进阶用法

### 启用网络访问
如果任务需要访问互联网（例如抓取网页、API 交互），需要添加 `--network` 参数。
*注意：这将使用危险的无沙箱模式，请确保你信任该操作。*

```bash
./run-session.sh --network "分析 GitHub 上最新的热门 React 库"
```

### 恢复上一次的会话上下文
默认情况下，每次“执行者”会话都是新的（为了节省 Token），只读取 `task_list.md` 和 `progress.md`。如果你希望保留上一次对话的完整上下文（例如为了不仅关注任务清单，还要记住刚才的对话细节），可以使用 `--resume-last`。

```bash
./run-session.sh --task-name my-task --continue --resume-last
```

## Claude Skill 使用说明

当你希望“使用 Claude 或 Claude
```

</details>
