---
name: adevinta__ai-engineering-metrics
source: https://github.com/adevinta/ai-engineering-metrics/blob/edc8a9bbc6555276859a8f124d022f7669cecb95/claude.md
repo: adevinta/ai-engineering-metrics
kind: claude-md
stars: 0
last_pushed: 2026-02-04T16:33:56Z
license: mit
score: 9
domains: [backend, cli-tools, data-pipeline, go]
tags: [architecture-patterns, developer-onboarding, troubleshooting-heuristics]
curated: 2026-06-15
curated_by: config-scout
---

# adevinta/ai-engineering-metrics — claude-md

**Why it's worth keeping:** Includes 'Common Development Tasks' for extending the codebase and 'When Helping Users' section containing critical debugging logic/heuristics.

**Summary:** Provides a comprehensive technical guide covering architecture diagrams, explicit expansion recipes, and specific troubleshooting heuristics.

**Source credibility:** Professional-grade documentation despite low GitHub star count; reflects high engineering standards.

**Recency:** Highly relevant; uses modern Go patterns and AWS SDK v2.

**Source:** [adevinta/ai-engineering-metrics/claude.md](https://github.com/adevinta/ai-engineering-metrics/blob/edc8a9bbc6555276859a8f124d022f7669cecb95/claude.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# AI Engineering Metrics - Claude Context

This document provides context for AI assistants (like Claude) working with the AI Engineering Metrics codebase.

## Project Purpose

This is a Go application designed to collect AI usage metrics from various data sources (starting with AWS Bedrock), filter and transform user identifiers, and publish aggregated metrics to analytics platforms like GetDX. The goal is to provide visibility into AI service usage, costs, and patterns across an organization.

## Architecture Overview

The application follows a pipeline pattern:

```
Data Sources → Collectors → Metrics → User Filtering → User ID Mapping → Publishers → External Platforms
```

### Key Components

1. **Types (`pkg/types/types.go`)**
   - `Publisher`: Interface for sending metrics to external platforms
   - `UserIDMapper`: Interface for transforming user identifiers

2. **Collectors (`pkg/collector/`)**
   - `Metric`: Core data structure representing a single AI usage event (`pkg/collector/metric.go`)
   - `ToolUsage`: Represents a user-tool combination for grouping metrics
   - `Collector`: Interface for gathering metrics from data sources
   - `BedrockCollector`: Reads AWS Bedrock
```

</details>
