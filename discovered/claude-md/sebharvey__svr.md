---
name: sebharvey__svr
source: https://github.com/sebharvey/svr/blob/ec33231a39d62a709e135e53de49b7d3b911b7f0/CLAUDE.MD
repo: sebharvey/svr
kind: claude-md
stars: 0
last_pushed: 2026-06-13T14:22:15Z
license: unknown
score: 9
domains: [web-frontend, backend-api, domain-logic]
tags: [railway, .net, azure, javascript]
curated: 2026-06-14
curated_by: config-scout
---

# sebharvey/svr — claude-md

**Why it's worth keeping:** It captures critical 'tribal knowledge' that code alone won't reveal, such as the non-intuitive railway direction conventions and specific algorithm priorities for train service selection.

**Summary:** Provides dense, high-value domain logic for a real-time transit visualization system.

**Source credibility:** Low star count, but the extreme specificity of domain rules suggests a genuine, high-quality project.

**Recency:** Highly current, featuring .NET 8 and mentions of MCP (Model Context Protocol).

**Source:** [sebharvey/svr/CLAUDE.MD](https://github.com/sebharvey/svr/blob/ec33231a39d62a709e135e53de49b7d3b911b7f0/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Severn Valley Railway Live Train Tracker

## Project Overview

A real-time web application that visualises train movements on the Severn Valley Railway heritage line between Kidderminster and Bridgnorth. The system consists of a .NET 8 Azure Functions API backend serving timetable data, and a pure JavaScript frontend providing live train tracking with no dependencies.

**Live URL**: https://victorious-mushroom-07851c603.1.azurestaticapps.net  
**API URL**: https://svrliveapi-aaeydueba4b9aveb.uksouth-01.azurewebsites.net

## Architecture

### Backend (Azure Functions API)
- **Framework**: .NET 8 (Isolated Worker Model)
- **Hosting**: Azure Functions
- **Location**: `src/API/SevernValleyTimetable/`
- **Primary Functions**:
  - `HealthCheckFunction.cs` - System health endpoint at `/api/health`
  - `TimetableFunction.cs` - Timetable data endpoint at `/api/timetable`
  - `TimetableService.cs` - Core business logic for timetable loading and caching
  - `TimetableMcpServer.cs` - MCP (Model Context Protocol) server (currently commented out)

### Frontend (Static Web App)
- **Technology**: Pure vanilla JavaScript, HTML5, CSS3
- **Hosting**: Azure Static Web Apps
- **Location**: `src/Web/`
```

</details>
