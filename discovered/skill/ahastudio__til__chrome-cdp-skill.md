---
name: ahastudio__til__chrome-cdp-skill
source: https://github.com/ahastudio/til/blob/4685c122729ce605bf49a0b9832e9100f7c6d6c6/chrome/chrome-cdp-skill.md
repo: ahastudio/til
kind: skill
stars: 173
last_pushed: 2026-06-15T08:28:53Z
license: unknown
score: 9
domains: [agents-ai, cli-tools, web-automation]
tags: [chrome-cdp, browser-automation, accessibility-tree, daemon-pattern]
curated: 2026-06-15
curated_by: config-scout
---

# ahastudio/til — skill

**Why it's worth keeping:** Implements a 'resident daemon' pattern to absorb expensive/modal-heavy connection handshakes, and utilizes the Accessibility Tree as a semantic compression technique for AI-friendly page structure.

**Summary:** Connects AI agents to a user's active Chrome session using a resident per-tab daemon via the Chrome DevTools Protocol. This maintains login states and existing tabs without the friction of spawning new browser instances.

**Source credibility:** High; demonstrates advanced architectural knowledge of browser protocols and user friction reduction.

**Recency:** Very current, utilizing Node.js 22 native capabilities.

**Source:** [ahastudio/til/chrome/chrome-cdp-skill.md](https://github.com/ahastudio/til/blob/4685c122729ce605bf49a0b9832e9100f7c6d6c6/chrome/chrome-cdp-skill.md) · 173★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# `chrome-cdp` skill

AI 에이전트가 실행 중인 Chrome 브라우저와 직접 상호작용할 수 있게 해주는
경량 CDP(Chrome DevTools Protocol) CLI 도구입니다.

<https://github.com/pasky/chrome-cdp-skill>

## 핵심 가치

**"이미 열려 있는 브라우저를 그대로 씁니다."**

Puppeteer 같은 도구는 격리된 새 브라우저를 띄웁니다. chrome-cdp-skill은
사용자가 실제로 사용 중인 Chrome 탭에 연결합니다. 로그인 상태, 페이지
상태, 열린 탭 전부를 AI 에이전트가 그대로 활용할 수 있습니다.

## 설치

`skills/chrome-cdp/` 디렉토리를 복사.

- Node.js 22+ 필요.
- npm install 불필요.

Chrome에서 `chrome://inspect/#remote-debugging` 토글을 켜야 합니다.

Chrome, Chromium, Brave, Edge, Vivaldi를 자동 감지합니다.

## 명령어

| 명령어                           | 설명                                       |
| -------------------------------- | ------------------------------------------ |
| `list`                           | 열린 탭 목록                               |
| `snap <target>`                  | 접근성 트리 스냅샷                         |
| `eval <target> "expr"`           | JavaScript 실행                            |
| `shot <target> [file]`           | 스크린샷 캡처 (DPR 좌표 매핑 포함)         |
| `html <target> [".selector"]`    | 전체 HTML 또는 CSS 선택자 범위 HTML        |
| `nav <target> <url>`             | URL 이동 후 로드 완료 대기                 |
| `net <target>`                   | 네트워크 리소스 타이밍
```

</details>
