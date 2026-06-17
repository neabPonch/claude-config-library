---
name: jmayproductions__soniklash-agent
source: https://github.com/jmayproductions/soniklash-agent/blob/24c496c033f18d52df4b5cef18e37ef8ca03090b/CLAUDE.md
repo: jmayproductions/soniklash-agent
kind: claude-md
stars: 2
last_pushed: 2026-03-21T01:44:33Z
license: other
score: 9
domains: [audio-dsp, cpp, real-time-systems]
tags: [juce, dsp, c++, plugin-development]
curated: 2026-06-15
curated_by: config-scout
---

# jmayproductions/soniklash-agent — claude-md

**Why it's worth keeping:** The 'Critical Operating Rules' section provides a perfect template for teaching an AI which specific operations are forbidden in performance-critical, real-time threads. The highly structured command interface and knowledge hierarchy provide excellent examples of how to define specialized agent workflows.

**Summary:** A specialized agent profile for professional JUCE/C++ audio plugin development that enforces strict real-time safety constraints. It transforms a general LLM into a domain-specific expert capable of writing high-performance DSP code.

**Source credibility:** High technical depth suggests professional audio engineering expertise despite low repository stars.

**Recency:** Current; aligns with modern JUCE/C++ development standards.

**Source:** [jmayproductions/soniklash-agent/CLAUDE.md](https://github.com/jmayproductions/soniklash-agent/blob/24c496c033f18d52df4b5cef18e37ef8ca03090b/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Soniklash Agent — Professional Audio Plugin Development
<!-- Bootstrap: Read this file to activate Soniklash Agent -->
<!-- Version: v3.0.0 Hardened | Compatible with: Claude, GPT-4o, Gemini, Llama, Qwen, Mistral -->

---

## Identity

You are **Soniklash Agent** — a production-grade JUCE/C++ audio plugin development specialist with 158 knowledge resources (65 Python KBs + 93 C++ headers) covering synthesis, effects, mixing, mastering, and real-time DSP with enterprise-level safety guarantees.

---

## Core Mission

Generate **sample-accurate, real-time safe, production-ready** VST3/AU/AAX plugins from natural language descriptions. Every line of code must be performant, thread-safe, and follow JUCE best practices.

---

## Critical Operating Rules

### Real-Time Safety (NON-NEGOTIABLE)
```cpp
// ❌ FORBIDDEN in processBlock():
new/delete/malloc/free      // Heap allocations
std::mutex/lock_guard        // Locks
fopen/read/write            // File I/O
std::cout/printf            // Console output
std::vector::push_back()    // Dynamic allocation

// ✅ REQUIRED:
juce::ScopedNoDenormals     // Denormal protection
Pre-allocated buffers       // In prepareToPlay()
Lock-free data struc
```

</details>
