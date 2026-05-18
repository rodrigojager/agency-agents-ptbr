# 🔌 Integrações

Este diretório contém as integrações da The Agency e formatos convertidos para
ferramentas de coding agentic suportadas.

## Ferramentas Suportadas

- **[Claude Code](#claude-code)** — agentes `.md`, use o repo diretamente
- **[GitHub Copilot](#github-copilot)** — agentes `.md`, use o repo diretamente
- **[Antigravity](#antigravity)** — `SKILL.md` por agente em `antigravity/`
- **[Gemini CLI](#gemini-cli)** — extensão + arquivos `SKILL.md` em `gemini-cli/`
- **[OpenCode](#opencode)** — arquivos de agente `.md` em `opencode/`
- **[OpenClaw](#openclaw)** — workspaces `SOUL.md` + `AGENTS.md` + `IDENTITY.md`
- **[Cursor](#cursor)** — arquivos de regras `.mdc` em `cursor/`
- **[Aider](#aider)** — `CONVENTIONS.md` em `aider/`
- **[Windsurf](#windsurf)** — `.windsurfrules` em `windsurf/`
- **[Kimi Code](#kimi-code)** — specs YAML de agentes em `kimi/`
- **[Qwen Code](#qwen-code)** — SubAgents `.md` com escopo de projeto em `.qwen/agents/`

## Instalação Rápida

```bash
# Instale automaticamente para todas as ferramentas detectadas
./scripts/install.sh

# Instale uma ferramenta específica com escopo home
./scripts/install.sh --tool antigravity
./scripts/install.sh --tool copilot
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool claude-code

# Gemini CLI precisa de arquivos de integração gerados em um clone novo
./scripts/convert.sh --tool gemini-cli
./scripts/install.sh --tool gemini-cli

# Qwen Code também precisa de arquivos SubAgent gerados em um clone novo
./scripts/convert.sh --tool qwen
./scripts/install.sh --tool qwen
```

Se você instalar o OpenClaw e o gateway já estiver rodando, reinicie-o após a instalação:

```bash
openclaw gateway restart
```

Para ferramentas com escopo de projeto, como OpenCode, Cursor, Aider, Windsurf e Qwen
Code, execute
o instalador a partir da raiz do seu projeto alvo, como mostrado nas seções
específicas por ferramenta abaixo.

## Regenerando Arquivos de Integração

Se você adicionar ou modificar agentes, regenere todos os arquivos de integração:

```bash
./scripts/convert.sh
```

---

## Claude Code

The Agency foi originalmente desenhada para Claude Code. Os agentes funcionam nativamente
sem conversão.

```bash
cp -r <category>/*.md ~/.claude/agents/
# ou instale tudo de uma vez:
./scripts/install.sh --tool claude-code
```

Veja [claude-code/README.md](claude-code/README.md) para detalhes.

---

## GitHub Copilot

The Agency também funciona nativamente com GitHub Copilot. Agentes podem ser copiados
diretamente para `~/.github/agents/` e `~/.copilot/agents/` sem conversão.

```bash
./scripts/install.sh --tool copilot
```

Veja [github-copilot/README.md](github-copilot/README.md) para detalhes.

---

## Antigravity

Skills são instaladas em `~/.gemini/antigravity/skills/`. Cada agente vira
uma skill separada com prefixo `agency-` para evitar conflitos de nome.

```bash
./scripts/install.sh --tool antigravity
```

Veja [antigravity/README.md](antigravity/README.md) para detalhes.

---

## Gemini CLI

Agentes são empacotados como uma extensão do Gemini CLI com arquivos de skill individuais.
A extensão é instalada em `~/.gemini/extensions/agency-agents/`.
Como o manifest do Gemini e as pastas de skills são artefatos gerados, execute
`./scripts/convert.sh --tool gemini-cli` antes de instalar a partir de um clone novo.

```bash
./scripts/convert.sh --tool gemini-cli
./scripts/install.sh --tool gemini-cli
```

Veja [gemini-cli/README.md](gemini-cli/README.md) para detalhes.

---

## OpenCode

Cada agente vira um arquivo `.md` com escopo de projeto em `.opencode/agents/`.

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool opencode
```

Veja [opencode/README.md](opencode/README.md) para detalhes.

---

## OpenClaw

Cada agente vira um workspace OpenClaw contendo `SOUL.md`, `AGENTS.md`
e `IDENTITY.md`.

Antes de instalar, gere os workspaces OpenClaw:

```bash
./scripts/convert.sh --tool openclaw
```

Então instale:

```bash
./scripts/install.sh --tool openclaw
```

Veja [openclaw/README.md](openclaw/README.md) para detalhes.

---

## Cursor

Cada agente vira um arquivo de rule `.mdc`. Rules têm escopo de projeto — execute o
instalador a partir da raiz do seu projeto.

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool cursor
```

Veja [cursor/README.md](cursor/README.md) para detalhes.

---

## Aider

Todos os agentes são consolidados em um único arquivo `CONVENTIONS.md` que o Aider
lê automaticamente quando está presente na raiz do seu projeto.

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool aider
```

Veja [aider/README.md](aider/README.md) para detalhes.

---

## Windsurf

Todos os agentes são consolidados em um único arquivo `.windsurfrules` para a
raiz do seu projeto.

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool windsurf
```

Veja [windsurf/README.md](windsurf/README.md) para detalhes.

---

## Kimi Code

Cada agente é convertido para uma especificação de agente Kimi Code CLI (formato YAML com
arquivos separados de system prompt). Agentes são instalados em `~/.config/kimi/agents/`.

Como os arquivos de agente Kimi são gerados a partir do Markdown fonte, execute
`./scripts/convert.sh --tool kimi` antes de instalar a partir de um clone novo.

```bash
./scripts/convert.sh --tool kimi
./scripts/install.sh --tool kimi
```

### Uso

Após a instalação, use um agente com a flag `--agent-file`:

```bash
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml
```

Ou em um projeto específico:

```bash
cd /your/project
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml \
     --work-dir /your/project
```

Veja [kimi/README.md](kimi/README.md) para detalhes.

---

## Qwen Code

Cada agente vira um arquivo SubAgent `.md` com escopo de projeto em `.qwen/agents/`.

A partir de um clone novo, gere primeiro os arquivos Qwen:

```bash
./scripts/convert.sh --tool qwen
```

Depois instale a partir da raiz do seu projeto:

```bash
cd /your/project && /path/to/agency-agents/scripts/install.sh --tool qwen
```

Veja [qwen/README.md](qwen/README.md) para detalhes.
