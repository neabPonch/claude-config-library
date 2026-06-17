---
name: dcmjs-org__dcmjs__asyncdicomreader-skill
source: https://github.com/dcmjs-org/dcmjs/blob/81e7e11cdefb56aa1a65bfe259648b865583ff88/docs/AsyncDicomReader-skill.md
repo: dcmjs-org/dcmjs
kind: skill
stars: 346
last_pushed: 2026-06-10T17:29:40Z
license: mit
score: 8
domains: [medical-imaging, data-parsing, javascript]
tags: [dicom, binary-streaming, memory-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# dcmjs-org/dcmjs — skill

**Why it's worth keeping:** It provides specific mental models for memory management through buffer clearing and explains the listener pattern required to handle fragmented binary data.

**Summary:** A technical deep-dive into the AsyncDicomReader for parsing large medical imaging files using streaming and listeners.

**Source credibility:** High; derived from dcmjs, a specialized library for DICOM manipulation.

**Recency:** Current; uses modern async/await patterns suitable for contemporary JavaScript environments.

**Source:** [dcmjs-org/dcmjs/docs/AsyncDicomReader-skill.md](https://github.com/dcmjs-org/dcmjs/blob/81e7e11cdefb56aa1a65bfe259648b865583ff88/docs/AsyncDicomReader-skill.md) · 346★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AsyncDicomReader Skill Guide

## Overview

The `AsyncDicomReader` is an asynchronous binary DICOM file reader that provides streaming capabilities for parsing DICOM files. It's designed to handle
large DICOM files efficiently by reading and processing data incrementally rather than loading entire files into memory at once.

## Key Features

- **Asynchronous/Streaming**: Reads DICOM files incrementally using async/await patterns
- **Memory Efficient**: Uses buffer streaming with automatic clearing to reduce memory footprint
- **Multiple Transfer Syntaxes**: Supports Explicit Little Endian, Explicit Big Endian, and Implicit Little Endian as well as compressed syntaxes.
- **Pixel Data Handling**: Handles both compressed and uncompressed pixel data
- **Sequence Support**: Properly parses DICOM sequences with defined and undefined lengths
- **Character Set Support**: Automatically handles different character encodings, but not multiple character encodings.
- **Error Handling**: Configurable error handling for malformed files

## Current Limitations

- Files must contain the standard DICM preamble
- Interface is preliminary and subject to change

## Basic Usage

### Reading a Complete
```

</details>
