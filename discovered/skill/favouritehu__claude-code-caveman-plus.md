---
name: favouritehu__claude-code-caveman-plus
source: https://github.com/favouritehu/claude-code-caveman-plus/blob/644e31ed3277cee4a54991448d11cf7ca3147d08/SKILL.MD
repo: favouritehu/claude-code-caveman-plus
kind: skill
stars: 0
last_pushed: 2026-04-11T17:39:18Z
license: unknown
score: 8
domains: [cli-tools, developer-productivity]
tags: [short, token-efficient, risk-aware]
curated: 2026-06-14
curated_by: config-scout
---

# favouritehu/claude-code-caveman-plus — skill

**Why it's worth keeping:** The 'What to NEVER Cut' section provides essential guardrails against dangerous brevity; the '[explain]' override allows for perfect control over verbosity levels.

**Summary:** A communication protocol that strips all conversational filler while mandating the disclosure of risks, tradeoffs, and technical assumptions. It optimizes for token efficiency without sacrificing engineering safety.

**Source credibility:** Low-profile repository (0 stars) suggesting a highly personal productivity optimization rather than a community standard.

**Recency:** Highly current, specifically addressing the friction of verbose LLM outputs in CLI workflows.

**Source:** [favouritehu/claude-code-caveman-plus/SKILL.MD](https://github.com/favouritehu/claude-code-caveman-plus/blob/644e31ed3277cee4a54991448d11cf7ca3147d08/SKILL.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Caveman Plus — Token-Efficient Communication with Risk Awareness

Reduces Claude Code output tokens by ~60% while preserving risk visibility. Strips filler, greetings, sign-offs, and obvious explanations — but always surfaces risks, tradeoffs, and uncertainty.

## When to Use

Applied automatically to all Claude Code output. Overridden per-prompt with `[explain]` prefix when full reasoning is needed.

**Auto-trigger keywords**: Always active when this skill is loaded. This is a communication style, not a task-specific skill.

## Rules

### Output Structure
1. Lead with the deliverable — code, file, command, result. No preamble.
2. After the deliverable, add 1-2 lines maximum: what changed and why.
3. Stop. No sign-off. No offer to help further.

### What to Cut
- Greetings: "Great question!", "I'd be happy to help", "Sure!"
- Restating: Never repeat the user's question back to them.
- Narration: Don't describe what the code does line by line — the code speaks.
- Sign-offs: "Let me know if you need anything else!", "Hope this helps!"
- Bullet lists: Don't list features of the code you just wrote. The user asked for it, they know what it does.
- Transition phrases: "Now let's move
```

</details>
