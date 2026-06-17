---
name: enuno__unifi-mcp-server
source: https://github.com/enuno/unifi-mcp-server/blob/db6b0cb8aa3c4e221fd247d14c7df0842b1ef838/SKILL.md
repo: enuno/unifi-mcp-server
kind: skill
stars: 166
last_pushed: 2026-06-14T04:47:17Z
license: apache-2.0
score: 9
domains: [network-infrastructure, cli-tools, iot]
tags: [unifi, networking, ubiquiti, mcp]
curated: 2026-06-14
curated_by: config-scout
---

# enuno/unifi-mcp-server — skill

**Why it's worth keeping:** Introduces the 'Scoped MCP profiles' pattern to prevent context bloat when dealing with large toolsets (86+ tools) and uses highly specific trigger keywords.

**Summary:** A sophisticated skill definition for UniFi network management that categorizes massive toolsets into logical domains.

**Source credibility:** High; notable star count and very recent maintenance indicated.

**Recency:** 

**Source:** [enuno/unifi-mcp-server/SKILL.md](https://github.com/enuno/unifi-mcp-server/blob/db6b0cb8aa3c4e221fd247d14c7df0842b1ef838/SKILL.md) · 166★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: unifi
description: >
  Manage UniFi network infrastructure via the UniFi MCP Server. Use this skill
  for any task involving UniFi devices, clients, networks, VLANs, WiFi, firewall
  rules, zone-based firewall, VPNs, traffic monitoring, backups, RADIUS, QoS,
  DPI, port forwarding, ACLs, DHCP, DNS, or site management. Triggers when the
  user mentions UniFi, Ubiquiti, network clients, APs, switches, gateways,
  firewall policies, or traffic flows in a network management context.
triggers:
  - UniFi
  - Ubiquiti
  - network clients
  - access point
  - UniFi switch
  - UniFi gateway
  - firewall policy
  - VLAN management
  - traffic flows
  - SSID
  - WiFi network
  - site controller
---

# UniFi MCP Server Skill

Interact with your UniFi Network Controller using 86+ MCP tools across six
capability domains. The server supports three API modes (local gateway,
cloud-v1, cloud-ea) and requires UniFi Network 9.0+ for zone-based firewall
features.

## Quick Setup

### Via MCP (recommended for full tool access)

Add to your MCP client config (`~/.claude/mcp.json` or equivalent):

```json
{
  "mcpServers": {
    "unifi": {
      "command": "uvx",
      "args": ["unifi-mcp-server
```

</details>
