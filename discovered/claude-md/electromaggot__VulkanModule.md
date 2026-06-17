---
name: electromaggot__VulkanModule
source: https://github.com/electromaggot/VulkanModule/blob/d69518944510692586e1f85480f741639962f4fc/CLAUDE.md
repo: electromaggot/VulkanModule
kind: claude-md
stars: 1
last_pushed: 2026-03-20T05:05:51Z
license: unlicense
score: 9
domains: [graphics, cpp]
tags: [vulkan, architecture, build-system]
curated: 2026-06-15
curated_by: config-scout
---

# electromaggot/VulkanModule — claude-md

**Why it's worth keeping:** The inclusion of 'Advanced Features' with code examples teaches Claude specific implementation patterns (like RAII and dynamic buffer usage) rather than just file locations.

**Summary:** Provides exhaustive platform-specific build instructions and deep architectural context for a high-performance Vulkan graphics module.

**Source credibility:** Low star count, but the technical depth suggests a professional-grade specialized library.

**Recency:** Current; uses modern CMake workflows and platform-specific dependency management.

**Source:** [electromaggot/VulkanModule/CLAUDE.md](https://github.com/electromaggot/VulkanModule/blob/d69518944510692586e1f85480f741639962f4fc/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Building and Running

### Prerequisites

#### All Platforms
- CMake 3.16+
- Vulkan SDK
- SDL2 and SDL2_image libraries
- GLM (OpenGL Mathematics library)

#### Platform-Specific Setup

**macOS:**
```bash
# Install via Homebrew
brew install vulkan-headers vulkan-loader molten-vk sdl2 sdl2_image glm
```

**Windows:**
- Install Vulkan SDK from https://vulkan.lunarg.com/
- Use vcpkg for dependencies:
```cmd
vcpkg install sdl2 sdl2-image glm vulkan
```

**Linux/Ubuntu:**
```bash
sudo apt-get update
sudo apt-get install vulkan-tools libvulkan-dev vulkan-validationlayers-dev
sudo apt-get install libsdl2-dev libsdl2-image-dev libglm-dev
sudo apt-get install build-essential cmake pkg-config
```

**Raspberry Pi 5:**
```bash
# Same as Linux, plus ARM64-specific packages
sudo apt-get install gcc-aarch64-linux-gnu g++-aarch64-linux-gnu
```

### Build the TestHarness

**All Platforms:**
```bash
cd TestHarness
mkdir -p build && cd build
cmake ..
cmake --build . -j$(nproc)
```

**Windows (Visual Studio):**
```cmd
cd TestHarness
mkdir build && cd build
cmake .. -G "Visual Studio 1
```

</details>
