---
name: huggingface__skills__skill
source: https://github.com/huggingface/skills/blob/c68f1b08d9eb3af22cdc1d3fb60e9cdb78522556/skills/transformers-js/SKILL.md
repo: huggingface/skills
kind: skill
stars: 10667
last_pushed: 2026-06-12T09:25:39Z
license: apache-2.0
score: 9
domains: [machine-learning, web-frontend, javascript]
tags: [transformers-js, ml, onnx, webgpu]
curated: 2026-06-15
curated_by: config-scout
---

# huggingface/skills — skill

**Why it's worth keeping:** Includes critical production-ready details like memory management (pipe.dispose()) and quantization options. Provides specific, actionable code snippets for diverse tasks from NER to WebGPU acceleration.

**Summary:** Provides exhaustive patterns for implementing local machine learning in JavaScript using Transformers.js across various modalities.

**Source credibility:** Extremely high; official documentation/skill set from Hugging Face.

**Recency:** Very current; includes modern patterns for Gemma 3 and WebGPU usage.

**Source:** [huggingface/skills/skills/transformers-js/SKILL.md](https://github.com/huggingface/skills/blob/c68f1b08d9eb3af22cdc1d3fb60e9cdb78522556/skills/transformers-js/SKILL.md) · 10667★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: transformers-js
description: Use Transformers.js to run state-of-the-art machine learning models directly in JavaScript/TypeScript. Supports NLP (text classification, translation, summarization), computer vision (image classification, object detection), audio (speech recognition, audio classification), and multimodal tasks. Works in browsers and server-side runtimes (Node.js, Bun, Deno) with WebGPU/WASM using pre-trained models from Hugging Face Hub.
license: Apache-2.0
metadata:
  author: huggingface
  version: "4.x"
  category: machine-learning
  repository: https://github.com/huggingface/transformers.js
compatibility: Requires Node.js 18+ (or compatible Bun/Deno runtime) or modern browser with ES modules support. WebGPU requires runtime and hardware support; WASM is the broad fallback. Internet access is needed for downloading models from Hugging Face Hub (optional if using local models).
---

# Transformers.js - Machine Learning for JavaScript

Transformers.js enables running state-of-the-art machine learning models directly in JavaScript across browsers and server-side runtimes (Node.js, Bun, Deno), with no Python server required.

## When to Use This Skill

Use this
```

</details>
