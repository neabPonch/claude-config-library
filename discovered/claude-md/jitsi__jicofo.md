---
name: jitsi__jicofo
source: https://github.com/jitsi/jicofo/blob/72d22dedae7f5f02eb88d2d245fc09dc1e1e73cc/CLAUDE.md
repo: jitsi/jicofo
kind: claude-md
stars: 341
last_pushed: 2026-06-12T22:24:34Z
license: apache-2.0
score: 9
domains: [backend, java, kotlin]
tags: [maven, architecture-guide, testing-patterns, multi-module]
curated: 2026-06-15
curated_by: config-scout
---

# jitsi/jicofo — claude-md

**Why it's worth keeping:** The inclusion of explicit 'Application Flow' steps and deep documentation on testing utilities provides the AI with crucial execution context. It also clearly outlines module dependencies to prevent the LLM from suggesting illegal imports.

**Summary:** A highly detailed guide for a multi-module Java/Kotlin project that covers build commands, architectural boundaries, and specific testing patterns.

**Source credibility:** High; Jitsi is a well-established, highly starred open-source project with active maintenance.

**Recency:** Current; the content reflects modern Kotlin/Java development practices relevant to today's Claude Code usage.

**Source:** [jitsi/jicofo/CLAUDE.md](https://github.com/jitsi/jicofo/blob/72d22dedae7f5f02eb88d2d245fc09dc1e1e73cc/CLAUDE.md) · 341★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Jicofo (JItsi COnference FOcus) is a signaling server for Jitsi Meet conferences. It manages XMPP Multi-User Chat (MUC) rooms, initiates Jingle sessions with participants, and coordinates media routing through Jitsi Videobridge instances using the Colibri2 protocol.

## Build and Test Commands

### Building
```bash
mvn install                          # Build all modules and create distribution package
mvn clean install                    # Clean build
mvn install -DskipTests              # Build without running tests
```

The distribution package is created in `jicofo/target/jicofo-1.1-SNAPSHOT-archive.zip`.

### Testing
```bash
mvn test                             # Run all tests
mvn test -pl jicofo-selector         # Run tests for specific module
mvn test -Dtest=BridgeSelectorTest   # Run specific test class
```

### Code Quality
```bash
mvn ktlint:check                     # Run ktlint (must be run for individual modules e.g. in ./jicofo-selector/)
mvn checkstyle:check                 # Run checkstyle (config: checkstyle.xml)
```

## Architecture

##
```

</details>
