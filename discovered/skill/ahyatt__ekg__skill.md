---
name: ahyatt__ekg__skill
source: https://github.com/ahyatt/ekg/blob/fe4aa7e9574a73515824736e8ebfba81ee864a1d/agent_tools/skill.md
repo: ahyatt/ekg
kind: skill
stars: 284
last_pushed: 2026-05-18T00:25:28Z
license: gpl-3.0
score: 9
domains: [agents-ai, cli-tools, knowledge-management]
tags: [memory, emacs, org-mode, task-management]
curated: 2026-06-16
curated_by: config-scout
---

# ahyatt/ekg — skill

**Why it's worth keeping:** The 'Prompt Co-Tags' concept is a top-tier technique for agents to retrieve specialized instructions related to specific tools or workflows. The structured approach to task lifecycle (TODO/DONE) provides an excellent template for agentic state management.

**Summary:** A comprehensive skill for an Emacs-backed knowledge graph that manages long-term memory, task state via Org-mode, and context-specific instructions.

**Source credibility:** Strong; well-maintained Emacs project with significant community interest (284 stars).

**Recency:** Highly current; the patterns of semantic search and instruction injection are perfectly aligned with modern agentic needs.

**Source:** [ahyatt/ekg/agent_tools/skill.md](https://github.com/ahyatt/ekg/blob/fe4aa7e9574a73515824736e8ebfba81ee864a1d/agent_tools/skill.md) · 284★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ekg
description: "Use this skill to supplement memory - both looking for and using memory to understand how to do things, and the state of tasks."
model: inherit
---

# ekg Skill — Emacs Knowledge Graph

`ekg` is an Emacs package ([source](https://github.com/ahyatt/ekg)) for taking
and retrieving notes, backed by a `sqlite` database. It should be used as a form
of agent memory, and it may also be used by users for their notes as well.

Here's how to use it from the command-line. Each script calls `emacsclient` so
the user must have run `M-x server-start` on their emacs, as well as loaded the
`ekg` package.

## Setup: Locating the Scripts

The command-line scripts live in the `agent_tools/` directory of the `ekg`
package. Since Emacs packages aren't normally on `$PATH`, resolve the directory
at the start of any session by asking Emacs where ekg is installed:

```sh
EKG_DIR=$(emacsclient --eval '(file-name-directory (locate-library "ekg"))' | tr -d '"')
```

Then invoke scripts with their full path, e.g. `"$EKG_DIR/agent_tools/ekg-read"`.

Alternatively, if you prefer, you can add the directory to your `$PATH`:

```sh
export PATH="$EKG_DIR/agent_tools:$PATH"
```

## ekg-add
```

</details>
