---
name: libriscv__godot-sandbox
source: https://github.com/libriscv/godot-sandbox/blob/97713ae3d74b3aeca277f0edeea401e74e420340/CLAUDE.md
repo: libriscv/godot-sandbox
kind: claude-md
stars: 450
last_pushed: 2026-05-09T04:30:28Z
license: bsd-3-clause
score: 9
domains: [systems-programming, compiler-engineering, game-engine]
tags: [risc-v, godot, low-level-abi, compiler-debugging]
curated: 2026-06-15
curated_by: config-scout
---

# libriscv/godot-sandbox — claude-md

**Why it's worth keeping:** It includes precise CLI commands for internal debugging tools and critical low-level memory/ABI constraints that prevent errors when writing assembly or C++ interaction code.

**Summary:** Provides deep technical context for a RISC-V sandbox, covering compiler architecture, debugging tool usage, and low-level ABI specifications.

**Source credibility:** High; the project has significant star count and recent maintenance activity within a complex domain.

**Recency:** Very current, with updates from only one month ago.

**Source:** [libriscv/godot-sandbox/CLAUDE.md](https://github.com/libriscv/godot-sandbox/blob/97713ae3d74b3aeca277f0edeea401e74e420340/CLAUDE.md) · 450★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
This project is a sandbox addon for the Godot engine. It implements a Sandbox node which can load a RISC-V ELF binary, which can then execute code and access the host Godot instance. The access can be restricted by class names, methods, properties etc. Execution is memory safe and has an optional execution timeout using instruction counting. The underlying emulator is libriscv. The emulator runs either in JIT or interpreter mode. This can be toggled during init. Both JIT and interpreter modes are faster than GDScript. Whitespace is tabs.

The Sandbox node can be instantiated, given an ELF and then it can export functions and properties making it a sort-of script-like instance. It can also be used as a Script, by attaching it to the Script of any Node. In that case, calling functions on the node will be forwarded to the script, which again calls into the sandboxed guest program. The sandbox node is implemented in src/sandbox.cpp and src/sandbox.h as well as a few src/sandbox_*.cpp files. The cpp ScriptLanguage is in src/cpp/*. The sandbox API is implemented in src/sandbox_syscalls.cpp and sandbox_syscalls_*.cpp.

The API inside the Sandbox follows the public GDScript API closely, si
```

</details>
