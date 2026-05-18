# Integração com Aider

O roster completo da Agency é consolidado em um único arquivo `CONVENTIONS.md`.
O Aider lê esse arquivo automaticamente quando ele está presente na raiz do seu projeto.

## Instalação

```bash
# Execute a partir da raiz do seu projeto
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool aider
```

## Ativar um Agente

Na sua sessão do Aider, referencie o agente pelo nome:

```
Use the Frontend Developer agent to refactor this component.
```

```
Apply the Reality Checker agent to verify this is production-ready.
```

## Uso Manual

Você também pode passar o arquivo de convenções diretamente:

```bash
aider --read CONVENTIONS.md
```

## Regenerar

```bash
./scripts/convert.sh --tool aider
```
