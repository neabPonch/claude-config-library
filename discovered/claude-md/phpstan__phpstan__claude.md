---
name: phpstan__phpstan__claude
source: https://github.com/phpstan/phpstan/blob/d3044dc09891688a0b63972571ed18e6377c1022/website/infra/CLAUDE.md
repo: phpstan/phpstan
kind: claude-md
stars: 13997
last_pushed: 2026-06-15T05:25:17Z
license: mit
score: 9
domains: [infrastructure, aws-cdk]
tags: [aws, typescript, iac, cloudfront]
curated: 2026-06-15
curated_by: config-scout
---

# phpstan/phpstan — claude-md

**Why it's worth keeping:** It encodes complex runtime redirect/rewrite rules that are not easily inferred from code alone; it also provides a high-utility 'When to edit what' guide.

**Summary:** Defines the AWS CDK infrastructure for phpstan.org, detailing stack architectures and critical CloudFront edge function rewrite logic.

**Source credibility:** Extremely high; part of the highly-regarded, well-maintained phpstan/phpstan repository.

**Recency:** Current; uses modern patterns like CloudFront Function 2.0 and OIDC for GitHub Actions.

**Source:** [phpstan/phpstan/website/infra/CLAUDE.md](https://github.com/phpstan/phpstan/blob/d3044dc09891688a0b63972571ed18e6377c1022/website/infra/CLAUDE.md) · 13997★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# phpstan.org website infrastructure (CDK)

AWS CDK app (TypeScript) that defines the production infra for [phpstan.org](https://phpstan.org):
S3 origin, CloudFront distribution, edge function, security headers policy,
ACM cert, Route 53 records, and the IAM roles that GitHub Actions assumes via OIDC.

See `README.md` for the bootstrap and cutover runbook. See `../CLAUDE.md` for
the parent website project conventions.

## Stacks

Both stacks deploy to `us-east-1` (required for CloudFront + ACM).

| Stack | Defined in | Resources |
| --- | --- | --- |
| `PhpstanOrgGithubOidc` | `lib/github-oidc-stack.ts` | GitHub OIDC provider + `phpstan-org-infra-deploy` role (used by `website-infra.yml` to deploy this CDK app) |
| `PhpstanOrgWebsite` | `lib/website-stack.ts` | S3 bucket (OAC, private, versioned), CloudFront distribution carrying all three aliases (apex + www + `new.phpstan.org`), CF Function 2.0, Response Headers Policy, ACM cert (DNS-validated, covers all 3 hostnames), the `new.phpstan.org` Route 53 record, and `phpstan-org-website-deploy` role (used by `website.yml` to sync content + invalidate) |

`bin/infra.ts` is the CDK app entrypoint. It hard-codes the account/region/repo/z
```

</details>
