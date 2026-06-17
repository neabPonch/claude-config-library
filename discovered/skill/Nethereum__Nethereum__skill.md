---
name: Nethereum__Nethereum__skill
source: https://github.com/Nethereum/Nethereum/blob/de892335570e2fa764370a730a42eb915c20fa4a/plugins/nethereum-skills/skills/wallet-quickstart/SKILL.md
repo: Nethereum/Nethereum
kind: skill
stars: 2253
last_pushed: 2026-05-12T09:00:06Z
license: mit
score: 9
domains: [.net, blockchain, mobile-dev, security]
tags: [nethereum, mvvm, blazor, maui, web3]
curated: 2026-06-16
curated_by: config-scout
---

# Nethereum/Nethereum — skill

**Why it's worth keeping:** It includes highly transferable boilerplate patterns for complex enterprise concerns like the Localizer pattern, Service Registration strategies, and the exact dependency injection sequence required for the SDK.

**Summary:** Provides an architectural blueprint and specific code patterns for building multi-platform crypto wallets using the Nethereum SDK. Covers everything from secure vault management to MVVM service registration and localization.

**Source credibility:** Extremely high; Nethereum is a premier, widely-used Ethereum library for .NET with significant community traction.

**Recency:** Current; utilizes modern .NET patterns including CommunityToolkit.Mvvm, Blazor, and MAUI.

**Source:** [Nethereum/Nethereum/plugins/nethereum-skills/skills/wallet-quickstart/SKILL.md](https://github.com/Nethereum/Nethereum/blob/de892335570e2fa764370a730a42eb915c20fa4a/plugins/nethereum-skills/skills/wallet-quickstart/SKILL.md) · 2253★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: wallet-quickstart
description: Build a multi-platform wallet application using the Nethereum Wallet SDK with MVVM architecture (.NET/C#). Use this skill when the user asks about building a wallet app, Nethereum.Wallet, wallet UI components, MVVM wallet, WalletVault, account management in the wallet SDK, or creating wallet screens in Blazor or MAUI.
user-invocable: true
---

# Nethereum Wallet SDK

Build multi-platform self-custodial wallet applications using a layered MVVM architecture with shared ViewModels and platform-specific renderers.

## Architecture

```
Nethereum.Wallet                              Core services
  + Nethereum.Wallet.UI.Components            Shared MVVM ViewModels
  + Nethereum.Wallet.UI.Components.Blazor     Blazor/MudBlazor renderer
    or .Maui                                  .NET MAUI renderer
```

NuGet packages:

```bash
dotnet add package Nethereum.Wallet
dotnet add package Nethereum.Wallet.UI.Components.Blazor
```

## Quick Start

### Register Services (Program.cs)

```csharp
builder.Services.AddNethereumWallet();
builder.Services.AddNethereumWalletBlazorComponents();
```

### Add the Wallet Component

```razor
@using Nethereum.Wallet.UI.
```

</details>
