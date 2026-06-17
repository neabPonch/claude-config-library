---
name: Sagit-chu__flvx__ai-skill
source: https://github.com/Sagit-chu/flvx/blob/3ce320da5a687c07fd341726f2f283fa4561569a/doc/ai-skill.md
repo: Sagit-chu/flvx
kind: skill
stars: 234
last_pushed: 2026-06-09T00:43:53Z
license: gpl-3.0
score: 8
domains: [backend-api, agents-ai, automation]
tags: [rest-api, tool-integration, auth-logic]
curated: 2026-06-15
curated_by: config-scout
---

# Sagit-chu/flvx — skill

**Why it's worth keeping:** It includes crucial implementation details like the non-standard authentication header format (omitting 'Bearer') which prevents tool-call failures.

**Summary:** Provides a structured method for exposing a REST API to AI agents via CLAUDE.md documentation.

**Source credibility:** High; 234 stars and very recent activity indicate a functional, real-world tool.

**Recency:** 

**Source:** [Sagit-chu/flvx/doc/ai-skill.md](https://github.com/Sagit-chu/flvx/blob/3ce320da5a687c07fd341726f2f283fa4561569a/doc/ai-skill.md) · 234★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Skill 使用指南

让大模型直接操作 FLVX 面板的技能包。支持 OpenCode、OpenClaw、Claude Code 等工具。

## 安装

### 方式 1: npm (推荐)

```bash
npm install -g @flvx/skill-api
```

postinstall 脚本会自动链接到 `~/.agents/skills/flvx-api/`。

### 方式 2: 手动链接

```bash
# 从 FLVX 源码
cd /path/to/flvx
mkdir -p ~/.agents/skills
ln -sf $(pwd)/skills/flvx-api ~/.agents/skills/

# 或从 GitHub
git clone https://github.com/Sagit-chu/flvx.git
cd flvx
ln -sf $(pwd)/skills/flvx-api ~/.agents/skills/
```

## 配置

设置环境变量：

```bash
export FLVX_BASE_URL="https://your-panel.example.com"
export FLVX_USERNAME="admin"
export FLVX_PASSWORD="your-password"
```

或使用凭证文件：

```bash
mkdir -p ~/.flvx
cat > ~/.flvx/.env << 'EOF'
export FLVX_BASE_URL="https://panel.example.com"
export FLVX_USERNAME="admin"
export FLVX_PASSWORD="your-password"
EOF
chmod 600 ~/.flvx/.env
source ~/.flvx/.env
```

---

## 工具接入方法

### OpenCode

OpenCode 是命令行 AI 编程助手，支持通过 skills 扩展能力。

**安装 skill:**
```bash
npm install -g @flvx/skill-api
```

**使用:**
```bash
export FLVX_BASE_URL="https://panel.example.com"
export FLVX_USERNAME="admin"
export FLVX_PASSWORD="your-password"

opencode
```

**示例对话:**
```
你: 查看我的转发列表
你: 创建一个转发到 192.168.1.100:80 使用隧道 1
你: 检查节点状态
你: 查看流量使用情况
```

---

###
```

</details>
