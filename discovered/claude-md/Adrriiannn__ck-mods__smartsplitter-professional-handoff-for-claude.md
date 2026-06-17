---
name: Adrriiannn__ck-mods__smartsplitter-professional-handoff-for-claude
source: https://github.com/Adrriiannn/ck-mods/blob/e9a46b4ed2c3b719cc599480334530877068420a/Docs/SmartSplitter_Professional_Handoff_For_Claude.md
repo: Adrriiannn/ck-mods
kind: claude-md
stars: 0
last_pushed: 2026-06-07T12:17:33Z
license: unknown
score: 9
domains: [game-dev, unity-ecs]
tags: [handoff, refactor-guide, technical-debt, context-injection]
curated: 2026-06-16
curated_by: config-scout
---

# Adrriiannn/ck-mods — claude-md

**Why it's worth keeping:** It utilizes a 'preserve vs. restructure' framework that prevents agents from repeating previous architectural errors. It also provides critical environmental discovery including specific Unity versions, local paths, and hard-won technical truths about the game engine.

**Summary:** A high-level technical handoff document that distinguishes between proven backend ECS logic and experimental UI layers to guide refactoring.

**Source credibility:** The content demonstrates high technical density consistent with professional software engineering handoffs despite low repo visibility.

**Recency:** Highly current; optimized for AI-driven refactoring and implementation tasks.

**Source:** [Adrriiannn/ck-mods/Docs/SmartSplitter_Professional_Handoff_For_Claude.md](https://github.com/Adrriiannn/ck-mods/blob/e9a46b4ed2c3b719cc599480334530877068420a/Docs/SmartSplitter_Professional_Handoff_For_Claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Smart Splitter Mod — Professional Technical Handoff for Restructure / Rebuild

**Project:** Core Keeper Smart Splitter Mod  
**Audience:** New implementation owner / Claude / another coding agent taking over from a research prototype  
**Authoring context:** Core Keeper Mod SDK, Unity 6000.0.59f2, ECS-heavy vanilla automation internals  
**Primary goal:** Hand off everything learned so the next implementation can restructure the mod cleanly instead of extending the current messy prototype.

---

## 0. Executive Summary

The Smart Splitter project set out to create a Core Keeper splitter variant that can route items by filter rules instead of vanilla alternating/splitting behavior. The target gameplay behavior evolved into:

```text
Unpowered Smart Splitter:
    behave exactly like vanilla Conveyor Belt Splitter

Powered Smart Splitter:
    evaluate configured lane filters
    send matching items left/right without splitting stacks unnecessarily
    optionally send unmatched items forward as a passthrough/reject lane
    expose a UI similar to Robot Arm filtering UI
```

The project produced one **high-value, production-relevant backend discovery** and one **low-quality, likely-to
```

</details>
