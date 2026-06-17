---
name: tigusigalpa__bingx-go
source: https://github.com/tigusigalpa/bingx-go/blob/b8360994504d9369179f02b9b9640cc84b448021/skill.md
repo: tigusigalpa/bingx-go
kind: skill
stars: 18
last_pushed: 2026-05-03T16:11:29Z
license: mit
score: 9
domains: [trading-api, fintech]
tags: [golang, crypto, bingx]
curated: 2026-06-14
curated_by: config-scout
---

# tigusigalpa/bingx-go — skill

**Why it's worth keeping:** Uses practical, copyable code snippets rather than just method signatures; includes critical constants and specific parameter patterns required for successful API execution.

**Summary:** Provides a high-density, code-first reference for interacting with the BingX exchange via Go. It covers the full lifecycle from client initialization to complex trading operations like TWAP and trailing stops.

**Source credibility:** Niche repository with professional documentation and very recent maintenance.

**Recency:** Highly current/recent based on push history.

**Source:** [tigusigalpa/bingx-go/skill.md](https://github.com/tigusigalpa/bingx-go/blob/b8360994504d9369179f02b9b9640cc84b448021/skill.md) · 18★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# bingx-go SDK — AI Skill Reference

> Full-featured Go SDK for the BingX cryptocurrency exchange API.
> Module: `github.com/tigusigalpa/bingx-go/v2`
> Requires: Go 1.21+, dependency: `gorilla/websocket`

---

## Installation

```bash
go get github.com/tigusigalpa/bingx-go/v2
go mod tidy
```

---

## Client Initialization

```go
import bingx "github.com/tigusigalpa/bingx-go/v2"

// Standard client
client := bingx.NewClient("API_KEY", "API_SECRET")

// With options
client := bingx.NewClient(apiKey, apiSecret,
    bingx.WithBaseURI("https://open-api.bingx.com"),   // default
    bingx.WithSignatureEncoding("hex"),                 // or "base64" (default)
    bingx.WithSourceKey("MyBot"),                       // optional tag
)

// Demo/VST environment (paper trading)
client := bingx.NewDemoClient(apiKey, apiSecret)
```

**Client options:**
- `WithBaseURI(uri string)` — override API endpoint
- `WithSignatureEncoding(enc string)` — `"base64"` (default) or `"hex"`
- `WithSourceKey(key string)` — label requests for debugging
- `WithDemoEnvironment()` — sets base URI to `https://open-api-vst.bingx.com`

**Service accessors on `*Client`:**
```go
client.Market()      // *services.MarketServ
```

</details>
