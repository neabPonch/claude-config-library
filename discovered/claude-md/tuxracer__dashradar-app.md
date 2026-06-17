---
name: tuxracer__dashradar-app
source: https://github.com/tuxracer/dashradar-app/blob/0aafa57d8161533bf4439985713a236bab8f50f4/CLAUDE.MD
repo: tuxracer/dashradar-app
kind: claude-md
stars: 0
last_pushed: 2026-02-21T07:46:39Z
license: unknown
score: 7
domains: [web-frontend, computer-vision]
tags: [nextjs, typescript, tensorflow, pwa]
curated: 2026-06-15
curated_by: config-scout
---

# tuxracer/dashradar-app — claude-md

**Why it's worth keeping:** The 'Working with AI Assistants' section provides high-value mapping of common domain tasks to specific files and constants, which drastically reduces LLM guesswork during refactors.

**Summary:** This file excels at explaining complex logic flows—such as the interaction between TensorFlow, RxJS observables, and canvas rendering—and providing clear instructions for AI-driven tasks.

**Source credibility:** A niche personal project with low social proof but a very well-structured documentation style.

**Recency:** Current; follows the highly effective pattern of guiding AI through logic flows rather than just listing dependencies.

**Source:** [tuxracer/dashradar-app/CLAUDE.MD](https://github.com/tuxracer/dashradar-app/blob/0aafa57d8161533bf4439985713a236bab8f50f4/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.MD - DashRadar App

## Project Overview

**DashRadar** is a Next.js web application that provides real-time object detection using a webcam feed. The app uses TensorFlow.js with the COCO-SSD model to identify objects in the camera view and provides audio feedback through text-to-speech capabilities.

**Status**: Early prototype / Proof of concept - code needs cleanup

**Key Features**:
- Real-time object detection via webcam
- TensorFlow.js COCO-SSD model integration
- Text-to-speech announcements for detected objects
- Visual overlay with emoji representations
- Dark mode support

## Tech Stack

- **Framework**: Next.js 12.3.1
- **Runtime**: React 18.2.0
- **Language**: TypeScript 4.8.4
- **ML/AI**:
  - @tensorflow/tfjs ^4.0.0
  - @tensorflow-models/coco-ssd ^2.2.2
- **UI**: @nextui-org/react ^1.0.0-beta.12
- **Additional Features**:
  - Text-to-speech: tesseract.js ^3.0.3
  - PWA support: next-pwa ^5.6.0
  - Analytics: fathom-client ^3.5.0
  - State management: RxJS ^7.8.0

## Project Structure

```
.
├── components/          # React components
│   └── Loading/        # Loading component
├── lib/                # Core utilities
│   ├── tf.ts          # TensorFlow detecti
```

</details>
