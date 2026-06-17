---
name: vm0-ai__vm0-skills__skill
source: https://github.com/vm0-ai/vm0-skills/blob/c2f02d7c1f3e0e8a25933f57587da9ffd7aa52fd/snowflake/SKILL.md
repo: vm0-ai/vm0-skills
kind: skill
stars: 66
last_pushed: 2026-06-16T10:01:37Z
license: unknown
score: 9
domains: [data-engineering, api-integration, sql]
tags: [snowflake, sql-api, curl]
curated: 2026-06-16
curated_by: config-scout
---

# vm0-ai/vm0-skills — skill

**Why it's worth keeping:** It includes specific remediation steps for common authentication failures and uses a robust pattern of writing JSON to temporary files to avoid shell-escaping issues during complex API calls.

**Summary:** Provides detailed curl templates and actionable troubleshooting steps for interacting with the Snowflake SQL API via programmatic access tokens.

**Source credibility:** The repository has respectable star counts for a specialized skills collection.

**Recency:** Current; aligns with modern Snowflake programmatic access patterns.

**Source:** [vm0-ai/vm0-skills/snowflake/SKILL.md](https://github.com/vm0-ai/vm0-skills/blob/c2f02d7c1f3e0e8a25933f57587da9ffd7aa52fd/snowflake/SKILL.md) · 66★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
---
name: snowflake
description: Snowflake API for data warehouse operations. Use when user mentions "Snowflake", "data warehouse", "SQL API", "warehouse", "database", "schema", or asks to query Snowflake data.
---

## Troubleshooting

If requests fail, run `zero doctor check-connector --env-name SNOWFLAKE_PAT` or `zero doctor check-connector --url https://$SNOWFLAKE_ACCOUNT.snowflakecomputing.com/api/v2/databases --method GET`

### Error 390432: `Network policy is required`

Snowflake refuses PAT authentication for any user that is not bound to a network policy. The account admin must attach one before the PAT can authenticate. Steps (perform in Snowsight):

1. Open [https://app.snowflake.com](https://app.snowflake.com) and sign in with an `ACCOUNTADMIN` or `SECURITYADMIN` role.
2. In the left sidebar go to **Projects → Worksheets** and open (or create) a SQL worksheet.
3. Run `SHOW USERS;` and note the value in the `name` column for the PAT-owning user.
4. Run the policy creation statement on its own:

   ```sql
   CREATE NETWORK POLICY pat_policy ALLOWED_IP_LIST = ('0.0.0.0/0');
   ```

5. Then run the user binding statement on its own (replace `USER_NAME` with the value from st
```

</details>
