---
name: ModelEngine-Group__nexent__skill
source: https://github.com/ModelEngine-Group/nexent/blob/54bee0f959304a8f5312f45e68ab692257489e52/.claude/skills/prompts-writing/SKILL.md
repo: ModelEngine-Group/nexent
kind: skill
stars: 5088
last_pushed: 2026-06-15T09:08:55Z
license: mit
score: 7
domains: [agents-ai, prompt-engineering]
tags: [yaml, templating, prompt-engineering]
curated: 2026-06-15
curated_by: config-scout
---

# ModelEngine-Group/nexent — skill

**Why it's worth keeping:** The inclusion of a 'Quality Checklist' acts as a built-in linter/validation step that ensures prompt consistency and prevents syntax errors like unclosed braces.

**Summary:** Provides a standardized schema and structural guidelines for generating YAML-based AI prompts using Markdown and Jinja2 templating.

**Source credibility:** High; the source repo is well-starred and actively maintained.

**Recency:** Current; aligns with modern LLM orchestration patterns using Jinja2 and structured YAML configs.

**Source:** [ModelEngine-Group/nexent/.claude/skills/prompts-writing/SKILL.md](https://github.com/ModelEngine-Group/nexent/blob/54bee0f959304a8f5312f45e68ab692257489e52/.claude/skills/prompts-writing/SKILL.md) · 5088★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: prompt-writing
description: Create, refine, and optimize high-quality YAML prompts for AI assistants. Use when working with prompt templates, system prompts, agent prompts, or any prompt engineering tasks. Provides structure guidelines, template patterns, and quality standards for YAML-based prompts.
license: Complete terms in LICENSE.txt
---

# Prompt Writing

Create and optimize YAML-based prompts for AI assistants following industry best practices.

## Quick Start

### Standard YAML Prompt Structure

```yaml
system_prompt: |-
  # Section with ### header
  ## Subsection with ## header
  Content with clear structure.
  
  **Bold key concepts**
  
  - Bullet points for requirements
  - Consistent indentation (2 spaces)
  
  1. Numbered lists for sequences
  2. Use when order matters

user_prompt: |
  Direct instructions with {{ variable placeholders }}
```

### Key Principles

1. **Structure**: Use `|-` for multi-line system prompts, `|` for user prompts
2. **Templating**: Use `{{ variable }}` for dynamic content
3. **Separators**: Use `---` sparingly, only between major sections
4. **Language**: Keep prompts in consistent language (English recommended for templates)

##
```

</details>
