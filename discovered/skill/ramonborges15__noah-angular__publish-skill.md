---
name: ramonborges15__noah-angular__publish-skill
source: https://github.com/ramonborges15/noah-angular/blob/611672683d04483f8d0db1ebd55d898f1c5e8214/PUBLISH_SKILL.md
repo: ramonborges15/noah-angular
kind: skill
stars: 1
last_pushed: 2026-02-18T20:16:10Z
license: mit
score: 7
domains: [web-frontend, devops, cli-tools]
tags: [angular, npm, semantic-versioning, github-actions]
curated: 2026-06-15
curated_by: config-scout
---

# ramonborges15/noah-angular — skill

**Why it's worth keeping:** The prompt structure is excellent; it breaks a high-stakes DevOps sequence into discrete, verifiable steps that an agent can execute reliably. It provides specific command patterns (like annotated tags) rather than vague instructions.

**Summary:** Automates the manual process of semantic versioning, changelog updates, and Git tagging required to trigger an NPM publication via GitHub Actions.

**Source credibility:** Personal/small project repository with low social proof.

**Recency:** Current; follows modern Git and CI/CD best practices.

**Source:** [ramonborges15/noah-angular/PUBLISH_SKILL.md](https://github.com/ramonborges15/noah-angular/blob/611672683d04483f8d0db1ebd55d898f1c5e8214/PUBLISH_SKILL.md) · 1★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Skill: Publicar Biblioteca Angular no NPM

## Objetivo
Publicar automaticamente a biblioteca `@ramonbsales/noah-angular` no npm usando GitHub Actions com versionamento semântico.

## Pré-requisitos Únicos (Fazer uma vez)

### 1. Configurar NPM Token no GitHub

```bash
# No NPM (https://www.npmjs.com/settings/ramonbsales/tokens):
# - Generate New Token → Automation
# - Copiar token

# No GitHub (settings/secrets/actions):
# - New repository secret
# - Name: NPM_TOKEN
# - Value: [Cole o token]
```

### 2. Verificar arquivo de workflow

O workflow deve estar em `.github/workflows/publish.yml` com:
- Trigger: `on: push tags: 'v*.*.*'` (recomendado — corresponde ao semver)
- Build: `ng build shared-components --configuration=production`
- Publish: authenticado com `NPM_TOKEN`

Nota: o workflow atual também aceita `v*` (mais permissivo). Recomendo alinhar a documentação e o workflow para usar `v*.*.*` se você quer forçar tags no formato semântico.

## Processo de Publicação (Repetir a cada release)

### Passos Executar

1. **Atualizar versão no package.json:**
   - Arquivo: `projects/shared-components/package.json`
   - Campo: `"version": "X.Y.Z"`
   - Seguir semântico: `MAJOR.MINOR.PA
```

</details>
