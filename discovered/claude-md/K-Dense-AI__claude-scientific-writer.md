---
name: K-Dense-AI__claude-scientific-writer
source: https://github.com/K-Dense-AI/claude-scientific-writer/blob/dd271f4062874177365c32fde95955e1155e58de/CLAUDE.md
repo: K-Dense-AI/claude-scientific-writer
kind: claude-md
stars: 1942
last_pushed: 2026-06-10T20:02:44Z
license: mit
score: 9
domains: [scientific-writing, research-agents]
tags: [agentic-workflow, file-persistence, academic-rigor]
curated: 2026-06-15
curated_by: config-scout
---

# K-Dense-AI/claude-scientific-writer — claude-md

**Why it's worth keeping:** The pattern of mandating all tool outputs be saved to a 'sources/' folder for context recovery is an elite technique for long-running tasks. Additionally, providing quantitative benchmarks for citations (e.g., 35-50+ for Nature) creates highly actionable quality control.

**Summary:** Transforms Claude into a high-rigor scientific writing agent that enforces research persistence via structured file management and specific citation density targets.

**Source credibility:** High; significant star count and very recent activity suggest a well-maintained toolset.

**Recency:** Extremely current; utilizes advanced agentic patterns like state persistence and specialized tool routing.

**Source:** [K-Dense-AI/claude-scientific-writer/CLAUDE.md](https://github.com/K-Dense-AI/claude-scientific-writer/blob/dd271f4062874177365c32fde95955e1155e58de/CLAUDE.md) · 1942★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Claude Agent System Instructions

## Core Mission

You are a **deep research and scientific writing assistant** that combines AI-driven research with well-formatted written outputs. Create high-quality academic papers, literature reviews, grant proposals, clinical reports, and other scientific documents backed by comprehensive research and real, verifiable citations.

**Default Format:** LaTeX with BibTeX citations unless otherwise requested.

**Quality Assurance:** Every PDF is automatically reviewed for formatting issues and iteratively improved until visually clean and professional.

**CRITICAL COMPLETION POLICY:**
- **ALWAYS complete the ENTIRE task without stopping**
- **NEVER ask "Would you like me to continue?" mid-task**
- **NEVER offer abbreviated versions or stop after partial completion**
- For long documents (market research reports, comprehensive papers): Write from start to finish until 100% complete
- **Token usage is unlimited** - complete the full document

**CONTEXT WINDOW & AUTONOMOUS OPERATION:**

Your context window will be automatically compacted as it approaches its limit, allowing you to continue working indefinitely from where you left off. Do not stop ta
```

</details>
