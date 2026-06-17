---
name: phpolygon__php-vio
source: https://github.com/phpolygon/php-vio/blob/0ab8f90188df7534e80f086e743f99425c1c34b8/CLAUDE.md
repo: phpolygon/php-vio
kind: claude-md
stars: 1
last_pushed: 2026-06-15T20:49:26Z
license: mit
score: 9
domains: [systems-programming, graphics-api]
tags: [build-instructions, architecture-map, c-extension]
curated: 2026-06-16
curated_by: config-scout
---

# phpolygon/php-vio — claude-md

**Why it's worth keeping:** Provides hyper-specific shell commands for various environments (macOS/Linux/Windows) and detailed maps of low-level object lifecycles and design patterns.

**Summary:** High-density technical specification including platform-specific build/test commands and internal architecture mapping.

**Source credibility:** Single star repo; content density suggests high-level systems programming expertise.

**Recency:** Extremely current (last pushed 0 months ago).

**Source:** [phpolygon/php-vio/CLAUDE.md](https://github.com/phpolygon/php-vio/blob/0ab8f90188df7534e80f086e743f99425c1c34b8/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# php-vio — PHP Video Input Output Extension

## Was ist das?

Eine PHP C-Extension die GPU-Rendering (OpenGL 4.1, Vulkan, Metal), Audio, Video-Recording, Streaming und Input in PHP verfügbar macht. Basis-Infrastruktur für die PHPolygon Game Engine.

## Build

### macOS (Homebrew)

```bash
# PHP 8.5 (Homebrew)
make clean; phpize --clean; phpize && \
./configure --enable-vio --with-glfw --with-glslang --with-spirv-cross --with-vulkan --with-ffmpeg --with-metal && \
make -j$(sysctl -n hw.ncpu)

# PHP 8.4 (Laravel Herd)
make clean; /usr/local/Cellar/php@8.4/8.4.19/bin/phpize --clean
/usr/local/Cellar/php@8.4/8.4.19/bin/phpize && \
./configure --enable-vio --with-glfw --with-glslang --with-spirv-cross --with-vulkan --with-ffmpeg --with-metal \
  --with-php-config=/usr/local/Cellar/php@8.4/8.4.19/bin/php-config && \
make -j$(sysctl -n hw.ncpu)
```

### Linux

```bash
# Dependencies (Ubuntu/Debian)
sudo apt install php-dev libglfw3-dev glslang-dev libvulkan-dev \
  libavcodec-dev libavformat-dev libavutil-dev libswscale-dev \
  spirv-cross libspirv-cross-c-shared-dev

# Build (kein --with-metal auf Linux)
phpize && \
./configure --enable-vio --with-glfw --with-glslang --with-spirv-cross
```

</details>
