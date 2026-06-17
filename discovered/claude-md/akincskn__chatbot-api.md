---
name: akincskn__chatbot-api
source: https://github.com/akincskn/chatbot-api/blob/1a252b36585af7d718d15434b63f6a85ae156a72/Claude.MD
repo: akincskn/chatbot-api
kind: claude-md
stars: 0
last_pushed: 2026-05-03T21:09:38Z
license: unknown
score: 9
domains: [backend-api, ai-rag, java-spring-boot]
tags: [spring-boot, architecture-patterns, rag, java-21]
curated: 2026-06-16
curated_by: config-scout
---

# akincskn/chatbot-api — claude-md

**Why it's worth keeping:** The explicit package tree and mandatory constraints (like file length limits and specific injection styles) provide excellent guardrails for AI agents to prevent codebase rot.

**Summary:** A highly opinionated architectural blueprint for a Spring Boot RAG application that enforces strict layering and coding standards.

**Source credibility:** Low social proof (0 stars), but the technical density suggests a high-quality personal project.

**Recency:** Very current, utilizing Java 21 and modern AI/RAG tech stacks.

**Source:** [akincskn/chatbot-api/Claude.MD](https://github.com/akincskn/chatbot-api/blob/1a252b36585af7d718d15434b63f6a85ae156a72/Claude.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md — Chatbot API (Spring Boot Backend)

## Proje Nedir?
AI Chatbot Platform'un backend API'ı. Kullanıcılar döküman yükler (PDF, URL, text), sistem bunları vectorize eder ve RAG (Retrieval Augmented Generation) ile soru-cevap chatbot'u oluşturur. Chatbot'lar embed script ile başka sitelere eklenebilir.

## Tech Stack
- Java 21 + Spring Boot 3.x
- Spring Security + JWT (stateless auth)
- Spring Data JPA + Hibernate
- PostgreSQL + pgvector extension (Neon)
- Groq API (Llama 3.3 — primary LLM)
- Google Gemini API (fallback LLM)
- HuggingFace Inference API (embedding — all-MiniLM-L6-v2)
- Apache PDFBox (PDF parsing)
- Jsoup (HTML parsing / web scraping)
- Maven
- Deploy: Koyeb (free tier)

## Mimari Kuralları

### Katmanlı Mimari (ZORUNLU)
```
Controller → Service → Repository
```
- Controller: HTTP layer, input validation (@Valid), auth kontrolü, DTO dönüşümü
- Service: Business logic, transaction yönetimi, external service çağrıları
- Repository: JPA data access, native query (pgvector)
- **Controller ASLA doğrudan Repository çağırmaz**
- **Repository ASLA business logic içermez**

### DTO Pattern (ZORUNLU)
- Entity'ler doğrudan response olarak DÖNMEZ
- Request DTO: kullanıcı
```

</details>
