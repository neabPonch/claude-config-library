---
name: applerom__agent1st__why-terraform-skill
source: https://github.com/applerom/agent1st/blob/b1d1f587982f0b102181ca315ebd1bd22465bbf7/.agents/skills/terraform/why-terraform-skill.md
repo: applerom/agent1st
kind: skill
stars: 20
last_pushed: 2026-06-12T18:13:42Z
license: mit
score: 9
domains: [devops, terraform, ai-agents, infrastructure-as-code]
tags: [attention-engineering, cost-modeling, tf-best-practices]
curated: 2026-06-15
curated_by: config-scout
---

# applerom/agent1st — skill

**Why it's worth keeping:** It derives rules from transformer mechanics, such as using code-level validations (preconditions) instead of prose to ensure constraints survive context truncation and treat names as semantic vectors for better retrieval.

**Summary:** A meta-protocol that redefines Terraform best practices by treating LLM attention as a finite resource rather than human working memory.

**Source credibility:** High; uses specific research citations (Anthropic/Chroma) to back its engineering-led approach to agentic workflows.

**Recency:** Very current; addresses modern transformer attention limitations and stateful infrastructure management.

**Source:** [applerom/agent1st/.agents/skills/terraform/why-terraform-skill.md](https://github.com/applerom/agent1st/blob/b1d1f587982f0b102181ca315ebd1bd22465bbf7/.agents/skills/terraform/why-terraform-skill.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Why This Skill Looks the Way It Does

Companion to [`SKILL.md`](SKILL.md). Read once — when you want to understand
the rules instead of just following them. It is not needed at runtime: the
skill is self-sufficient, and reloading this file on every task would violate
the very attention budget it explains.

## The one-sentence version

Best practices encode cost assumptions; agents changed the costs; this skill
re-derives Terraform practice from the new costs instead of inheriting answers
to questions nobody is asking anymore.

## Best practices are compressed cost models

Every "best practice" is a stored answer to the question "what is expensive
here?"

- DRY answers: hand-writing and hand-synchronizing code is expensive.
- Deep module hierarchies answer: human working memory is small — hide detail behind interfaces.
- Workspaces answer: maintaining duplicate directories by hand felt wasteful.
- Constraints-in-the-wiki answers: enforcement code is tedious; prose is quick.

These were correct answers — for human costs.

An agent authoring and operating Terraform has a different cost vector:

- **writing is nearly free** — generation is the native motion of the model
- **attention
```

</details>
