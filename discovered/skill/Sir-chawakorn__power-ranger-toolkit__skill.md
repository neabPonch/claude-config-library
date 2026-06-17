---
name: Sir-chawakorn__power-ranger-toolkit__skill
source: https://github.com/Sir-chawakorn/power-ranger-toolkit/blob/da26dc2dcc168ebab2c2bbc727acc3b020890273/src/skills/chrome-extension/skill.md
repo: Sir-chawakorn/power-ranger-toolkit
kind: skill
stars: 33
last_pushed: 2026-01-14T19:14:41Z
license: unknown
score: 7
domains: [browser-extensions, web-automation]
tags: [chrome-extension, manifest-v3, javascript, automation]
curated: 2026-06-15
curated_by: config-scout
---

# Sir-chawakorn/power-ranger-toolkit — skill

**Why it's worth keeping:** Includes essential boilerplate for async message passing (return true pattern), service worker persistence via alarms, and a logical decision tree for architectural planning.

**Summary:** A technical template for building modern Manifest V3 Chrome Extensions, covering communication, storage, and UI patterns.

**Source credibility:** Moderate; 33 stars indicates utility for specific web automation tasks.

**Recency:** Current; adheres to Manifest V3 standards which are the current industry requirement.

**Source:** [Sir-chawakorn/power-ranger-toolkit/src/skills/chrome-extension/skill.md](https://github.com/Sir-chawakorn/power-ranger-toolkit/blob/da26dc2dcc168ebab2c2bbc727acc3b020890273/src/skills/chrome-extension/skill.md) · 33★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: chrome-extension
description: Build Chrome Extensions with Manifest V3, background service workers, content scripts, and message passing. Use when developing TikTok Uploader extension or any browser extensions.
---

# 🔌 Chrome Extension Skill

## Use Cases
- TikTok auto-uploader
- Web automation tools
- Content modification
- Data extraction

---

## Manifest V3 Structure

```json
{
  "manifest_version": 3,
  "name": "Extension Name",
  "version": "1.0.0",
  "permissions": ["activeTab", "storage", "tabs"],
  "host_permissions": ["https://*.tiktok.com/*"],
  "background": {
    "service_worker": "background.js"
  },
  "content_scripts": [{
    "matches": ["https://*.tiktok.com/*"],
    "js": ["content.js"]
  }],
  "action": {
    "default_popup": "popup.html"
  },
  "side_panel": {
    "default_path": "sidepanel.html"
  }
}
```

---

## Message Passing

### Content → Background
```javascript
// content.js
chrome.runtime.sendMessage({ type: 'UPLOAD_COMPLETE', data: result });

// background.js
chrome.runtime.onMessage.addListener((message, sender, sendResponse) => {
  if (message.type === 'UPLOAD_COMPLETE') {
    console.log('Upload done:', message.data);
    sendResponse({
```

</details>
