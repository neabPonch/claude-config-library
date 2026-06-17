---
name: seethroughlab__vivid-opencv
source: https://github.com/seethroughlab/vivid-opencv/blob/b599c2d6c845d55bc350446793ee153e893d3f40/CLAUDE.md
repo: seethroughlab/vivid-opencv
kind: claude-md
stars: 0
last_pushed: 2026-01-14T14:18:11Z
license: mit
score: 9
domains: [computer-vision, cpp, systems-programming]
tags: [opencv, cmake, pimpl, build-system]
curated: 2026-06-16
curated_by: config-scout
---

# seethroughlab/vivid-opencv — claude-md

**Why it's worth keeping:** Includes explicit 'Task to File' mappings and specific code patterns that allow an AI agent to perform complex modifications without needing to guess the architecture.

**Summary:** Provides high-density technical context covering build processes, architectural patterns (PIMPL/Registration), and critical platform-specific ABI constraints.

**Source credibility:** Low social proof via stars, but content demonstrates high technical depth regarding MSVC/OpenCV integration.

**Recency:** Current; updated within the last 5 months.

**Source:** [seethroughlab/vivid-opencv/CLAUDE.md](https://github.com/seethroughlab/vivid-opencv/blob/b599c2d6c845d55bc350446793ee153e893d3f40/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# vivid-opencv

OpenCV computer vision module for Vivid. Builds OpenCV from source to avoid MSVC STL ABI issues on Windows.

## Build Commands

```bash
# Build with vivid SDK
cmake -B build -DVIVID_ROOT=/path/to/vivid-sdk
cmake --build build

# Build with tests
cmake -B build -DVIVID_ROOT=/path/to/vivid-sdk -DBUILD_TESTS=ON
cmake --build build
ctest --test-dir build
```

## Project Structure

```
vivid-opencv/
├── include/vivid/opencv/     # Public headers
│   ├── opencv.h              # Main include (all operators)
│   ├── contours.h            # Contour detection
│   ├── optical_flow.h        # Motion detection
│   ├── blob_track.h          # Blob tracking
│   └── export.h              # DLL export macros
├── src/                      # Implementation
│   ├── opencv.cpp            # Module entry point
│   ├── contours.cpp          # Contours operator + REGISTER_OPERATOR
│   ├── optical_flow.cpp      # OpticalFlow operator + REGISTER_OPERATOR
│   └── blob_track.cpp        # BlobTrack operator + REGISTER_OPERATOR
├── examples/                 # Runnable demos
│   ├── contours-webcam/
│   ├── contours-video/
│   ├── optical-flow/
│   └── blob-tracking/
├── .github/workflows/
```

</details>
