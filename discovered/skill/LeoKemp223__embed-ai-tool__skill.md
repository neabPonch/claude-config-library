---
name: LeoKemp223__embed-ai-tool__skill
source: https://github.com/LeoKemp223/embed-ai-tool/blob/f32330c347f712871e1971e3bb437cd0cd129493/skills/build-cmake/SKILL.md
repo: LeoKemp223/embed-ai-tool
kind: skill
stars: 599
last_pushed: 2026-05-21T07:15:17Z
license: unknown
score: 9
domains: [embedded-systems, cli-tools, devops]
tags: [cmake, embedded, workflow, orchestration]
curated: 2026-06-15
curated_by: config-scout
---

# LeoKemp223/embed-ai-tool — skill

**Why it's worth keeping:** Uses professional agentic patterns like structured failure routing (e.g., 'artifact-missing') and explicit handoff instructions to link skills together in a workflow.

**Summary:** A highly structured skill for managing CMake-based embedded firmware builds through environment auto-detection and state persistence.

**Source credibility:** High; the repository has significant community validation with nearly 600 stars.

**Recency:** Very current; updated within the last month.

**Source:** [LeoKemp223/embed-ai-tool/skills/build-cmake/SKILL.md](https://github.com/LeoKemp223/embed-ai-tool/blob/f32330c347f712871e1971e3bb437cd0cd129493/skills/build-cmake/SKILL.md) · 599★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: build-cmake
description: 当需要配置或构建基于 CMake 的嵌入式固件工程，调用自带脚本执行构建并定位固件产物时使用。
---

# 构建 CMake 工程

## 适用场景

- `Project Profile` 中标明 `build_system: cmake`。
- 用户希望对 CMake MCU 工程执行配置、重编译或确认固件产物。
- 烧录或调试流程需要新的 `ELF`、`HEX` 或 `BIN`。
- 需要在构建前确认环境是否就绪（cmake、生成器、工具链）。

## 必要输入

- 工作区路径，或一份已有的 `Project Profile`。
- 可选的构建预设、构建目录、目标名、生成器、构建类型和工具链文件。

## 自动探测

- 若存在 `CMakePresets.json`，优先使用脚本的 `--list-presets` 列出并选择预设。
- 否则检查 `CMakeLists.txt`、已有构建目录和工具链文件。
- 若已有成功的构建目录且与当前意图一致，优先复用。
- 生成器由脚本自动探测，优先 `Ninja`，其次是宿主机上已安装的 Make 工具。
- 对调试导向请求默认使用 `Debug`，否则默认使用 `RelWithDebInfo`。

## 执行步骤

1. 先阅读 [references/usage.md](references/usage.md)，确认本次是环境探测、列出预设、执行构建，还是仅扫描产物。
2. 若不确定环境是否就绪，先运行自带脚本 [scripts/cmake_builder.py](scripts/cmake_builder.py) 的 `--detect` 模式确认。
3. 若存在 CMakePresets.json，使用 `--list-presets` 列出预设，再用 `--preset <name>` 构建。
4. 若无预设，使用 `--source`、`--build-dir`、`--generator`、`--build-type`、`--toolchain` 手动配置构建。
5. 读取脚本输出的构建结果和产物扫描报告，重点关注首选产物（ELF > HEX > BIN）和失败分类。
6. 将构建目录、产物路径、产物类型和生成器信息写回 `Project Profile`，并在需要时交给下游 skill。

## 失败分流

- 当缺少 `cmake` 或所需生成器时，返回 `environment-missing`。
- 当配置或构建因预设损坏、缺失工具链文件或目标名无效而失败时，返回 `project-config-error`。
- 当构建看似成功但未找到可烧录或可调试产物时，返回 `artifact-missing`。
- 当存在
```

</details>
