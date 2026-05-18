# Integração com Cursor

Converte o roster completo da Agency em arquivos de regras `.mdc` para o Cursor. As rules têm
**escopo de projeto** — instale a partir da raiz do seu projeto.

## Instalação

```bash
# Execute a partir da raiz do seu projeto
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool cursor
```

Isso cria arquivos `.cursor/rules/<agent-slug>.mdc` no seu projeto.

## Ativar uma Rule

No Cursor, referencie um agente no seu prompt:

```
@frontend-developer Review this React component for performance issues.
```

Ou habilite uma rule como always-on editando o frontmatter:

```yaml
---
description: Expert frontend developer...
globs: "**/*.tsx,**/*.ts"
alwaysApply: true
---
```

## Regenerar

```bash
./scripts/convert.sh --tool cursor
```
