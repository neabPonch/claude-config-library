---
name: sjswerdloff__dicom_event_broker_adapter
source: https://github.com/sjswerdloff/dicom_event_broker_adapter/blob/f4ebdb2cc69f0479158bbfdbcf752c4eba32719d/CLAUDE.md
repo: sjswerdloff/dicom_event_broker_adapter
kind: claude-md
stars: 1
last_pushed: 2026-05-03T12:03:10Z
license: apache-2.0
score: 7
domains: [backend, integration-adapter]
tags: [python, poetry, pytest, mqtt]
curated: 2026-06-15
curated_by: config-scout
---

# sjswerdloff/dicom_event_broker_adapter — claude-md

**Why it's worth keeping:** Includes high-signal instructions for running tests with specific markers and provides exact orchestration scripts for external dependencies like Mosquitto. This reduces LLM guesswork during development/testing cycles.

**Summary:** Defines precise CLI commands for dependency management, tiered testing (unit vs integration), and local infrastructure setup. Establishes strict Pythonic coding standards and library-specific idioms.

**Source credibility:** Small developer project with recent maintenance activity.

**Recency:** Current; follows modern Python toolchain standards (Poetry, Pytest).

**Source:** [sjswerdloff/dicom_event_broker_adapter/CLAUDE.md](https://github.com/sjswerdloff/dicom_event_broker_adapter/blob/f4ebdb2cc69f0479158bbfdbcf752c4eba32719d/CLAUDE.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# DICOM Event Broker Adapter Development Guide

## Commands
- Install dependencies: `poetry install`
- Run unit tests: `poetry run pytest tests -m "no mqtt_integration"`
- Run integration tests: `poetry run pytest -m mqtt_integration -v`
- Run tests with specific marker: `poetry run pytest -m mqtt_integration`
- Run all tests: `poetry run pytest tests`
- Run specific test: `poetry run pytest tests/test_file.py::TestClass::test_method`
- Lint code: `poetry run flake8 dicom_event_broker_adapter`
- Format code: `poetry run black dicom_event_broker_adapter`
- Sort imports: `poetry run isort dicom_event_broker_adapter`
- Start Mosquitto for testing: `./scripts/run_mosquitto.sh start`
- Stop Mosquitto after testing: `./scripts/run_mosquitto.sh stop`

## Code Style
- Follow Black formatting (line length: 127)
- Use type hints for all function parameters and return values
- Follow snake_case naming for variables and functions
- Use descriptive docstrings for modules, classes, and functions
- Structure imports: stdlib → third-party → local
- Use explicit exception handling with specific exception classes
- Follow pytest patterns for testing with fixtures in conftest.py
- Make use of pynetdi
```

</details>
