---
name: claude-dev-suite__claude-dev-suite__skill
source: https://github.com/claude-dev-suite/claude-dev-suite/blob/95ca62433c5577c1965ff811bd8e8d39292bed8f/skills/real-time/webrtc/SKILL.md
repo: claude-dev-suite/claude-dev-suite
kind: skill
stars: 20
last_pushed: 2026-06-05T03:43:52Z
license: mit
score: 8
domains: [web-frontend, real-time-communication]
tags: [webrtc, video-streaming, p2p, sfu]
curated: 2026-06-15
curated_by: config-scout
---

# claude-dev-suite/claude-dev-suite — skill

**Why it's worth keeping:** Includes high-signal 'Anti-Patterns' and specific negative constraints that prevent the agent from choosing WebRTC when SSE or Socket.io is more appropriate.

**Summary:** A specialized knowledge guide for WebRTC implementation covering signaling, peer connections, and SFU integration.

**Source credibility:** The repository is small (20 stars), but the structured technical content suggests professional expertise.

**Recency:** Current; includes modern patterns for SFU integration via LiveKit and track replacement logic.

**Source:** [claude-dev-suite/claude-dev-suite/skills/real-time/webrtc/SKILL.md](https://github.com/claude-dev-suite/claude-dev-suite/blob/95ca62433c5577c1965ff811bd8e8d39292bed8f/skills/real-time/webrtc/SKILL.md) · 20★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: webrtc
description: |
  WebRTC peer-to-peer communication. Signaling, ICE/STUN/TURN, media streams,
  data channels, screen sharing, and SFU integration (mediasoup, LiveKit).

  USE WHEN: user mentions "WebRTC", "video call", "peer-to-peer", "P2P",
  "screen sharing", "data channel", "STUN", "TURN", "mediasoup", "LiveKit"

  DO NOT USE FOR: server-to-client streaming - use `sse`;
  chat messaging - use `socket-io`
allowed-tools: Read, Grep, Glob, Write, Edit
---
# WebRTC

## Peer Connection Setup

```typescript
const config: RTCConfiguration = {
  iceServers: [
    { urls: 'stun:stun.l.google.com:19302' },
    { urls: 'turn:turn.example.com', username: 'user', credential: 'pass' },
  ],
};

const pc = new RTCPeerConnection(config);

// Get local media
const stream = await navigator.mediaDevices.getUserMedia({ video: true, audio: true });
stream.getTracks().forEach((track) => pc.addTrack(track, stream));

// Display remote stream
pc.ontrack = (event) => {
  remoteVideo.srcObject = event.streams[0];
};

// ICE candidates — send to remote peer via signaling
pc.onicecandidate = (event) => {
  if (event.candidate) {
    signalingChannel.send({ type: 'ice-candidate', candidate:
```

</details>
