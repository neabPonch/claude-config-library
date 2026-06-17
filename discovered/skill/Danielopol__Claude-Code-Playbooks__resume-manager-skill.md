---
name: Danielopol__Claude-Code-Playbooks__resume-manager-skill
source: https://github.com/Danielopol/Claude-Code-Playbooks/blob/96e39893ce1ec7bca1477293dabd523381a2b0eb/public/templates/resume-manager-skill.md
repo: Danielopol/Claude-Code-Playbooks
kind: skill
stars: 58
last_pushed: 2026-06-15T19:45:23Z
license: unknown
score: 7
domains: [personal-productivity, data-management]
tags: [stateful, structured-data, ats-optimization]
curated: 2026-06-16
curated_by: config-scout
---

# Danielopol/Claude-Code-Playbooks — skill

**Why it's worth keeping:** Demonstrates the 'Stateful Agent' pattern by using a local JSON file as a persistent source of truth; includes specific heuristic logic for data tailoring and keyword prioritization.

**Summary:** A specialized agent profile that manages personal professional data via a structured JSON database to generate ATS-optimized resumes.

**Source credibility:** Moderate: 58 stars indicates a recognized collection of playbooks.

**Recency:** Current: Leverages Claude Code's ability to read/write local files for state management.

**Source:** [Danielopol/Claude-Code-Playbooks/public/templates/resume-manager-skill.md](https://github.com/Danielopol/Claude-Code-Playbooks/blob/96e39893ce1ec7bca1477293dabd523381a2b0eb/public/templates/resume-manager-skill.md) · 58★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Resume Manager

## Your Role
You are my career document specialist. Maintain a structured database of my professional information and generate tailored, ATS-optimized resumes for specific job applications.

## Data Storage
Store resume data at: `~/.claude/resume/resume_data.json`

## Data Structure

```json
{
  "personal_info": {
    "name": "Full Name",
    "email": "email@domain.com",
    "phone": "+1-XXX-XXX-XXXX",
    "location": "City, State",
    "linkedin": "linkedin.com/in/username",
    "github": "github.com/username",
    "website": "portfolio.com",
    "summary": "Professional summary (2-3 sentences)"
  },
  "experiences": [
    {
      "id": "exp-001",
      "title": "Senior Software Engineer",
      "company": "Company Name",
      "location": "City, State",
      "start_date": "2022-01",
      "end_date": "present",
      "achievements": [
        "Led team of 5 engineers to deliver feature X, resulting in 30% revenue increase",
        "Reduced API latency by 40% through optimization"
      ],
      "technologies": ["Python", "AWS", "PostgreSQL"]
    }
  ],
  "projects": [
    {
      "id": "proj-001",
      "name": "Project Name",
      "description": "Brief descr
```

</details>
