---
name: h2oai__h2o-3
source: https://github.com/h2oai/h2o-3/blob/1676df7c04a6ea7a2f4cdf0f37be0783df7d7527/CLAUDE.md
repo: h2oai/h2o-3
kind: claude-md
stars: 7492
last_pushed: 2026-06-14T17:58:13Z
license: apache-2.0
score: 10
domains: [machine-learning, distributed-systems, java, backend]
tags: [architecture-patterns, distributed-computing, ml-platform]
curated: 2026-06-14
curated_by: config-scout
---

# h2oai/h2o-3 — claude-md

**Why it's worth keeping:** It defines the system's 'mental model' rather than just commands, teaching the AI how to reason about distributed data and where to avoid breaking core dependencies.

**Summary:** Provides deep architectural context for a distributed ML platform, including data distribution models (DKV/MRTask) and specific implementation patterns.

**Source credibility:** High; H2O is a major industry-standard open-source ML platform with active maintenance.

**Recency:** Current; contains detailed, modern Gradle/CI workflow instructions.

**Source:** [h2oai/h2o-3/CLAUDE.md](https://github.com/h2oai/h2o-3/blob/1676df7c04a6ea7a2f4cdf0f37be0783df7d7527/CLAUDE.md) · 7492★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build Commands

### Quick Build (Skip Tests)
```bash
./gradlew --parallel clean build -x test
# Or use the Makefile shortcut:
make
```

### Full Build (With Tests)

Most probably cannot run on laptop.

```bash
./gradlew syncSmalldata    # Download test data from S3
./gradlew build
```

### Run H2O Locally
```bash
java -jar build/h2o.jar
# Access UI at http://localhost:54321
```

## Testing

### Java Tests
H2O uses a custom multi-node testing framework (not standard JUnit runners):

- **Single-node cluster tests**: `./gradlew :h2o-algos:testSingleNode`
- **Multi-node cluster tests**: `./gradlew :h2o-algos:testMultiNode`
- **Single JVM tests**: `./gradlew :h2o-algos:testSingleNodeOneProc`

Test files are located in:
- `h2o-core/src/test/java/` - Platform tests
- `h2o-algos/src/test/java/` - Algorithm tests (e.g., `hex/tree/gbm/GBMTest.java`)

**Running a single test class**: Use the `test.single` property:
```bash
./gradlew :h2o-algos:testSingleNode -Dtest.single=GBMTest
```

## Module Architecture

### Core Dependencies
```
h2o-genmodel (standalone POJO/MOJO scorin
```

</details>
