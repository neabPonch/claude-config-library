---
name: huggingface__blog__upskill
source: https://github.com/huggingface/blog/blob/87a151e2b199304e3ddd28e8ce8f911f5b6f5517/upskill.md
repo: huggingface/blog
kind: skill
stars: 3443
last_pushed: 2026-06-15T14:32:45Z
license: unknown
score: 8
domains: [agents-ai, systems-programming, cuda, machine-learning]
tags: [upskilling, trace-to-skill, performance-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# huggingface/blog — skill

**Why it's worth keeping:** It details how to transform interactive execution traces into structured, validated skills that include project architecture and domain-specific optimizations.

**Summary:** Describes a methodology for 'upskilling' agents by using expert traces from high-end models to create specialized skill files for complex tasks like CUDA development.

**Source credibility:** High; published via the official Hugging Face blog with high community engagement.

**Recency:** Very current; discusses SOTA models like Claude Opus 4.5.

**Source:** [huggingface/blog/upskill.md](https://github.com/huggingface/blog/blob/87a151e2b199304e3ddd28e8ce8f911f5b6f5517/upskill.md) · 3443★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
title: "We Got Claude to Build CUDA Kernels and teach open models!"
thumbnail: /blog/assets/upskill/thumbnail.png
authors:
- user: burtenshaw
- user: evalstate
- user: merve
- user: pcuenq
---


# We got Claude to teach open models how to write CUDA kernels!

The best thing about agent skills is _upskilling_ your agents on hard problems. There are two ways to look at that: 
1. You can take Opus 4.5 or other SOTA models and tackle the hardest problems out there. 
2. You can take models that run on your laptop and upskill them to harder problems. In this blog post, we’ll show you how to take on the latter. 

This blog post walks through the process of using a new tool, `upskill`, to generate and evaluate agent skills with large models and use them with smaller models. We will benchmark `upskill` on the task of writing CUDA kernels for [`diffusers`](https://huggingface.co/docs/diffusers/en/index) models, but the process is generally useful for cutting costs, or using smaller models on hard and domain-specific problems. 

## What are agent skills?

In case you missed it, agent skills are taking the coding agent game by storm. In fact, they’re a straightforward concept to define mod
```

</details>
