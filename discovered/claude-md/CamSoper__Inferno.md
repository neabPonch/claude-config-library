---
name: CamSoper__Inferno
source: https://github.com/CamSoper/Inferno/blob/9cabcb189ee91ab123dc9e5fc03848fee01fb19f/CLAUDE.md
repo: CamSoper/Inferno
kind: claude-md
stars: 47
last_pushed: 2026-06-14T22:25:13Z
license: mit
score: 9
domains: [iot, embedded-systems, .net]
tags: [hardware-control, pid, dotnet, raspberry-pi]
curated: 2026-06-15
curated_by: config-scout
---

# CamSoper/Inferno — claude-md

**Why it's worth keeping:** Excellent use of 'domain-specific business logic' explanation (the P-Value system) which AI cannot easily infer from code alone. Mapping physical hardware pins/addresses directly in the file is a top-tier technique for hardware projects.

**Summary:** Provides high-density domain knowledge for an IoT control system, including state machine logic and PID parameters. It includes essential build, deployment (Pulumi), and hardware-level mappings.

**Source credibility:** High; shows high technical maturity with detailed architectural and hardware specifics.

**Recency:** Current; utilizes modern .NET, Pulumi, and structured deployment workflows suitable for current AI coding assistants.

**Source:** [CamSoper/Inferno/CLAUDE.md](https://github.com/CamSoper/Inferno/blob/9cabcb189ee91ab123dc9e5fc03848fee01fb19f/CLAUDE.md) · 47★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Inferno is a smart wood pellet smoker controller for a Traeger Junior Elite 20, running on a Raspberry Pi 3 with .NET. It manages fire control (auger, blower, igniter) via GPIO relays, reads temperatures via RTD sensors through an MCP3008 ADC over SPI, and displays status on a 20x4 I2C LCD.

## Build & Deploy

```bash
# Build entire solution
dotnet build Inferno.sln

# Build individual project
dotnet build Inferno.Api/Inferno.Api.csproj

# Deploy project
cd Inferno.Deploy/
pulumi up
```

Deployment to the Pi is managed via Pulumi (see `Inferno.Deploy`). The Pi hostname is `inferno`.

```bash
# Run tests
dotnet test Inferno.Tests
```

## Architecture

Six projects in `Inferno.sln`:

- **Inferno.Api** — ASP.NET Core Web API (port 5000/5001). Core controller logic, PID algorithm, fire management, hardware device abstractions. This is the main application that runs on the Pi.
- **Inferno.Cli** — Command-line client for controlling the smoker remotely via HTTP.
- **Inferno.Common** — Shared models (`SmokerMode`, `SmokerStatus`, `Temps`), interfaces (`
```

</details>
