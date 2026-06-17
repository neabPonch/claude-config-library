---
name: jvsurmano123__maxima-agrossimula
source: https://github.com/jvsurmano123/maxima-agrossimula/blob/d57ab34226b846530d393eb725e60c9dab87f0c5/CLAUDE.MD
repo: jvsurmano123/maxima-agrossimula
kind: claude-md
stars: 0
last_pushed: 2026-04-04T04:51:17Z
license: unknown
score: 8
domains: [web-frontend, fintech]
tags: [rationale-driven, architectural-constraints, stack-definition]
curated: 2026-06-16
curated_by: config-scout
---

# jvsurmano123/maxima-agrossimula — claude-md

**Why it's worth keeping:** The 'What NOT to use' table and the 'Rationale' sections are elite patterns that prevent AI from suggesting incorrect or unwanted libraries.

**Summary:** Provides an exceptionally detailed technology stack including explicit rationales for architectural decisions.

**Source credibility:** Specific technical depth suggests a professional developer, despite low repository visibility.

**Recency:** Extremely current; references cutting-edge versions like React 19 and Tailwind v4.

**Source:** [jvsurmano123/maxima-agrossimula/CLAUDE.MD](https://github.com/jvsurmano123/maxima-agrossimula/blob/d57ab34226b846530d393eb725e60c9dab87f0c5/CLAUDE.MD) · 0★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
SEMPRE FALE COMIGO EM PT-BR.

<!-- GSD:project-start source:PROJECT.md -->
## Project

**Máxima Agrossimula**

Software de simulação e análise financeira para fazendas de pecuária e agricultura. Consultores da Máxima AgroNegócios inserem dados da propriedade (área, região, AEE efetiva, tipos de capim, efetividade de pastagem, maquinário, custos) e o sistema calcula automaticamente capacidade produtiva, DRE projetada, fluxo de caixa, VPL/TIR e cenários de "e se" com projeção de até 10 anos. Substitui planilhas manuais usadas hoje nos diagnósticos de R$50k+, gerando relatórios profissionais em PDF para entrega ao clientefinal.

**Core Value:** Inserir dados de uma fazenda e receber automaticamente cenários financeiros completos (DRE, caixa, VPL, TIR, stress tests) com projeção de até 10 anos — inteligência pronta para o consultor entregar ao cliente.

### Constraints

- **Plataforma**: Web — React + Supabase é a stack definida pelo usuário
- **Equipe**: Uso interno da equipe da Máxima (sem login de clientes)
- **Fórmulas**: Padrão com parâmetros variáveis por fazenda — não mudam por região
- **Dados de mercado**: Inputados manualmente pelo consultor, base editável no sistema
<!-- GSD
```

</details>
