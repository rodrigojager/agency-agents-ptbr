# Progresso da Tradução pt-BR dos Agentes

Este documento registra o andamento da tradução **manual** dos agentes para português brasileiro, com foco em contexto e semântica.

## Objetivo
> **Importante:** este fluxo é 100% manual. Não usar scripts automáticos de tradução.

- Traduzir os arquivos de agentes (`*.md`) para pt-BR com qualidade editorial.
- Preservar termos em inglês quando forem realmente naturais no uso brasileiro (ex.: bug, commit, push, deploy, issue, branch, pull request, merge request, CEO, mouse).
- Manter consistência entre sessões futuras de trabalho.

## Diretrizes de Tradução (padrão do projeto)
1. **Tradução manual e contextual**
   - Não fazer substituição palavra-por-palavra.
   - Priorizar sentido do trecho no contexto do agente.

2. **Preservação de termos técnicos (quando natural no Brasil)**
   - Manter em inglês: bug, commit, push, deploy, issue, branch, pull request, merge request, CEO, mouse.
   - Avaliar caso a caso outros termos técnicos conforme contexto.

3. **Tom e estilo**
   - Preservar a personalidade do agente.
   - Manter tom profissional, direto e claro.

4. **Estrutura do arquivo**
   - Manter frontmatter YAML (`name`, `description`, `color`, `emoji`, `vibe`).
   - Manter seções, listas, blocos de código e templates técnicos.
   - Traduzir títulos e conteúdo, sem quebrar formatação Markdown.

5. **Nomenclatura de agentes**
   - Traduzir `name` quando houver equivalente natural em pt-BR.
   - Não forçar tradução estranha de nomes técnicos.

6. **Qualidade mínima antes de concluir um arquivo**
   - Revisar fluidez em pt-BR.
   - Verificar consistência terminológica.
   - Confirmar que não há trechos em “portunhol técnico”/mistura artificial.

## Status Atual

### Concluídos
- [x] `design/design-brand-guardian.md`
- [x] `design/design-ui-designer.md`
- [x] `design/design-ux-researcher.md`
- [x] `design/design-ux-architect.md`
- [x] `design/design-image-prompt-engineer.md`
- [x] `design/design-inclusive-visuals-specialist.md`
- [x] `design/design-whimsy-injector.md`
- [x] `design/design-visual-storyteller.md`
- [x] `academic/academic-anthropologist.md`
- [x] `academic/academic-geographer.md`
- [x] `academic/academic-historian.md`
- [x] `engineering/engineering-code-reviewer.md`
- [x] `engineering/engineering-ai-engineer.md`
- [x] `engineering/engineering-ai-data-remediation-engineer.md`

### Em andamento
- [ ] _(nenhum no momento)_

### Pendentes (demais agentes)
- [ ] Todos os agentes das pastas: `design/`, `engineering/`, `finance/`, `game-development/`, `marketing/`, `paid-media/`, `product/`, `project-management/`, `sales/`, `spatial-computing/`, `specialized/`, `support/`, `testing/`.

## Como retomar a tradução em uma próxima sessão
1. Abrir este arquivo: `TRANSLATION_PROGRESS_pt-BR.md`.
2. Continuar a partir da seção **Em andamento**.
3. Ao concluir um agente:
   - mover para **Concluídos**;
   - remover de **Em andamento/Pendentes**;
   - manter as diretrizes acima sem exceções.
4. Fazer commit com mensagem explícita, por exemplo:
   - `Manually translate academic-historian agent to pt-BR`

## Regra de ouro
Se houver dúvida entre “tradução literal” e “naturalidade em pt-BR”, escolher sempre a redação mais natural **sem perder precisão técnica**.
