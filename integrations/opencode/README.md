# Integração com OpenCode

Agentes OpenCode são arquivos `.md` com YAML frontmatter armazenados em
`.opencode/agents/`. O conversor mapeia cores nomeadas para códigos hex e adiciona
`mode: subagent` para que agentes sejam invocados sob demanda via `@agent-name`, em vez
de poluir o seletor principal de agentes.

## Instalação

```bash
# Execute a partir da raiz do seu projeto
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool opencode
```

Isso cria arquivos `.opencode/agents/<slug>.md` no diretório do seu projeto.

## Ativar um Agente

No OpenCode, invoque um subagent com o prefixo `@`:

```
@frontend-developer help build this component.
```

```
@reality-checker review this PR.
```

Você também pode selecionar agentes pela UI de seletor de agentes do OpenCode.

## Formato do Agente

Cada arquivo de agente gerado contém:

```yaml
---
name: Frontend Developer
description: Expert frontend developer specializing in modern web technologies...
mode: subagent
color: "#00FFFF"
---
```

- **mode: subagent** — agente fica disponível sob demanda, não aparece na lista principal percorrida com Tab
- **color** — código hex (cores nomeadas dos arquivos fonte são convertidas automaticamente)

## Projeto vs Global

Agentes em `.opencode/agents/` têm **escopo de projeto**. Para deixá-los disponíveis
globalmente em todos os projetos, primeiro gere os arquivos de agentes e depois instale
com `--path`:

```bash
./scripts/convert.sh --tool opencode
./scripts/install.sh --tool opencode --path ~/.config/opencode/agents
```

## Regenerar

```bash
./scripts/convert.sh --tool opencode
```
