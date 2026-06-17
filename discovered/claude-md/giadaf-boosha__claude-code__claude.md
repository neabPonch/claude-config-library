---
name: giadaf-boosha__claude-code__claude
source: https://github.com/giadaf-boosha/claude-code/blob/bd0ae06c4eb7d660ac92771aab8c69173aec92bb/examples/personas/8-legacy-stack/CLAUDE.md
repo: giadaf-boosha/claude-code
kind: claude-md
stars: 6
last_pushed: 2026-06-15T05:12:13Z
license: unknown
score: 8
domains: [legacy-systems, enterprise]
tags: [legacy, ibm-i, rpg, modernization]
curated: 2026-06-15
curated_by: config-scout
---

# giadaf-boosha/claude-code — claude-md

**Why it's worth keeping:** It implements strict 'anti-failure' rules to prevent syntax/opcode hallucinations in older languages and establishes essential safety boundaries for production environments.

**Summary:** A specialized template for managing and modernizing legacy enterprise systems such as IBM i (RPG) or COBOL.

**Source credibility:** Low social proof via repository metrics, but content demonstrates high domain-specific expertise.

**Recency:** Current; accounts for modern large-context window capabilities.

**Source:** [giadaf-boosha/claude-code/examples/personas/8-legacy-stack/CLAUDE.md](https://github.com/giadaf-boosha/claude-code/blob/bd0ae06c4eb7d660ac92771aab8c69173aec92bb/examples/personas/8-legacy-stack/CLAUDE.md) · 6★

<details><summary>Excerpt (first 1200 chars)</summary>

```markdown
# Sistema: <nome legacy>

## Stack (esempio RPG; adatta al tuo)
- IBM i 7.5, RPGLE free + RPGLE fixed-form, CL programs
- DB2 for i, file fisici/logici + SQL
- Build: PDM / RDi
- (Alternativa COBOL: COBOL Enterprise + JCL + DB2 z/OS)
- (Alternativa .NET: .NET Framework 4.8 WebForms + WCF)
- (Alternativa Java EE: Java 8 + Struts 1 + EJB 2.1 + WebLogic 10)

## Regole anti-fallimento (rigide)
- LEGGI sempre il sorgente prima di proporre modifiche
- Non inventare opcode RPG / verbi COBOL: verifica nei manuali IBM/Microsoft
- Non assumere semantica di file logici: leggi DDS
- Cita sempre member:linea quando referenzi codice
- Modernizzazione = strangler fig, non rewrite

## Boundary
- Niente modifiche dirette su QGPL / produzione
- Output in libreria DEV; promozione manuale
- Backup membro prima di ogni edit
- Mai DROP / DELETE su tabelle senza approvazione DBA

## Documentazione
- Ogni programma esplorato → docs/legacy/<NOME>.md
- Diagrammi flusso in mermaid

## Output style
- "Explanatory" attivo: spiega il *perche'* del codice legacy
- 1M context per caricare interi sorgenti (4000+ righe)
```

</details>
