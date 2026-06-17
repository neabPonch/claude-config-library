---
name: blackscythe123__voxa__claude
source: https://github.com/blackscythe123/voxa/blob/02e5246fbf8dc27ce6f6f261e1d70443a1d02201/voxa-kotlin/CLAUDE.md
repo: blackscythe123/voxa
kind: claude-md
stars: 2
last_pushed: 2026-06-14T20:46:23Z
license: gpl-3.0
score: 9
domains: [mobile-android, embedded-audio, ui-ux]
tags: [android, kotlin, voice, ime]
curated: 2026-06-16
curated_by: config-scout
---

# blackscythe123/voxa — claude-md

**Why it's worth keeping:** The 'Android gotchas' provide essential hardware/API timing logic, while the 'Slop linter' enforces stylistic constraints that prevent AI-generated patterns.

**Summary:** Combines critical platform edge cases, environment workarounds, and aesthetic 'slop' rules to maintain high-quality development.

**Source credibility:** Low star count but highly specific technical depth suggests real-world utility.

**Recency:** Current; covers modern Android 13+ features and contemporary developer environments.

**Source:** [blackscythe123/voxa/voxa-kotlin/CLAUDE.md](https://github.com/blackscythe123/voxa/blob/02e5246fbf8dc27ce6f6f261e1d70443a1d02201/voxa-kotlin/CLAUDE.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Voxa

Android Kotlin/Compose voice-dictation IME. Captures a ChatGPT session in a WebView, transcribes via OpenAI Whisper, inserts text into the active text field.

## Build & install
- `./gradlew :app:assembleRelease` — release uses debug keystore (in `buildTypes.release`) so output is sideload-installable.
- Reliable install when USB drops mid-stream: `adb push app-release.apk /data/local/tmp/voxa.apk && adb shell pm install -r /data/local/tmp/voxa.apk`
- `MSYS_NO_PATHCONV=1` prefix on Git Bash to stop `/data/local/tmp` getting rewritten to `C:/Program Files/Git/...`
- Gradle needs JDK 11+; Android Studio's bundled JBR is JDK 21 and is the safe default.

## Logs
- `adb logcat -s VoxaAudio:*` — audio routing decisions (Builtin / WiredHeadset / BluetoothSco etc.)
- `adb exec-out screencap -p > out.png` — reliable screen capture on OEM Android (avoid `shell screencap -p FILE` + pull)

## Android gotchas
- `AudioManager.setCommunicationDevice()` only accepts devices from `availableCommunicationDevices`, NOT `getDevices(GET_DEVICES_INPUTS)`. Wrong list = silent false.
- BT SCO needs ~400ms settle time after `setCommunicationDevice` before MediaRecorder will capture from the headset
```

</details>
