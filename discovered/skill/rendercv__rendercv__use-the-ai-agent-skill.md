---
name: rendercv__rendercv__use-the-ai-agent-skill
source: https://github.com/rendercv/rendercv/blob/1d4b87bc427e4cf61c0ef49623c971b0e2224708/docs/user_guide/how_to/use_the_ai_agent_skill.md
repo: rendercv/rendercv
kind: skill
stars: 16881
last_pushed: 2026-05-01T00:11:29Z
license: mit
score: 9
domains: [cli-tools, automation, content-generation]
tags: [schema-driven, auto-generated, pydantic]
curated: 2026-06-15
curated_by: config-scout
---

# rendercv/rendercv — skill

**Why it's worth keeping:** It uses a sophisticated AST-driven pipeline to auto-generate its own documentation from Pydantic models, ensuring the skill never suffers from schema drift. It also includes a promptfoo evaluation suite for deterministic validation of agent outputs.

**Summary:** This skill provides an AI agent with the full YAML schema, CLI commands, and design configurations required to automate CV creation via RenderCV.

**Source credibility:** High; highly popular open-source project (16k+ stars) with active maintenance.

**Recency:** Very current, updated within the last few months.

**Source:** [rendercv/rendercv/docs/user_guide/how_to/use_the_ai_agent_skill.md](https://github.com/rendercv/rendercv/blob/1d4b87bc427e4cf61c0ef49623c971b0e2224708/docs/user_guide/how_to/use_the_ai_agent_skill.md) · 16881★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Use the AI Agent Skill

RenderCV provides an AI agent skill that teaches AI coding assistants how to create, edit, and render CVs. Once installed, your agent gains full knowledge of RenderCV's YAML schema, CLI commands, themes, locales, and design options.

## Supported Agents

The skill works with any AI agent that supports the [skills standard](https://skills.sh), including Claude Code, Claude Desktop, Cursor, Codex, Copilot, Windsurf, and Gemini CLI.

## Install the Skill

=== "Vercel Skills CLI"

    ```bash
    npx skills add rendercv/rendercv-skill
    ```

    You can also target a specific agent:

    ```bash
    npx skills add rendercv/rendercv-skill -a claude-code
    npx skills add rendercv/rendercv-skill -a cursor
    npx skills add rendercv/rendercv-skill -a codex
    ```

=== "OpenSkills"

    ```bash
    npx openskills install rendercv/rendercv-skill
    ```

=== "Claude Desktop"

    1. Download [`rendercv_skill.zip`](../../assets/rendercv_skill.zip).
    2. In Claude Desktop, click **Customize** (top left), then select **Skills**.
    3. Click **"+"** and select **"Upload a skill"**.
    4. Upload the downloaded ZIP file.

    The skill will appear in your Skills
```

</details>
