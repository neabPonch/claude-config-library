---
name: mikopbx__Core__skill
source: https://github.com/mikopbx/Core/blob/7a7a7a7de6b3f2fef94bb063e48781668fef0ea5/.claude/skills/browserstack-tester/SKILL.md
repo: mikopbx/Core
kind: skill
stars: 551
last_pushed: 2026-06-16T09:40:20Z
license: gpl-3.0
score: 8
domains: [web-testing, devops, automation]
tags: [browserstack, phpunit, selenium, docker, php]
curated: 2026-06-16
curated_by: config-scout
---

# mikopbx/Core — skill

**Why it's worth keeping:** It defines exact `docker exec` command templates with required environment variables and provides the project-specific helper method API to enable an agent to write new UI tests correctly.

**Summary:** Provides detailed orchestration instructions for running PHPUnit/Selenium tests through a BrowserStack tunnel inside Docker containers.

**Source credibility:** High; based on a mature, actively maintained open-source PBX project (551 stars).

**Recency:** Very recent; references modern tech stacks like PHP 8.4 and Asterisk 22.

**Source:** [mikopbx/Core/.claude/skills/browserstack-tester/SKILL.md](https://github.com/mikopbx/Core/blob/7a7a7a7de6b3f2fef94bb063e48781668fef0ea5/.claude/skills/browserstack-tester/SKILL.md) · 551★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: browserstack-tester
description: Тестирование веб-интерфейса MikoPBX через BrowserStack. Запуск PHPUnit тестов с Selenium WebDriver в облачных браузерах. Использовать для автоматизированного тестирования админ-панели, проверки форм, навигации и интерактивных элементов.
allowed-tools: Bash, Read, Write, Edit, Glob, Grep
---

# BrowserStack Web UI Tester

Тестирование веб-интерфейса MikoPBX через BrowserStack. Запуск PHPUnit тестов с Selenium WebDriver в облачных браузерах. Использовать для автоматизированного тестирования админ-панели, проверки форм, навигации и интерактивных элементов.

## Prerequisites

**BrowserStack Local must be running on the host machine:**

```bash
# In a separate terminal on macOS host:
cd ~/PhpstormProjects/mikopbx/Core/tests/AdminCabinet
./start-browserstack-local.sh
```

This creates a secure tunnel between BrowserStack cloud browsers and local PBX server.

## Running Tests

### Basic Test Execution

```bash
# Run specific test file
docker exec -t mikopbx_tests-refactoring /bin/sh -c "
  cd /offload/rootfs/usr/www &&
  SERVER_PBX=https://172.16.33.72 \
  BROWSERSTACK_DAEMON_STARTED=true \
  BROWSERSTACK_LOCAL_IDENTIFIER=local_test \
  php vendo
```

</details>
