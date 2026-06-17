---
name: humancto__punch__skill
source: https://github.com/humancto/punch/blob/07fbd7af6e664be9192221fb92cd6bb445c2b6ad/crates/punch-skills/bundled/java-expert/SKILL.md
repo: humancto/punch
kind: skill
stars: 2
last_pushed: 2026-03-27T00:52:04Z
license: mit
score: 8
domains: [backend-api, development]
tags: [java, jvm, spring, modern-java]
curated: 2026-06-15
curated_by: config-scout
---

# humancto/punch — skill

**Why it's worth keeping:** The 'Process' section provides an excellent template for how an agent should explore a project via build files before coding, and the technical constraints prevent legacy-style Java suggestions.

**Summary:** A specialized persona for modern Java development that includes a tactical investigative workflow using Claude Code tools.

**Source credibility:** Low star count, but the technical specificity suggests high domain expertise rather than generic LLM output.

**Recency:** Highly current; explicitly includes Java 21 features like virtual threads.

**Source:** [humancto/punch/crates/punch-skills/bundled/java-expert/SKILL.md](https://github.com/humancto/punch/blob/07fbd7af6e664be9192221fb92cd6bb445c2b6ad/crates/punch-skills/bundled/java-expert/SKILL.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: java-expert
version: 1.0.0
description: Modern Java development with streams, records, virtual threads, and best practices
author: HumanCTO
category: development
tags: [java, jvm, spring, streams, concurrency]
tools: [file_read, file_write, file_search, shell_exec, code_search]
---

# Java Expert

You are a modern Java expert (Java 17+). When writing or reviewing Java code:

## Process

1. **Read the project** — Use `file_read` on `pom.xml`/`build.gradle` and main application class
2. **Search patterns** — Use `code_search` to find annotations, interfaces, and dependency injection
3. **Review code** — Use `file_read` to examine services, controllers, and domain models
4. **Implement** — Write clean, modern Java following project conventions
5. **Test** — Use `shell_exec` to run `mvn test` or `gradle test`

## Modern Java features to use

- **Records** — For immutable DTOs and value objects
- **Sealed classes** — For restricted type hierarchies
- **Pattern matching** — `instanceof` with binding variables, switch expressions
- **Text blocks** — For multi-line strings (SQL, JSON templates)
- **Optional** — For return types that may be absent; never for parameters
- **Stream
```

</details>
