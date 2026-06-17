---
name: nndeploy__nndeploy
source: https://github.com/nndeploy/nndeploy/blob/4ad43d9ab299c52fe6f5b7f99d4e5b1cda0ddf06/CLAUDE.md
repo: nndeploy/nndeploy
kind: claude-md
stars: 1829
last_pushed: 2026-04-25T11:15:25Z
license: apache-2.0
score: 9
domains: [cpp, ai-frameworks, embedded-systems]
tags: [architecture, build-system, extension-patterns, high-performance]
curated: 2026-06-15
curated_by: config-scout
---

# nndeploy/nndeploy — claude-md

**Why it's worth keeping:** The 'Key Patterns' section provides actionable templates for extension, while the detailed build-time configuration options prevent AI from guessing how to enable features.

**Summary:** Provides a deep architectural blueprint and procedural 'recipes' for extending the framework via new backends or nodes.

**Source credibility:** High; a popular repository (1829 stars) with recent activity and professional documentation structure.

**Recency:** Current; highly relevant for Claude Code's ability to navigate complex C++ codebases and build systems.

**Source:** [nndeploy/nndeploy/CLAUDE.md](https://github.com/nndeploy/nndeploy/blob/4ad43d9ab299c52fe6f5b7f99d4e5b1cda0ddf06/CLAUDE.md) · 1829★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

nndeploy is a high-performance AI deployment framework for edge computing (desktop, mobile, edge devices, servers). It provides a visual workflow editor and supports 13+ inference backends including ONNXRuntime, TensorRT, OpenVINO, MNN, TNN, ncnn, CoreML, AscendCL, RKNN, SNPE, TVM, PyTorch, and an internal inference engine.

## Build Commands

### Basic Build (Linux/macOS)

```bash
mkdir build && cd build # 假如存在，则不新建
cp ../cmake/config.cmake . # 假如当前目录已经存在config.cmake，则不拷贝
cmake ..
make -j
make install
```

The build creates:
- `libnndeploy_framework.so` (or `.dll`/`.dylib`) - Main framework library
- `libnndeploy_plugin_*.so` - Algorithm plugins
- `nndeploy_demo_*` - Demo executables
- `build/nndeploy_${VERSION}_${PLATFORM}_...` - Install directory

### Build Configuration

Edit `build/config.cmake` to enable/disable components. Key options:
- `ENABLE_NNDEPLOY_BUILD_SHARED` - Build shared library (default ON)
- `ENABLE_NNDEPLOY_DEVICE_CUDA` - Enable NVIDIA CUDA
- `ENABLE_NNDEPLOY_DEVICE_ASCEND_CL` - Enable Huawei Ascend
- `ENABLE_NNDEPLOY_INFERE
```

</details>
