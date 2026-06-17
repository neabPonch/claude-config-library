---
name: GoogleChrome__modern-web-guidance-src__skill
source: https://github.com/GoogleChrome/modern-web-guidance-src/blob/9f21354503bbb7b734e71390d008aa82ad1ae049/skills-src/cpp-on-the-web/SKILL.md
repo: GoogleChrome/modern-web-guidance-src
kind: skill
stars: 759
last_pushed: 2026-06-12T22:24:06Z
license: apache-2.0
score: 9
domains: [web-assembly, cpp, frontend-tooling]
tags: [wasm, emscripten, cpp, optimization]
curated: 2026-06-15
curated_by: config-scout
---

# GoogleChrome/modern-web-guidance-src — skill

**Why it's worth keeping:** Contains highly specific, actionable compiler flag recommendations (e.g., -sSTRICT, -sEXPORT_ES6) and precise workflows for separate compilation/linking that prevent common WASM integration errors.

**Summary:** Provides expert guidance for compiling C++ via Emscripten into modern ES6-compatible WebAssembly modules.

**Source credibility:** Extremely high; originates from a Google Chrome official guidance repository.

**Recency:** Very current; focuses on modern ES6 module output and contemporary JS/C++ interop techniques.

**Source:** [GoogleChrome/modern-web-guidance-src/skills-src/cpp-on-the-web/SKILL.md](https://github.com/GoogleChrome/modern-web-guidance-src/blob/9f21354503bbb7b734e71390d008aa82ad1ae049/skills-src/cpp-on-the-web/SKILL.md) · 759★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: cpp-on-the-web
description: Compiling C and C++ for the modern web using WebAssembly. Use this skill when you need to port C++ code, build C++ libraries with Emscripten, or set up high-performance C++ components in the browser.
---

# Compiling C++ to the Web using WebAssembly

This skill provides guidance for using **Emscripten** to target the modern web with C and C++. It focuses on ES6 module output, clean JS/C++ interop, and common pitfalls.

## Quick Start

1. **Installation:** Use the [Emscripten SDK (emsdk)](https://github.com/emscripten-core/emsdk) as the quickest way to install.
   ```bash
   ./emsdk install latest
   ./emsdk activate latest
   source ./emsdk_env.sh
   ```
2. **Environment:** Ensure `emcc` is in your PATH.
3. **Boilerplate:** Use the `hello-world` template in `assets/hello-world`.
   - `main.cpp`: Basic Embind example.
   - `index.html`: Modern ES6 module loading.
   - `Makefile`: Recommended flags for modern web.

## Recommended Compilation Flags

- `-sSTRICT`: Opt into modern Emscripten behavior.
- `-sEXPORT_ES6`: Output a modern ES6 module (this implies `-sMODULARIZE`).
- `-sENVIRONMENT=web`: For optimal codesize limit the output only run on t
```

</details>
