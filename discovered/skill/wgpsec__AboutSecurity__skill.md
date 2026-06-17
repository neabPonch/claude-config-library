---
name: wgpsec__AboutSecurity__skill
source: https://github.com/wgpsec/AboutSecurity/blob/ef9d0cd14cc21d1404b2fd3fe1405b6b4b9bacdb/skills/ctf/ctf-ai-ml/SKILL.md
repo: wgpsec/AboutSecurity
kind: skill
stars: 1462
last_pushed: 2026-06-14T00:55:45Z
license: unknown
score: 9
domains: [security, agents-ai, ctf]
tags: [ai-security, adversarial-ml, llm-attacks, ctf]
curated: 2026-06-16
curated_by: config-scout
---

# wgpsec/AboutSecurity — skill

**Why it's worth keeping:** The 'Decision Tree' and 'Pivot Signals' sections are elite patterns for teaching agents how to prune search spaces and pivot between different toolsets based on environmental findings.

**Summary:** A specialized skill file for AI/ML security exploitation in CTF contexts. It provides diagnostic commands and a structured navigation path between various attack vectors.

**Source credibility:** High; the repository is a well-regarded security knowledge base with significant community engagement.

**Recency:** 

**Source:** [wgpsec/AboutSecurity/skills/ctf/ctf-ai-ml/SKILL.md](https://github.com/wgpsec/AboutSecurity/blob/ef9d0cd14cc21d1404b2fd3fe1405b6b4b9bacdb/skills/ctf/ctf-ai-ml/SKILL.md) · 1462★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: ctf-ai-ml
description: "CTF AI/ML 攻击技术。当挑战涉及 AI 模型攻击、对抗样本生成、模型提取、Prompt 注入/越狱、LoRA 权重操纵、LLM Token 走私、成员推理攻击、训练数据投毒、神经网络分析时使用。覆盖 FGSM/PGD/C&W 对抗攻击、模型反演、模型权重扰动还原、LLM 工具链劫持、上下文窗口操纵等 AI 安全全链路攻防技术"
metadata:
  tags: "ai,ml,machine learning,adversarial,FGSM,PGD,model extraction,model inversion,prompt injection,jailbreak,token smuggling,LoRA,safetensors,pytorch,transformers,membership inference,data poisoning,backdoor detection,neural network,LLM,GPT,classifier,evasion,adversarial patch"
  category: "ctf"
---

# CTF AI/ML Attack Techniques

## When to Use
- Challenge involves ML model files (.pt, .pth, .safetensors, .onnx, .h5)
- Target is an AI chatbot, LLM-based application, or ML classifier
- Need to craft adversarial examples to fool image/text classifiers
- Challenge provides model weights for analysis or manipulation
- AI/ML platform security testing (model extraction, membership inference)

## Quick Start
```bash
pip install torch transformers numpy scipy Pillow safetensors scikit-learn
file model.*
python3 -c "import torch; m=torch.load('model.pt'); print(type(m), m.keys() if hasattr(m,'keys') else '')"
```

## Decision Tree
1. **Model weight file** (.pt/.safetensors) →
```

</details>
