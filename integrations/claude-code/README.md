# Integração com Claude Code

The Agency foi criada para Claude Code. Não precisa de conversão — os agentes funcionam
nativamente com o formato existente `.md` + YAML frontmatter.

## Instalação

```bash
# Copie todos os agentes para o diretório de agentes do Claude Code
./scripts/install.sh --tool claude-code

# Ou copie manualmente uma categoria
cp engineering/*.md ~/.claude/agents/
```

## Ativar um Agente

Em qualquer sessão do Claude Code, referencie um agente pelo nome:

```
Activate Frontend Developer and help me build a React component.
```

```
Use the Reality Checker agent to verify this feature is production-ready.
```

## Diretório de Agentes

Os agentes são organizados em divisões. Veja o [README principal](../../README.md) para
o roster completo da Agency.
