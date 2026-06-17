---
name: emgucv__emgutf
source: https://github.com/emgucv/emgutf/blob/48809f69ae0ed886604fc93da5031b83db6147cb/CLAUDE.md
repo: emgucv/emgutf
kind: claude-md
stars: 222
last_pushed: 2026-04-22T01:27:20Z
license: other
score: 9
domains: [.net, native-interop, machine-learning]
tags: [pinvoke, tensorflow, csharp, cpp-wrapper]
curated: 2026-06-15
curated_by: config-scout
---

# emgucv/emgutf — claude-md

**Why it's worth keeping:** It explicitly warns about auto-generated code to prevent AI edits and provides highly specific P/Invoke marshaling conventions necessary for low-level development. The build section detail is excellent, accounting for the high complexity of building native dependencies via Bazel and CMake.

**Summary:** This file provides a comprehensive blueprint for a complex multi-layer architecture involving native C++ and .NET interop.

**Source credibility:** High; a well-maintained, specialized wrapper project with significant star count.

**Recency:** Current; includes references to modern toolchains like Visual Studio 2022/2026.

**Source:** [emgucv/emgutf/CLAUDE.md](https://github.com/emgucv/emgutf/blob/48809f69ae0ed886604fc93da5031b83db6147cb/CLAUDE.md) · 222★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Emgu TF is a cross-platform .NET wrapper for the Google TensorFlow library, enabling TF functions to be called from C#, VB, VC++, and IronPython. The repo contains two main wrappers:
- **Emgu TF** — full TensorFlow model loading/running (Windows, macOS, Linux, Android)
- **Emgu TF Lite** — TensorFlow Lite model loading/running (Windows, macOS, Linux, Android, iOS)

The native C++ layer is exposed through P/Invoke via two extern libraries: `tfextern` (full TF) and `tfliteextern` (TF Lite).

## Architecture

### Layer structure
1. **Native layer** — C/C++ wrapper DLLs built from the `tensorflow/` submodule using CMake or Bazel. The DLLs (`tfextern`, `tfliteextern`) must be present in `lib/runtimes/<rid>/native/` before building .NET code.
2. **P/Invoke layer** — `TfInvoke` (in `Emgu.TF/`) and `TfLiteInvoke` (in `Emgu.TF.Lite/`) are partial static classes that expose the native DLL entry points via `[DllImport]`.
3. **Managed wrappers** — `Graph`, `Session`, `Tensor`, `Interpreter`, etc. inherit `UnmanagedObject` (from `Emgu.TF.Util/`) and wrap nati
```

</details>
