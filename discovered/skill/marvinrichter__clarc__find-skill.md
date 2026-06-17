---
name: marvinrichter__clarc__find-skill
source: https://github.com/marvinrichter/clarc/blob/a8355b036a977300dfce1758af1c0d7e3371a26b/commands/find-skill.md
repo: marvinrichter/clarc
kind: skill
stars: 10
last_pushed: 2026-06-15T15:11:41Z
license: mit
score: 7
domains: [cli-tools, knowledge-management, agents-ai]
tags: [search, meta-skill, discovery]
curated: 2026-06-15
curated_by: config-scout
---

# marvinrichter/clarc — skill

**Why it's worth keeping:** Uses efficient shell scripting (grep/awk) to extract metadata from flat files for rapid discovery. It treats local knowledge as an indexable toolset rather than just static text.

**Summary:** Provides a command to search a local directory of structured Markdown skill files by keyword and displays their descriptions/activation criteria.

**Source credibility:** Small-scale but highly active project focusing on specialized agent workflows.

**Recency:** Highly current; utilizes standard shell commands compatible with modern CLI environments.

**Source:** [marvinrichter/clarc/commands/find-skill.md](https://github.com/marvinrichter/clarc/blob/a8355b036a977300dfce1758af1c0d7e3371a26b/commands/find-skill.md) · 10★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
description: Search all available skills by keyword and return the top matches with their descriptions. Use when unsure which skill covers a topic.
---

# Find Skill

Search the skills library by keyword. Returns the top matching skills with descriptions and activation criteria.

## Usage

```
/find-skill <keyword or topic>
```

## Examples

```
/find-skill jwt auth
/find-skill postgres query optimization
/find-skill react state
/find-skill go testing mocks
/find-skill api design versioning
```

## Workflow

Run this Bash command to search:

```bash
QUERY="$ARGUMENTS"
SKILLS_DIR="${CLAUDE_PLUGIN_ROOT:-$HOME/.claude}/skills"

echo "Searching skills for: $QUERY"
echo "---"

grep -rl --include="SKILL.md" -i "$QUERY" "$SKILLS_DIR" 2>/dev/null \
  | while read -r file; do
      dir=$(dirname "$file")
      name=$(basename "$dir")
      desc=$(grep -m1 '^description:' "$file" | sed 's/^description: *//;s/^"//;s/"$//')
      when=$(awk '/^## When to (Activate|Use)/,/^##/' "$file" | grep '^- ' | head -3 | sed 's/^- /  • /')
      echo "[$name]"
      echo "  $desc"
      if [ -n "$when" ]; then
        echo "  When to use:"
        echo "$when"
      fi
      echo ""
    done \
  | hea
```

</details>
