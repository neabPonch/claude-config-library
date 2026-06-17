---
name: nawodyaishan__ar-fashion-tryon__claude
source: https://github.com/nawodyaishan/ar-fashion-tryon/blob/4f89a17e4d87ffdfc8db909328646769c6d49db6/garment-processing-api/CLAUDE.md
repo: nawodyaishan/ar-fashion-tryon
kind: claude-md
stars: 8
last_pushed: 2026-06-08T01:17:15Z
license: mit
score: 9
domains: [backend-api, machine-learning, computer-vision]
tags: [fastapi, api-spec, microservice, mlops]
curated: 2026-06-15
curated_by: config-scout
---

# nawodyaishan/ar-fashion-tryon — claude-md

**Why it's worth keeping:** The inclusion of specific `curl` examples for every endpoint and detailed request flow diagrams provides highly actionable ground truth for debugging and feature development.

**Summary:** This file acts as a comprehensive technical manual, providing deep architectural context and complete API documentation. It enables Claude to understand not just how to run the code, but exactly how the data pipeline and business logic function.

**Source credibility:** High-quality documentation from a specialized AI/ML project.

**Recency:** Very recent, utilizing modern Python tooling like `uv`.

**Source:** [nawodyaishan/ar-fashion-tryon/garment-processing-api/CLAUDE.md](https://github.com/nawodyaishan/ar-fashion-tryon/blob/4f89a17e4d87ffdfc8db909328646769c6d49db6/garment-processing-api/CLAUDE.md) · 8★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This is a **FastAPI-based garment extraction and virtual try-on microservice** that classifies clothing items, removes backgrounds, constructs full outfits, and performs AI-powered virtual try-on using machine learning. It uses **Cloudinary for image storage** and **Gradio API (CatVTON) for virtual try-on**, making it suitable for cloud deployment.

**Core functionality:**
- **Classification**: TensorFlow CNN model identifies garment type (T-shirt, Trousers, or Other)
- **Background Removal**: Uses rembg (u2net model) to create transparent cutouts
- **Outfit Construction**: Merges upper + lower garments from cutouts (transparent backgrounds)
- **Virtual Try-On**: Integrates with Gradio Space (CatVTON) for realistic garment visualization
- **Cloud Storage**: Uploads originals, cutouts, and try-on results to Cloudinary
- **Dual Input Methods**: Accepts file uploads or image URLs

## Quick Start

### Installation

```bash
# Install dependencies
uv sync
```

### Environment Setup

**Required environment variables:**
```bash
# Cloudinary credentials (REQUIRED
```

</details>
