---
name: yaklang__hack-skills__skill
source: https://github.com/yaklang/hack-skills/blob/5bf2fd1eb50d20321b89b04920fd4c663c521bc9/skills/anti-debugging-techniques/SKILL.md
repo: yaklang/hack-skills
kind: skill
stars: 1095
last_pushed: 2026-06-04T07:22:15Z
license: mit
score: 9
domains: [security, reverse-engineering, systems-programming]
tags: [anti-debug, linux, windows, bypass, malware-analysis]
curated: 2026-06-15
curated_by: config-scout
---

# yaklang/hack-skills — skill

**Why it's worth keeping:** The inclusion of an 'AI LOAD INSTRUCTION' that addresses model weaknesses and a 'Quick bypass picks' table makes it highly actionable. The data is extremely granular (e.g., exact PEB/x64 offsets), moving beyond generic explanations to practical implementation details.

**Summary:** A high-density technical playbook for detecting and bypassing anti-debugging mechanisms on Linux and Windows. It provides specific memory offsets, assembly snippets, and tool-based bypass strategies.

**Source credibility:** High; the repository has significant community validation with over 1k stars.

**Recency:** Current; these techniques remain industry standards for low-level systems security and reverse engineering.

**Source:** [yaklang/hack-skills/skills/anti-debugging-techniques/SKILL.md](https://github.com/yaklang/hack-skills/blob/5bf2fd1eb50d20321b89b04920fd4c663c521bc9/skills/anti-debugging-techniques/SKILL.md) · 1095★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: anti-debugging-techniques
description: >-
  Anti-debugging detection and bypass playbook. Use when reversing protected
  binaries that detect debuggers via ptrace, PEB flags, timing checks, or
  signal/exception handlers on Linux and Windows.
---

# SKILL: Anti-Debugging Techniques — Detection & Bypass Playbook

> **AI LOAD INSTRUCTION**: Expert anti-debug techniques across Linux and Windows. Covers ptrace, PEB flags, NtQueryInformationProcess, timing attacks, signal-based detection, TLS callbacks, VEH tricks, and all corresponding bypass methods. Base models often miss the distinction between user-mode and kernel-mode detection and the correct patching strategy for each.

## 0. RELATED ROUTING

- [code-obfuscation-deobfuscation](../code-obfuscation-deobfuscation/SKILL.md) when the binary also uses control flow flattening, VM protection, or string encryption
- [vm-and-bytecode-reverse](../vm-and-bytecode-reverse/SKILL.md) when the anti-debug sits inside a custom VM dispatcher
- [symbolic-execution-tools](../symbolic-execution-tools/SKILL.md) when you want to symbolically skip anti-debug checks entirely

### Advanced Reference

Also load [ANTI_DEBUG_MATRIX.md](./ANTI_DEBUG
```

</details>
