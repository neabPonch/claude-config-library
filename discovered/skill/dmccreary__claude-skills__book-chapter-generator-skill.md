---
name: dmccreary__claude-skills__book-chapter-generator-skill
source: https://github.com/dmccreary/claude-skills/blob/b6d1be9817ffbfdca74cc79a6f21575d82012622/docs/prompts/book-chapter-generator-skill.md
repo: dmccreary/claude-skills
kind: skill
stars: 74
last_pushed: 2026-06-10T18:04:50Z
license: unknown
score: 8
domains: [content-automation, cli-tools]
tags: [meta-prompting, workflow-orchestration, file-system]
curated: 2026-06-16
curated_by: config-scout
---

# dmccreary/claude-skills — skill

**Why it's worth keeping:** It demonstrates how to enforce complex logical constraints like topological sorting (dependency management) and strict schema enforcement for file system creation.

**Summary:** A meta-prompt designed to create a specialized skill that transforms learning data into a structured book/course directory hierarchy.

**Source credibility:** Strong; the repository shows active maintenance and significant community interest via star count.

**Recency:** Current; follows modern agentic pattern-of-thought for structured tool use.

**Source:** [dmccreary/claude-skills/docs/prompts/book-chapter-generator-skill.md](https://github.com/dmccreary/claude-skills/blob/b6d1be9817ffbfdca74cc79a6f21575d82012622/docs/prompts/book-chapter-generator-skill.md) · 74★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Prompt to Create a Chapter Generator

!!! prompt
    Use the skill-creator skill to create a new skill called `book-chapter-generator`.
    This skill will look at the following resources:

    ## Input Resources
    1. Course Description at /docs/course-description.md
    2. Learning Graph at /docs/learning-graph/learning-graph.json
    3. Concept Taxonomy at /docs/learning-graph/concept-taxonomy.md

    ## Step 1: Design Chapters

    It will then suggest an outline of about 12 chapters for this book assuming you have about 200 concepts to cover.
    Each chapter will have a Chapter Title in Title Case and be no longer than 200 characters long.
    This is so that the listing of the chapters can fit on a single line per chapter.
    Use the course description and the learning graph to make sure that

    1. Each concept is covered once
    2. No concept is introduced before its dependencies are covered
    3. No chapter contains too many or two few concepts

    You may, at your discretion have as few as six chapters, or as many as 20 chapters.

    ## Step 2: Present Chapter Design to the User

    Present a simple list of Chapter Titles to the user.  Only present the
    Chap
```

</details>
