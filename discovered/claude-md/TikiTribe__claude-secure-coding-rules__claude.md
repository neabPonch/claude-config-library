---
name: TikiTribe__claude-secure-coding-rules__claude
source: https://github.com/TikiTribe/claude-secure-coding-rules/blob/f644d862f89f926537591d64439c067b1e066ffe/rules/rag/graph/memgraph/CLAUDE.md
repo: TikiTribe/claude-secure-coding-rules
kind: claude-md
stars: 127
last_pushed: 2026-05-26T21:07:54Z
license: mit
score: 9
domains: [security, database, ai-rag, backend]
tags: [cypher, memgraph, injection-prevention, security-rules]
curated: 2026-06-16
curated_by: config-scout
---

# TikiTribe/claude-secure-coding-rules — claude-md

**Why it's worth keeping:** Uses a highly effective 'Do/Don't/Why' structure with explicit exploit examples; includes industry-standard CWE/OWASP references to ground the AI's logic.

**Summary:** Provides strict security protocols for Memgraph database operations, specifically targeting Cypher injection, data encryption, and RBAC.

**Source credibility:** Strong community validation indicated by 127 stars on a specialized security repo.

**Recency:** Very current, referencing OWASP 2025 standards.

**Source:** [TikiTribe/claude-secure-coding-rules/rules/rag/graph/memgraph/CLAUDE.md](https://github.com/TikiTribe/claude-secure-coding-rules/blob/f644d862f89f926537591d64439c067b1e066ffe/rules/rag/graph/memgraph/CLAUDE.md) · 127★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# CLAUDE.md - Memgraph Security Rules

Security rules for Memgraph graph database in RAG and AI applications.

**Prerequisites**: `rules/_core/rag-security.md`, `rules/_core/graph-database-security.md`

---

## Rule: Cypher Injection Prevention with Parameters

**Level**: `strict`

**When**: Executing any Cypher query with user-supplied data

**Do**: Use parameterized queries with gqlalchemy or neo4j driver
```python
from gqlalchemy import Memgraph

memgraph = Memgraph()

# Parameterized query - safe
def find_user(user_id: str):
    query = """
        MATCH (u:User {id: $user_id})
        RETURN u.name, u.email
    """
    results = memgraph.execute_and_fetch(query, {"user_id": user_id})
    return list(results)

# With neo4j driver
from neo4j import GraphDatabase

driver = GraphDatabase.driver("bolt://localhost:7687")
with driver.session() as session:
    result = session.run(
        "MATCH (n:Document) WHERE n.title = $title RETURN n",
        title=user_input
    )
```

**Don't**: Concatenate user input into Cypher queries
```python
# VULNERABLE - Cypher injection
def find_user_unsafe(user_id: str):
    query = f"MATCH (u:User {{id: '{user_id}'}}) RETURN u"
    return memgraph
```

</details>
