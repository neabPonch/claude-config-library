---
name: nemanjan00__dev-environment__claude
source: https://github.com/nemanjan00/dev-environment/blob/4c83ff637ac77cf9f9ce226adf38e6e8caea9a30/profiles/analyst/CLAUDE.md
repo: nemanjan00/dev-environment
kind: claude-md
stars: 52
last_pushed: 2026-06-12T09:39:08Z
license: unknown
score: 8
domains: [cli-tools, data-analysis, security, devops]
tags: [profile, tooling, forensics]
curated: 2026-06-15
curated_by: config-scout
---

# nemanjan00/dev-environment — claude-md

**Why it's worth keeping:** It provides exact command signatures and one-liners (e.g., for dsq and duckdb) that allow an agent to perform complex data tasks without trial-and-error.

**Summary:** A highly specialized toolset profile designed for data analysis, database inspection, and system forensics within a containerized environment.

**Source credibility:** Individual developer providing a high-density, specialized dev environment/image.

**Recency:** 

**Source:** [nemanjan00/dev-environment/profiles/analyst/CLAUDE.md](https://github.com/nemanjan00/dev-environment/blob/4c83ff637ac77cf9f9ce226adf38e6e8caea9a30/profiles/analyst/CLAUDE.md) · 52★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Analyst Profile

For inspecting live systems and data stores: pulling logs, querying databases,
poking at S3 buckets and message queues, and slicing structured data. Extends
the `reversing` profile, so all binary/forensics tooling is also available.

## Object storage / S3

- **aws-cli-v2** (`aws`) — official AWS CLI. Supports AWS, and any S3-compatible
  endpoint via `--endpoint-url` (MinIO, Ceph, Wasabi, etc.).
- **s3cmd** — scriptable S3 client, handy for batch ops and non-AWS providers.
- **rclone** — universal remote-storage mover. Handles S3, GCS, Azure, SFTP,
  WebDAV, and 40+ more. Use `rclone lsf`, `rclone cat`, `rclone copy` for quick
  pulls from any configured remote.

## SQL clients

- **postgresql** (`psql`) — PostgreSQL client. Server not started by default;
  this is the CLI only.
- **mariadb-clients** (`mariadb`, `mysqldump`) — MySQL/MariaDB CLI.
- **sqlite** (`sqlite3`) — SQLite CLI for local `.db` / `.sqlite` files.
- **duckdb** — in-process analytical SQL engine. Queries CSV/Parquet/JSON
  directly: `duckdb -c "SELECT count(*) FROM 'data.parquet'"`. Great for
  ad-hoc analysis without loading into a real warehouse.
- **dsq** — run SQL against JSON/CSV/TSV/Exc
```

</details>
