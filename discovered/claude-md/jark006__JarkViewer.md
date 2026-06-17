---
name: jark006__JarkViewer
source: https://github.com/jark006/JarkViewer/blob/d77b60a1258db7f5a692853664e151d0b65a2718/CLAUDE.md
repo: jark006/JarkViewer
kind: claude-md
stars: 1166
last_pushed: 2026-05-24T16:35:20Z
license: gpl-3.0
score: 9
domains: [desktop-app, systems-programming, image-processing]
tags: [cpp, win32, opencv]
curated: 2026-06-15
curated_by: config-scout
---

# jark006/JarkViewer — claude-md

**Why it's worth keeping:** Includes critical 'Modification Precautions' regarding binary compatibility and specific build-time dependencies, plus a detailed runtime data flow to navigate event-driven logic.

**Summary:** Provides comprehensive build instructions, architectural decomposition, and runtime data flow for a specialized Win32/C++/OpenCV project.

**Source credibility:** Highly credible: 1k+ stars and actively maintained repository.

**Recency:** Very current; utilizes modern C++23 standards.

**Source:** [jark006/JarkViewer/CLAUDE.md](https://github.com/jark006/JarkViewer/blob/d77b60a1258db7f5a692853664e151d0b65a2718/CLAUDE.md) · 1166★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## 项目概览

JarkViewer 是 Windows 10/11 x64 原生图片查看器，使用 C++23、Win32、Direct3D 11 和 OpenCV 构建。它以单可执行文件方式发布，重点支持大量静态图、动图、RAW、LivePhoto/MotionPhoto、EXIF 信息显示、打印/简单编辑和文件关联。

## 常用命令

本项目优先使用 PowerShell 执行仓库根目录下的 `buildRelease.ps1` 脚本进行编译、构建：

```powershell
# Release x64 构建
./buildRelease.ps1

# 运行已构建程序
./x64/Release/JarkViewer.exe
./x64/Release/JarkViewer.exe "D:/path/to/image.png"
```

每次修改后至少保证 `buildRelease.ps1` 能干净编译通过；行为变更需手动冒烟验证静态图加载、动图播放、EXIF 显示、打印预览和导出流程。

## 构建前提

- 项目文件是 `JarkViewer/JarkViewer.vcxproj`，工具集为 `v145`，语言标准为 C++23，目标平台为 x64；需要安装支持 v145 工具集的 Visual Studio/Build Tools。
- `JarkViewer.vcxproj` 中 `VcpkgEnabled=false`，默认使用仓库内的静态库目录：`JarkViewer/lib*`、`JarkViewer/ffmpeg`、`JarkViewer/include`。
- README 说明第三方静态库需从 release 的 `static_lib` 包准备；如果改为 vcpkg，需要在项目属性中启用并补齐依赖。
- Release 输出程序位于 `x64/Release/JarkViewer.exe`，中间文件位于 `JarkViewer/x64/<Configuration>`。

## 高层架构

- `JarkViewer/src/main.cpp` 定义 `JarkViewerApp` 和 `wWinMain`。入口初始化 Exiv2 BMFF、禁用 IME、初始化 COM，然后创建窗口、解析命令行图片路径并进入主循环。
- `JarkViewer/include/D3D11App.h` 与 `JarkViewer/src/D3D11App.cpp` 提供 Win32 窗口、消息分发、Direct
```

</details>
