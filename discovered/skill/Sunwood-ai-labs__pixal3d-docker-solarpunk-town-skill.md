---
name: Sunwood-ai-labs__pixal3d-docker-solarpunk-town-skill
source: https://github.com/Sunwood-ai-labs/pixal3d-docker-solarpunk-town-skill/blob/e7270fa5461b15762540dcd198ffd7859926c569/Skill.md
repo: Sunwood-ai-labs/pixal3d-docker-solarpunk-town-skill
kind: skill
stars: 3
last_pushed: 2026-05-17T06:55:10Z
license: other
score: 9
domains: [cli-tools, computer-vision, 3d-generation, automation]
tags: [image-to-3d, docker, blender, workflow-automation]
curated: 2026-06-14
curated_by: config-scout
---

# Sunwood-ai-labs/pixal3d-docker-solarpunk-town-skill — skill

**Why it's worth keeping:** It excels at documenting 'gotchas' like the Windows Blender launcher workaround, provides rigorous verification steps (file size checks), and includes a structured reporting protocol for agentic reliability.

**Summary:** A highly specialized skill for managing a local Dockerized image-to-3D generation pipeline and integrating assets into Blender. It covers everything from environment variable configuration to complex OS-specific software execution.

**Source credibility:** A niche repository with high-quality, manual technical documentation despite low star count.

**Recency:** Highly current; follows modern Docker Compose and local environment patterns.

**Source:** [Sunwood-ai-labs/pixal3d-docker-solarpunk-town-skill/Skill.md](https://github.com/Sunwood-ai-labs/pixal3d-docker-solarpunk-town-skill/blob/e7270fa5461b15762540dcd198ffd7859926c569/Skill.md) · 3★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: pixal3d-image-to-3d
description: Generate 3D GLB models from input images with the Pixal3D Docker workflow in this repository. Use when Codex needs to convert PNG/JPG/WebP images into Pixal3D 3D assets, run the Gradio Pixal3D app, inspect or serve generated GLB outputs, batch-convert solarpunk town assets, tune FOV/background-removal settings, or troubleshoot Docker/NVIDIA/Hugging Face cache issues for Pixal3D image-to-3D generation.
---

# Pixal3D Image-to-3D

Use this skill to turn an image into a GLB model with the local Pixal3D Docker setup in this repository.
Also use it when arranging the generated assets into the Blender solarpunk town world under `outputs/generated_game_assets/workfiles/`.

## Repository Assumptions

- Work from the repository root: `D:\Prj\pixal3d-docker-solarpunk-town`.
- Use Docker Compose as the primary runtime. The `pixal3d` service runs `inference.py`.
- Expect NVIDIA GPU support through Docker. If GPU access is unavailable, stop and report that Pixal3D generation cannot run in this setup.
- Keep generated assets under `outputs/generated_game_assets/` unless the user requests another location.
- Keep source images under `assets/generated_gam
```

</details>
