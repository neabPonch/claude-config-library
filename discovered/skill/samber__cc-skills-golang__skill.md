---
name: samber__cc-skills-golang__skill
source: https://github.com/samber/cc-skills-golang/blob/a5e0e5997aac169b659e70cb826a20b489bc4c6c/skills/golang-spf13-cobra/SKILL.md
repo: samber/cc-skills-golang
kind: skill
stars: 2139
last_pushed: 2026-06-09T13:53:57Z
license: mit
score: 9
domains: [cli-tools, golang]
tags: [cobra, go, cli]
curated: 2026-06-15
curated_by: config-scout
---

# samber/cc-skills-golang — skill

**Why it's worth keeping:** It uses highly effective 'Modes' (Build/Extend/Review) and emphasizes critical technical nuances like error-returning hooks and testable output redirection via command buffers.

**Summary:** A high-fidelity skill file for engineering Go CLI tools using the Cobra library, providing structured personas and operational modes.

**Source credibility:** High; source repository has significant stars and active, recent maintenance.

**Recency:** Current; aligns with modern Go development and agentic coding patterns.

**Source:** [samber/cc-skills-golang/skills/golang-spf13-cobra/SKILL.md](https://github.com/samber/cc-skills-golang/blob/a5e0e5997aac169b659e70cb826a20b489bc4c6c/skills/golang-spf13-cobra/SKILL.md) · 2139★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: golang-spf13-cobra
description: "Golang CLI command tree library using spf13/cobra — cobra.Command, RunE vs Run, PersistentPreRunE hook chain, Args validators (NoArgs, ExactArgs, MatchAll, custom), persistent vs local flags, command groups, ValidArgsFunction, RegisterFlagCompletionFunc, ShellCompDirective, usage/help template customization, man-page and markdown doc generation, and testing with SetArgs/SetOut/SetErr. Apply when using or adopting spf13/cobra, or when the codebase imports `github.com/spf13/cobra`. For configuration layering alongside cobra, see the `samber/cc-skills-golang@golang-spf13-viper` skill. For general CLI architecture (project layout, exit codes, signal handling, I/O patterns), see `samber/cc-skills-golang@golang-cli`."
user-invocable: true
license: MIT
compatibility: Designed for Claude Code or similar AI coding agents, and for projects using Golang.
metadata:
  author: samber
  version: "1.0.1"
  openclaw:
    emoji: "🐍"
    homepage: https://github.com/samber/cc-skills-golang
    requires:
      bins:
        - go
    install: []
    skill-library-version: "1.10.2"
allowed-tools: Read Edit Write Glob Grep Bash(go:*) Bash(golangci-lint:*) Bash(g
```

</details>
