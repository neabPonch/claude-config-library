# Advisor Questionnaire

Use this questionnaire when a user's project description lacks enough detail to generate a confident config. Ask only the questions that are still unanswered.

---

## Core questions

1. **What are you building?**
   _Brief description — e.g., "a multi-tenant SaaS dashboard", "a CLI tool for data pipelines", "a mobile game"_

2. **What is your primary stack / language?**
   _e.g., Next.js + TypeScript, Python + FastAPI, Go, Rust, Swift_

3. **What does your backend look like?** (if applicable)
   _e.g., REST API, GraphQL, gRPC, serverless functions, none_

4. **What is your data layer?**
   _e.g., Postgres + Prisma, MongoDB, SQLite, no database_

5. **Solo or team?**
   _Solo dev / small team (2-5) / larger team_

6. **What does your CI/CD look like?**
   _e.g., GitHub Actions, GitLab CI, no CI yet_

7. **Where does it deploy?**
   _e.g., Vercel, AWS, GCP, self-hosted, not yet decided_

8. **Any specific pain points you want Claude to help with most?**
   _e.g., test coverage, code review, refactoring, documentation, debugging_

---

## Domain signal questions (ask if the domain is ambiguous)

**If data/ML is involved:**
- Training, inference, or both?
- Any specific frameworks (PyTorch, JAX, Hugging Face, LangChain)?
- Notebooks or pure Python scripts?

**If agents/AI is involved:**
- Orchestrating multiple LLM calls, or building tooling around a single model?
- Using Claude, OpenAI, or other providers?
- MCP servers, custom tools, or both?

**If devops/infra is involved:**
- IaC tool (Terraform, Pulumi, CDK)?
- Container orchestration (k8s, ECS, Docker Compose)?

**If mobile is involved:**
- iOS, Android, or cross-platform (React Native, Flutter)?

**If security is involved:**
- Offensive (CTF, pentest) or defensive (SIEM, hardening)?

---

## Output the advisor should produce

After gathering answers, generate:

```
## Recommended CLAUDE.md

[composed content]

## Recommended Skills

- [skill name] — [why it fits]
- ...

## Recommended Workflow Practices

- [workflow/practices/foo.md] — [one-line reason]
- ...

## Notes

[anything project-specific not covered by templates]
```
