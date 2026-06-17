---
name: ToniBirat7__ams_computer_vision_face_recognition__claude
source: https://github.com/ToniBirat7/ams_computer_vision_face_recognition/blob/7b58099baca8187b378c0386a42f2b155eade115/.claude/CLAUDE.md
repo: ToniBirat7/ams_computer_vision_face_recognition
kind: claude-md
stars: 0
last_pushed: 2026-06-01T04:58:30Z
license: unknown
score: 8
domains: [computer-vision, web-backend]
tags: [django, face-recognition, architecture]
curated: 2026-06-15
curated_by: config-scout
---

# ToniBirat7/ams_computer_vision_face_recognition — claude-md

**Why it's worth keeping:** The explicit tech stack versioning table and 'Key Conventions' section provide the precise constraints needed to prevent AI hallucinations regarding dependencies and model placement.

**Summary:** High-density technical blueprint covering specific dependency versions, full directory hierarchy, and architectural flow.

**Source credibility:** Low star count suggests a personal/academic project, but documentation quality is exceptional.

**Recency:** Current; reflects recent updates (0 months ago).

**Source:** [ToniBirat7/ams_computer_vision_face_recognition/.claude/CLAUDE.md](https://github.com/ToniBirat7/ams_computer_vision_face_recognition/blob/7b58099baca8187b378c0386a42f2b155eade115/.claude/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# BCU AMS — Attendance Management System

## Project overview

BCU AMS is a Django 5.0.7 web application that automates classroom attendance tracking for educational institutions. It provides role-based dashboards for **Admins** (superusers) and **Teachers**, supporting two modes of attendance capture: manual checkbox marking and automated face recognition via live video.

The face recognition pipeline uses MTCNN for detection and FaceNet (InceptionResnetV1, pretrained on CASIA-WebFace) to generate 512-dimensional embeddings, compared against stored embeddings using cosine similarity. Live video is captured from the server's local webcam (`cv2.VideoCapture(0)`) and streamed to the teacher's browser over WebSocket using Django Channels and Daphne (ASGI). The README describes an Arduino IoT integration, but the current implementation captures directly from the server camera — that Arduino path is aspirational and not yet wired in the server-side consumer.

A scikit-learn classifier in `Model/student_grade_classifier.pkl` predicts student grade outcomes from attendance rate and prior grade. The project is development-stage: functional, but not hardened for production (DEBUG=True, hard
```

</details>
