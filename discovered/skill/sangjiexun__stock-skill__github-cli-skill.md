---
name: sangjiexun__stock-skill__github-cli-skill
source: https://github.com/sangjiexun/stock-skill/blob/6e6f0bce1c0df9f149a39e73c142e1e57316d343/doc/github-cli-skill.md
repo: sangjiexun/stock-skill
kind: skill
stars: 3
last_pushed: 2026-05-31T07:54:34Z
license: unknown
score: 7
domains: [cli-tools, devops]
tags: [github-cli, git, proxy, configuration]
curated: 2026-06-15
curated_by: config-scout
---

# sangjiexun/stock-skill — skill

**Why it's worth keeping:** Provides highly specific Git/gh configuration patterns (like `instead-of` URL mappings) that are essential for troubleshooting connectivity issues in restricted environments.

**Summary:** A specialized technical reference for GitHub CLI, focused on navigating network restrictions through mirroring and proxy configurations.

**Source credibility:** High density of actionable, expert-level command sequences tailored to specific regional technical challenges.

**Recency:** Up-to-date with modern GitHub CLI (`gh`) workflows and proxying best practices.

**Source:** [sangjiexun/stock-skill/doc/github-cli-skill.md](https://github.com/sangjiexun/stock-skill/blob/6e6f0bce1c0df9f149a39e73c142e1e57316d343/doc/github-cli-skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: github-cli-skill
description: "GitHub CLI 工具箱 - 中国开发者适配版。支持gh CLI安装、镜像加速、代理配置、SSH/HTTPS切换，解决GitHub访问慢/连不上的问题。当用户提到github、gh cli、git clone、github加速、github代理时使用。"
emoji: "🐙"
homepage: "https://github.com/cli/cli"
install:
  - kind: pip
    package: requests
---

# GitHub CLI 中国开发者适配 Skill 🐙

## 核心能力（6大模块）

| 模块 | 命令 | 功能 | 场景 |
|------|------|------|------|
| 1️⃣ 安装配置 | `install` | 安装/更新 GitHub CLI | 首次使用 |
| 2️⃣ 镜像加速 | `mirror` | 配置 gh-proxy 等镜像 | 解决访问慢 |
| 3️⃣ 代理配置 | `proxy` | 设置 HTTP/SOCKS 代理 | 企业网络 |
| 4️⃣ SSH/HTTPS | `auth` | 认证和协议切换 | 安全访问 |
| 5️⃣ 仓库操作 | `repo` | clone/push/pull 等 | 日常开发 |
| 6️⃣ PR/Issue | `pr_issue` | PR 和 Issue 管理 | 协作开发 |

---

## 一、安装配置 (install)

### 安装 GitHub CLI

```bash
# Windows - 使用 winget
winget install GitHub.cli

# Windows - 使用 Chocolatey
choco install gh

# macOS - 使用 Homebrew
brew install gh

# Linux - 使用 apt
apt install gh

# Python pip 安装（备用）
pip install requests
```

### 验证安装

```bash
gh --version
# gh version 2.XX.X (2026-XX-XX)
```

### 认证登录

```bash
# 交互式登录
gh auth login

# 使用 token 登录（适合自动化）
gh auth login --with-token < TOKEN

# 查看当前认证状态
gh auth status
```

---

## 二、镜像加速 (mirror)

> 💡 解决 GitHub 访问慢、下载失败问题

### 公共镜像服务

| 镜像服务 | 网
```

</details>
