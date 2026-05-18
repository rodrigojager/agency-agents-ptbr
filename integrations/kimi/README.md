# Integração com Kimi Code CLI

Converte todos os agentes da Agency em especificações de agente para Kimi Code CLI. Cada agente
vira um diretório contendo `agent.yaml` (spec do agente) e `system.md` (system
prompt).

## Instalação

### Pré-requisitos

- [Kimi Code CLI](https://github.com/MoonshotAI/kimi-cli) instalado

### Instalar

```bash
# Gere os arquivos de integração (obrigatório em clone novo)
./scripts/convert.sh --tool kimi

# Instale os agentes
./scripts/install.sh --tool kimi
```

Isso copia os agentes para `~/.config/kimi/agents/`.

## Uso

### Ativar um Agente

Use a flag `--agent-file` para carregar um agente específico:

```bash
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml
```

### Em um Projeto

```bash
cd /your/project
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml \
     --work-dir /your/project \
     "Review this React component for performance issues"
```

### Listar Agentes Instalados

```bash
ls ~/.config/kimi/agents/
```

## Estrutura do Agente

Cada diretório de agente contém:

```
~/.config/kimi/agents/frontend-developer/
├── agent.yaml    # Especificação do agente (tools, subagents)
└── system.md     # System prompt com personalidade e instruções
```

### Formato de agent.yaml

```yaml
version: 1
agent:
  name: frontend-developer
  extend: default  # Herda do agente default built-in do Kimi
  system_prompt_path: ./system.md
  tools:
    - "kimi_cli.tools.shell:Shell"
    - "kimi_cli.tools.file:ReadFile"
    # ... todas as tools default
```

## Regenerar

Depois de modificar os agentes fonte:

```bash
./scripts/convert.sh --tool kimi
./scripts/install.sh --tool kimi
```

## Solução de Problemas

### Arquivo de agente não encontrado

Garanta que você executou `convert.sh` antes de `install.sh`:

```bash
./scripts/convert.sh --tool kimi
```

### Kimi CLI não detectado

Confira se `kimi` está no seu PATH:

```bash
which kimi
kimi --version
```

### YAML inválido

Valide os arquivos gerados:

```bash
python3 -c "import yaml; yaml.safe_load(open('integrations/kimi/frontend-developer/agent.yaml'))"
```
