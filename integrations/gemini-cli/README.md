# Integração com Gemini CLI

Empacota todos os 61 agentes da Agency como uma extensão do Gemini CLI. A extensão
é instalada em `~/.gemini/extensions/agency-agents/`.

## Instalação

```bash
# Gere primeiro os arquivos de integração do Gemini CLI
./scripts/convert.sh --tool gemini-cli

# Depois instale a extensão
./scripts/install.sh --tool gemini-cli
```

## Ativar uma Skill

No Gemini CLI, referencie um agente pelo nome:

```
Use the frontend-developer skill to help me build this UI.
```

## Estrutura da Extensão

```
~/.gemini/extensions/agency-agents/
  gemini-extension.json
  skills/
    frontend-developer/SKILL.md
    backend-architect/SKILL.md
    reality-checker/SKILL.md
    ...
```

## Regenerar

```bash
./scripts/convert.sh --tool gemini-cli
```
