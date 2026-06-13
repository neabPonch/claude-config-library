# Advisor

The advisor is the "choose your own adventure" layer of this library. It takes a project description and outputs a composed, ready-to-use config set.

## Two modes

### Mode 1: Claude Code in-repo (best)

```bash
cd claude-config-library
claude
```

Ask: *"I'm building X with Y stack. Generate my CLAUDE.md and skills."*

The repo's `CLAUDE.md` instructs Claude to act as advisor, read the catalog, and compose a tailored output.

### Mode 2: Standalone prompt

Use [`prompts/advisor.md`](prompts/advisor.md) — paste it into any Claude session. It's self-contained and doesn't require this repo to be open.

## Files

| File | Purpose |
|------|---------|
| `prompts/advisor.md` | Standalone advisor prompt (paste into Claude) |
| `prompts/questionnaire.md` | Structured questions the advisor asks |
| `output-templates/` | Skeleton output formats for common project types |

## Adding output templates

If a project type is common enough to have a pre-baked starting point (e.g., "Next.js SaaS"), add a template to `output-templates/[name].md`. The advisor will prefer pre-baked templates over full composition when a good match exists.
