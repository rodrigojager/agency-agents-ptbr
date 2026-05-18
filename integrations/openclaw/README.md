# Integração com OpenClaw

Agentes OpenClaw são instalados como workspaces contendo arquivos `SOUL.md`, `AGENTS.md`
e `IDENTITY.md`. O instalador copia cada workspace para
`~/.openclaw/agency-agents/` e o registra quando o CLI `openclaw` está
disponível.

Antes de instalar, gere os workspaces OpenClaw:

```bash
./scripts/convert.sh --tool openclaw
```

## Instalação

```bash
./scripts/install.sh --tool openclaw
```

## Ativar um Agente

Após a instalação, agentes ficam disponíveis por `agentId` nas sessões OpenClaw.

Se o gateway OpenClaw já estiver rodando, reinicie-o após a instalação:

```bash
openclaw gateway restart
```

## Regenerar

```bash
./scripts/convert.sh --tool openclaw
```
