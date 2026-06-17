---
name: Yusong-Enceladus__claude-skills__skill
source: https://github.com/Yusong-Enceladus/claude-skills/blob/007b57180e0fd2618ade26a6511708ef7da1f344/preflight-hpc/skill.md
repo: Yusong-Enceladus/claude-skills
kind: skill
stars: 8
last_pushed: 2026-03-18T08:23:27Z
license: unknown
score: 8
domains: [hpc, ai-research, devops]
tags: [slurm, gpu, validation, mujoco]
curated: 2026-06-16
curated_by: config-scout
---

# Yusong-Enceladus/claude-skills — skill

**Why it's worth keeping:** Includes high-value, specific verification logic like EGL rendering tests and HuggingFace connectivity checks that are difficult to debug manually.

**Summary:** Automates environmental validation for HPC clusters to prevent failed SLURM jobs by checking GPU status, network reachability, and library compatibility.

**Source credibility:** Low star count but highly specialized/expert content specific to ML research workflows.

**Recency:** Current; aligns perfectly with modern agentic tool use for environment auditing.

**Source:** [Yusong-Enceladus/claude-skills/preflight-hpc/skill.md](https://github.com/Yusong-Enceladus/claude-skills/blob/007b57180e0fd2618ade26a6511708ef7da1f344/preflight-hpc/skill.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: preflight-hpc
description: "Validate HPC environment before experiment deployment. Checks GPU, rendering, network, dependencies, and model loading. Use before submitting SLURM jobs."
argument-hint: [server-name]
allowed-tools: Bash(*), Read, Write
---

# Pre-flight HPC Validation

Validate compute environment on: **$ARGUMENTS**

## Checks

### 1. Connectivity
```bash
ssh $SERVER "echo 'SSH OK'; hostname; nvidia-smi -L | head -2"
```

### 2. GPU Availability
```bash
ssh $SERVER "nvidia-smi --query-gpu=index,name,memory.used,memory.total --format=csv,noheader"
```

### 3. Network (proxy detection)
```bash
ssh $SERVER "env | grep -i proxy; curl -s --max-time 5 https://huggingface.co > /dev/null 2>&1 && echo 'HF reachable' || echo 'HF BLOCKED — set HF_HUB_OFFLINE=1'"
```

### 4. Conda Environment
```bash
ssh $SERVER "conda activate <your-conda-env> 2>/dev/null && python -c 'import torch; print(f\"PyTorch {torch.__version__}, CUDA: {torch.cuda.is_available()}\")'"
```

### 5. Rendering (for robotics)
```bash
ssh $SERVER "srun --gres=gpu:1 --time=5:00 --partition=<your-partition> bash -c '
export MUJOCO_GL=egl
python -c \"
import mujoco
m = mujoco.MjModel.from_xml_string(chr(60
```

</details>
