---
name: artokun__comfyui-mcp__node-skill
source: https://github.com/artokun/comfyui-mcp/blob/561c3682237dcb95932d8542fdd2ac017e86ab77/plugin/commands/node-skill.md
repo: artokun/comfyui-mcp
kind: skill
stars: 152
last_pushed: 2026-06-13T23:47:07Z
license: mit
score: 8
domains: [agents-ai, cli-tools, automation]
tags: [meta-skill, comfyui, tool-generation, automation]
curated: 2026-06-14
curated_by: config-scout
---

# artokun/comfyui-mcp — skill

**Why it's worth keeping:** Demonstrates a 'meta-programming' pattern where one skill generates others to scale agent capabilities without manual documentation effort.

**Summary:** A meta-skill that automates the creation of new skill files for ComfyUI custom node packs via registry IDs or GitHub URLs.

**Source credibility:** Strong; 152 stars and recent activity suggest a highly useful, specialized tool for the ComfyUI ecosystem.

**Recency:** Current; aligns with modern Claude Code/MCP plugin patterns.

**Source:** [artokun/comfyui-mcp/plugin/commands/node-skill.md](https://github.com/artokun/comfyui-mcp/blob/561c3682237dcb95932d8542fdd2ac017e86ab77/plugin/commands/node-skill.md) · 152★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Generate a Claude skill for a ComfyUI custom node pack
argument-hint: Registry ID or GitHub URL of the node pack
---

# /comfy-skill — Generate a Node Pack Skill

The user wants to generate a Claude Code skill file for a ComfyUI custom node pack.

## Instructions

1. **Parse the argument.** The argument is: $ARGUMENTS
   - A ComfyUI Registry ID (e.g., `comfyui-impact-pack`)
   - A GitHub repository URL (e.g., `https://github.com/ltdrdata/ComfyUI-Impact-Pack`)
   - Nothing — ask the user which node pack they want to generate a skill for

2. **Generate the skill.** Use the `generate_node_skill` tool with:
   - `source`: the registry ID or GitHub URL
   - `install_in`: save to `skills/<pack-name>/` inside the plugin directory

3. **Report the result.** Tell the user:
   - Where the skill file was saved
   - A brief summary of what nodes are covered
   - That they may need to restart Claude Code for the skill to take effect

## Example

User: `/comfy-skill comfyui-impact-pack`

Steps:
- Call `generate_node_skill` with source `"comfyui-impact-pack"` and `install_in` set to the skills directory
- Show the user where the file was saved and what it covers

## Notes

- The
```

</details>
