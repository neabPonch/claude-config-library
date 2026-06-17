---
name: adbc-drivers__databricks__claude
source: https://github.com/adbc-drivers/databricks/blob/48a3beb2bbcc1da9d2b2b839ab51b2afc3fcc209/csharp/CLAUDE.md
repo: adbc-drivers/databricks
kind: claude-md
stars: 7
last_pushed: 2026-06-12T16:02:50Z
license: apache-2.0
score: 9
domains: [database-drivers, dotnet, systems-programming]
tags: [architecture-map, build-instructions, performance-tuning]
curated: 2026-06-16
curated_by: config-scout
---

# adbc-drivers/databricks — claude-md

**Why it's worth keeping:** The hierarchy-to-file-path mapping is excellent, and the 'Important Implementation Details' section provides the exact type of reasoning required to prevent regression during refactoring.

**Summary:** Provides high-context architectural mapping and specific build/test commands essential for navigating complex driver logic. It includes critical implementation 'nuances' that prevent an AI from accidentally optimizing away carefully tuned constants.

**Source credibility:** High; part of a legitimate Apache-licensed driver project with active maintenance.

**Recency:** Very current; explicitly references modern Claude Code workflows.

**Source:** [adbc-drivers/databricks/csharp/CLAUDE.md](https://github.com/adbc-drivers/databricks/blob/48a3beb2bbcc1da9d2b2b839ab51b2afc3fcc209/csharp/CLAUDE.md) · 7★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
<!--
Copyright (c) 2025 ADBC Drivers Contributors

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
-->

# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This repository contains ADBC (Apache Arrow Database Connectivity) drivers for Databricks, implemented in C#. The driver is built on top of the Apache Spark ADBC driver and provides Databricks-specific functionality including OAuth authentication, CloudFetch for high-performance result retrieval, and comprehensive Databricks SQL support.

## Building and Testing

### C# Driver

The C# implementation is located in the `csharp/` directory. Build and test using standard .NET commands:
```

</details>
