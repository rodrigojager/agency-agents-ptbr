# Integração com Qwen Code

Qwen Code usa arquivos SubAgent `.md` com escopo de projeto em `.qwen/agents/`.

Os arquivos gerados vêm de `scripts/convert.sh --tool qwen`, que grava um arquivo
Markdown de SubAgent por agente da agency em `integrations/qwen/agents/`.

## Gerar

A partir da raiz do repositório:

```bash
./scripts/convert.sh --tool qwen
```

## Instalação

Execute o instalador a partir da raiz do seu projeto alvo:

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool qwen
```

Isso copia os arquivos SubAgent gerados para:

```text
.qwen/agents/
```

## Atualizar no Qwen Code

Após a instalação:

- execute `/agents manage` no Qwen Code para atualizar a lista de agentes, ou
- reinicie a sessão atual do Qwen Code

## Observações

- Qwen Code tem escopo de projeto, não escopo home
- Os arquivos Qwen gerados usam frontmatter mínimo: `name`, `description` e
  `tools` opcional
- Se você atualizar agentes neste repo, regenere o output Qwen antes de
  reinstalar
