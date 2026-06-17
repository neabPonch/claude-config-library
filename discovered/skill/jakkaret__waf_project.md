---
name: jakkaret__waf_project
source: https://github.com/jakkaret/waf_project/blob/aaab0da3ea132a3100e894151866a5dd42463c25/Skill.md
repo: jakkaret/waf_project
kind: skill
stars: 2
last_pushed: 2026-05-26T09:19:13Z
license: unknown
score: 9
domains: [security, infrastructure, networking, devops]
tags: [waf, cdn, architecture-map, system-context]
curated: 2026-06-14
curated_by: config-scout
---

# jakkaret/waf_project — skill

**Why it's worth keeping:** The use of ASCII request flow diagrams and explicit port-to-service mappings provides the exact mental model an agent needs to debug distributed systems. The inclusion of 'Common Commands' makes it highly actionable for operational tasks.

**Summary:** A high-density architectural guide for a distributed WAF and CDN system that maps complex networking flows to specific service ports.

**Source credibility:** A niche project with low star count, likely a specialized proof-of-concept.

**Recency:** Very current, utilizing modern stacks like React 18 and Vite 5.

**Source:** [jakkaret/waf_project/Skill.md](https://github.com/jakkaret/waf_project/blob/aaab0da3ea132a3100e894151866a5dd42463c25/Skill.md) · 2★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# 🛡️ Skill.md — WAF Automated + CDN System

> **คู่มือบริบทสำหรับ AI**  
> ไฟล์นี้ช่วยให้ AI เข้าใจโปรเจกต์นี้ได้ทันทีโดยไม่ต้องอธิบายซ้ำทุกครั้ง

---

## 1. โปรเจกต์คืออะไร

ระบบรักษาความปลอดภัยและกระจายโหลด Web Application แบบ production-grade ประกอบด้วย 2 ส่วนหลัก:

| ส่วน | คำอธิบาย |
|------|-----------|
| **WAF (Web Application Firewall)** | ใช้ Nginx + ModSecurity + OWASP CRS กรองและบล็อก traffic อันตราย เช่น SQLi, XSS |
| **CDN (Content Delivery Network)** | Multi-edge node (SG/JP/TH) พร้อม GeoDNS routing, proxy cache, และ Cache Purge API |

Target origin ที่ใช้ทดสอบ: **DVWA** (Damn Vulnerable Web Application)

---

## 2. Tech Stack

| Layer | Technology |
|-------|-----------|
| **WAF/Proxy** | Nginx, ModSecurity v3, OWASP CRS |
| **CDN Edge** | Nginx (proxy_cache), ModSecurity per-node |
| **GeoDNS** | Python (custom DNS server, `dnslib`) |
| **Cache Purge API** | FastAPI (Python) |
| **Dashboard Backend** | FastAPI + Uvicorn (Python) |
| **Dashboard Frontend** | **React 18 + Vite** (TypeScript), TailwindCSS, React Router v6 |
| **State Management** | Zustand (global) + React Query (server state / data fetching) |
| **Charts** | Recharts |
| **Alert Bot** | Telegram Bot A
```

</details>
