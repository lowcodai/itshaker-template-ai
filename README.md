# itshaker-template-ai

> Template pour projets IA, agents, MCP, prompts, RAG, LLM.

[![Governance](https://img.shields.io/badge/governance-itshaker-blue)](https://github.com/itshaker/itshaker-copilot-governance)

## Description

Template GitHub pour projets d'intelligence artificielle itshaker. Inclut tout `itshaker-template-base` plus :
- Structure agents, prompts, MCP, RAG
- Instructions de gouvernance IA (safety, prompt engineering)
- Hooks spécialisés IA (session-logger, attester-import-check)
- Workflow AI Safety Check
- Éléments Awesome Copilot IA (acreadiness, arize, agentic-eval…)

## Utilisation

```bash
cd itshaker-bootstrap
./scripts/new-project.sh --type ai --name <mon-projet-ia>
```

## Structure spécifique IA

```
.
├── agents/     # Fichiers .agent.md — définitions d'agents
├── prompts/    # Prompts versionnés avec métadonnées
├── mcp/        # Serveurs MCP (Model Context Protocol)
├── rag/        # Pipelines RAG (chunking, indexing, retrieval)
└── llm-wiki/   # Documentation des modèles et comportements observés
```

## Safety & Gouvernance IA

Tous les projets IA doivent respecter la politique `ai-usage-policy.md` de la gouvernance itshaker.

Avant chaque merge :
1. Review des prompts avec `ai-prompt-engineering-safety-review`
2. Validation des agents avec `agent-governance`
3. Compliance OWASP LLM Top 10 via `agent-owasp-compliance`

## Éléments Awesome Copilot spécifiques

| Élément | Type | Usage |
|---------|------|-------|
| `agent-safety.instructions.md` | Instruction | Safety pour agents |
| `ai-prompt-engineering-safety-best-practices.instructions.md` | Instruction | Safety prompts |
| `session-logger` | Hook | Log des sessions Copilot |
| `acreadiness-assess` | Skill | Évaluation maturité IA |
| `agent-governance` | Skill | Gouvernance agent |
| `agentic-eval` | Skill | Évaluation comportement agent |
| `ai-prompt-engineering-safety-review` | Skill | Review safety prompts |
| `agent-owasp-compliance` | Skill | OWASP LLM compliance |
| `arize-instrumentation` | Skill | Observabilité LLM |
| `acreadiness-cockpit` | Plugin | Tableau de bord maturité IA |

## Références

- [itshaker-copilot-governance](https://github.com/itshaker/itshaker-copilot-governance)
- [OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
- [github/awesome-copilot](https://github.com/github/awesome-copilot)
