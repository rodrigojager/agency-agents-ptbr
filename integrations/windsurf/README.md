# Integração com Windsurf

O roster completo da Agency é consolidado em um único arquivo `.windsurfrules`.
As rules têm **escopo de projeto** — instale a partir da raiz do seu projeto.

## Instalação

```bash
# Execute a partir da raiz do seu projeto
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool windsurf
```

## Ativar um Agente

No Windsurf, referencie um agente pelo nome no seu prompt:

```
Use the Frontend Developer agent to build this component.
```

## Regenerar

```bash
./scripts/convert.sh --tool windsurf
```
