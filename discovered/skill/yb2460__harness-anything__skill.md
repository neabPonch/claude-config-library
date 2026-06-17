---
name: yb2460__harness-anything__skill
source: https://github.com/yb2460/harness-anything/blob/b3a42f0efa20663974743468cb0bbddc89107c06/photoshop-harness/skills/cli-anything-photoshop/SKILL.md
repo: yb2460/harness-anything
kind: skill
stars: 799
last_pushed: 2026-06-12T03:16:49Z
license: mit
score: 9
domains: [cli-tools, automation, creative-software]
tags: [photoshop, com-automation, windows-api]
curated: 2026-06-15
curated_by: config-scout
---

# yb2460/harness-anything — skill

**Why it's worth keeping:** The implementation features a crucial `--json` flag for machine-readable output and organizes complex GUI state into logical command groups (project/layer/text). This pattern of providing structured control over opaque desktop software is highly transferable to any COM or CLI-capable application.

**Summary:** A CLI bridge that uses Windows COM automation to allow AI agents to programmatically control Adobe Photoshop. It enables high-level manipulation of layers, text, and document properties through structured commands.

**Source credibility:** High; 799 stars indicates significant utility, and the repo shows active maintenance.

**Recency:** Extremely current; specifically designed for modern agentic workflows like Claude Code.

**Source:** [yb2460/harness-anything/photoshop-harness/skills/cli-anything-photoshop/SKILL.md](https://github.com/yb2460/harness-anything/blob/b3a42f0efa20663974743468cb0bbddc89107c06/photoshop-harness/skills/cli-anything-photoshop/SKILL.md) · 799★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: "cli-anything-photoshop"
description: "通过 COM 自动化操控 Adobe Photoshop 的 CLI harness。支持项目管理、图层操作、选区控制、文字编辑、图像调整和多格式导出。"
---

# CLI-Anything Photoshop

通过 Windows COM 自动化接口操控 Adobe Photoshop 的命令行工具。

## 前置条件

- **Windows 10/11**
- **Adobe Photoshop 2023+** (需注册 COM 接口)
- **Python 3.10+** 及 `pywin32` 包

## 安装

```bash
cd photoshop-harness/agent-harness
pip install -e .
```

安装后可使用 `cli-anything-photoshop` 命令。

## 命令结构

```
cli-anything-photoshop [--json] [--project <path>] [--dry-run] <command-group> <command> [options]
```

### 全局选项

| 选项 | 描述 |
|------|------|
| `--json` | 以 JSON 格式输出（供 AI Agent 解析） |
| `--project <path>` | 自动打开或创建 PSD 项目文件 |
| `--dry-run` | 执行命令但不保存到磁盘 |

## 命令组

### project — 项目管理
| 命令 | 选项 | 描述 |
|------|------|------|
| `new <path>` | `-w` width, `-h` height, `-r` resolution, `-m` mode, `-b` bg-color | 创建新 PSD |
| `open <path>` | | 打开 PSD 文件 |
| `save [path]` | | 保存文档 |
| `close` | `--no-save` | 关闭文档 |

### document — 文档操作
| 命令 | 选项 | 描述 |
|------|------|------|
| `info` | | 文档信息 |
| `resize` | `-w` width, `-h` height, `-r` resolution | 调整尺寸 |
| `canvas` | `-w` width, `-h` height, `-a` anchor | 调整画布 |
| `crop` | `--left --top --right --bottom` | 裁切 |
| `
```

</details>
