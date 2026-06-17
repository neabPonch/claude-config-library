---
name: NickDegs__sosyalpanel-flutter
source: https://github.com/NickDegs/sosyalpanel-flutter/blob/fda7ec010d272058cef9543c6a01e3f6efaf546d/CLAUDE.md
repo: NickDegs/sosyalpanel-flutter
kind: claude-md
stars: 0
last_pushed: 2026-06-14T21:06:41Z
license: unknown
score: 8
domains: [mobile-dev, cicd, ios, android]
tags: [crash-prevention, github-actions, version-pinning]
curated: 2026-06-16
curated_by: config-scout
---

# NickDegs/sosyalpanel-flutter — claude-md

**Why it's worth keeping:** It uses extremely high-signal instructions like specific 'sed' commands, exact package versions, and code stubs that an AI agent can use to proactively prevent build/runtime failures.

**Summary:** Mandates strict GitHub Action versioning and provides critical shell-based hotfixes to prevent runtime crashes in Capacitor, React Native, and Flutter mobile environments.

**Source credibility:** Low social proof (0 stars), but content contains highly specific, advanced technical troubleshooting patterns seen in real production environments.

**Recency:** Very current; addresses modern Xcode/SDK compatibility issues.

**Source:** [NickDegs/sosyalpanel-flutter/CLAUDE.md](https://github.com/NickDegs/sosyalpanel-flutter/blob/fda7ec010d272058cef9543c6a01e3f6efaf546d/CLAUDE.md) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Proje Kuralları

## GitHub Actions Versiyon Kuralları (ZORUNLU — crash önleme)

Workflow yazarken YALNIZCA bu versiyonları kullan. Yanlış versiyon = workflow anında crash.

| Action | Doğru | Yanlış |
|---|---|---|
| actions/checkout | @v4 | ~~@v5 @v6~~ |
| actions/setup-java | @v4 | ~~@v5~~ |
| actions/upload-artifact | @v4 | ~~@v5 @v6 @v7~~ |
| actions/download-artifact | @v4 | ~~@v5~~ |
| softprops/action-gh-release | @v2 | ~~@v3~~ |
| subosito/flutter-action | @v2 | — |
| ruby/setup-ruby | @v1 | — |
| r0adkll/upload-google-play | @v1 | — |

Her workflow dosyasına ekle (jobs bloğu üstüne):
```yaml
env:
  FORCE_JAVASCRIPT_ACTIONS_TO_NODE24: true
```

iOS Codemagic: `xcrun altool` Xcode 16da kaldırıldı.
Upload için `publishing.app_store_connect` bloğunu kullan, manuel altool adımı EKLEME.


## Mobil Uygulama Crash Önleme Kuralları (ZORUNLU — açılınca kapanmasın)

TestFlight/Play Store sonrası uygulama HEMEN kapanıyorsa (startup crash) önce bu listeye bak.

### Capacitor + @capacitor-community/admob + Xcode 26
Belirti: AdMob'lu Capacitor app TestFlight'ta açılınca hemen kapanır.
Kök neden: ConsentExecutor.swift iOS 26 SDK ile uyumsuz → startup crash.
Çözüm — CI workflow'a ekle (b
```

</details>
