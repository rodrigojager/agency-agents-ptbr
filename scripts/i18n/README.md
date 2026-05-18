# Localização em Chinês (zh-CN)

Localiza os campos `name` e `description` dos agentes no YAML frontmatter para chinês simplificado. Isso torna os nomes dos agentes legíveis no seletor de agentes do Copilot Chat para usuários que falam chinês.

## Arquivos

| Arquivo | Descrição |
|------|-------------|
| `agent-names-zh.json` | Mapeamento de nomes de agentes em inglês -> traduções em chinês (130+ entradas) |
| `localize-agents-zh.ps1` | Script PowerShell que lê o JSON e atualiza os arquivos de agentes instalados |

## Uso

Depois de instalar os agentes com `install.sh --tool copilot`:

```powershell
# Localiza os nomes dos agentes para chinês
powershell -ExecutionPolicy Bypass -File scripts/i18n/localize-agents-zh.ps1
```

Por padrão, o script processa:
- `%USERPROFILE%\.github\agents\`
- `%USERPROFILE%\.copilot\agents\`

Passe caminhos customizados se necessário:

```powershell
powershell -File scripts/i18n/localize-agents-zh.ps1 -TargetDirs @("C:\custom\path\agents")
```

## Como Funciona

1. Lê `agent-names-zh.json` (codificado em UTF-8) para obter o mapa de traduções
2. Para cada arquivo `.md` nos diretórios de destino:
   - Extrai o campo `name:` do YAML frontmatter
   - Procura a tradução em chinês
   - Substitui os campos `name:` e `description:`
   - Grava de volta como UTF-8

## Resultado

Antes:
```yaml
---
name: Security Engineer
description: Threat modeling, secure code review, security architecture
---
```

Depois:
```yaml
---
name: 安全工程师
description: 威胁建模、安全代码审查与应用安全架构专家
---
```

## Observações

- Modifica apenas **cópias instaladas** (em `~/.github/agents/`), não os arquivos fonte
- Execute novamente após cada atualização com `install.sh` (que sobrescreve com os originais em inglês)
- O arquivo JSON é a fonte única da verdade para traduções — adicione novos agentes nele
- O script é puro ASCII (evita problemas de encoding no PowerShell); todo o texto em chinês fica no JSON
