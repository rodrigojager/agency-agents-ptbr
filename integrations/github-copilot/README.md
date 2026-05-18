# Integração com GitHub Copilot

The Agency funciona com GitHub Copilot out of the box. Não precisa de conversão —
os agentes usam o formato existente `.md` + YAML frontmatter.

## Instalação

```bash
# Copie todos os agentes para os diretórios de agentes do GitHub Copilot
./scripts/install.sh --tool copilot

# Ou copie manualmente uma categoria
cp engineering/*.md ~/.github/agents/
cp engineering/*.md ~/.copilot/agents/
```

## Ativar um Agente

Em qualquer sessão do GitHub Copilot, referencie um agente pelo nome:

```
Activate Frontend Developer and help me build a React component.
```

```
Use the Reality Checker agent to verify this feature is production-ready.
```

## Diretório de Agentes

Os agentes são organizados em divisões. Veja o [README principal](../../README.md) para
o roster completo atual.
