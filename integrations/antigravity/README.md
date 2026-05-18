# Integração com Antigravity

Instala o roster completo da Agency como skills do Antigravity. Cada agente recebe o prefixo
`agency-` para evitar conflitos com skills existentes.

## Instalação

```bash
./scripts/install.sh --tool antigravity
```

Isso copia arquivos de `integrations/antigravity/` para
`~/.gemini/antigravity/skills/`.

## Ativar uma Skill

No Antigravity, ative um agente pelo slug:

```
Use the agency-frontend-developer skill to review this component.
```

Os slugs disponíveis seguem o padrão `agency-<agent-name>`, por exemplo:
- `agency-frontend-developer`
- `agency-backend-architect`
- `agency-reality-checker`
- `agency-growth-hacker`

## Regenerar

Depois de modificar agentes, regenere os arquivos de skills:

```bash
./scripts/convert.sh --tool antigravity
```

## Formato do Arquivo

Cada skill é um arquivo `SKILL.md` com frontmatter compatível com Antigravity:

```yaml
---
name: agency-frontend-developer
description: Expert frontend developer specializing in...
risk: low
source: community
date_added: '2026-03-08'
---
```
