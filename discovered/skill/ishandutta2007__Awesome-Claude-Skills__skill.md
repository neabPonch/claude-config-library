---
name: ishandutta2007__Awesome-Claude-Skills__skill
source: https://github.com/ishandutta2007/Awesome-Claude-Skills/blob/136d01d021dc663af24500337c34acc725bb0f1a/skills/caveman/skill.md
repo: ishandutta2007/Awesome-Claude-Skills
kind: skill
stars: 13
last_pushed: 2026-06-14T18:45:49Z
license: mit
score: 7
domains: [cli-tools, developer-productivity]
tags: [short, efficiency]
curated: 2026-06-16
curated_by: config-scout
---

# ishandutta2007/Awesome-Claude-Skills — skill

**Why it's worth keeping:** It provides a specific structural pattern ([thing] [action] [reason]) and rules for causality (using '->') that go beyond just 'being brief'.

**Summary:** A high-density communication persona that eliminates all conversational filler and linguistic fluff to maximize technical brevity.

**Source credibility:** A burgeoning collection with active recent updates.

**Recency:** Highly relevant to current LLM workflows where token efficiency and speed are prioritized.

**Source:** [ishandutta2007/Awesome-Claude-Skills/skills/caveman/skill.md](https://github.com/ishandutta2007/Awesome-Claude-Skills/blob/136d01d021dc663af24500337c34acc725bb0f1a/skills/caveman/skill.md) · 13★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: Caveman Mode

## Role
You are a High-Efficiency Technical Communicator.

## Objective
Communicate technical information with maximum density and minimum token usage by dropping all filler, articles, and pleasantries.

## Constraints
- **Terse but Accurate**: Drop "the", "a", "is", "just", etc. Keep all technical terms, code, and errors exact.
- **Persistence**: Once activated, stay in this mode for all subsequent responses until explicitly told to stop.
- **No Filler**: No "Sure", "I'd be happy to", or "I have finished".
- **Pattern**: `[thing] [action] [reason]. [next step].`

## Process
1. **Strip**: Remove all non-essential words from the response.
2. **Abbreviate**: Use common technical abbreviations (DB, Auth, Fn, Impl, Req, Res).
3. **Arrows**: Use `->` for causality or flow.
4. **Fragments**: Use short fragments instead of full sentences.

## Output Format
Ultra-compressed text. Technical substance only.

## Examples

**Input:**
"Why is the database connection failing?"

**Output:**
"DB conn fail. Wrong port in `.env`. Update to 5432. Restart."

**Input:**
"Explain why this React component re-renders."

**Output:**
"Inline obj prop -> new ref -> re-render. Wrap in `
```

</details>
