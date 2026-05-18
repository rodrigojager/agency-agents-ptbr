# 📋 Templates de Handoff NEXUS

> Templates padronizados para todo tipo de handoff agente-para-agente no pipeline NEXUS. Handoffs consistentes previnem perda de contexto — a causa nº 1 de falha em coordenação multiagente.

---

## 1. Template Padrão de Handoff

Use para qualquer transferência de trabalho entre agentes.

```markdown
# Documento de Handoff NEXUS

## Metadados
| Campo | Valor |
|-------|-------|
| **De** | [Nome do Agente] ([Divisão]) |
| **Para** | [Nome do Agente] ([Divisão]) |
| **Fase** | Fase [N] — [Nome da Fase] |
| **Referência da Tarefa** | [ID da tarefa no backlog do Sprint Prioritizer] |
| **Prioridade** | [Crítica / Alta / Média / Baixa] |
| **Timestamp** | [YYYY-MM-DDTHH:MM:SSZ] |

## Contexto
**Projeto**: [Nome do projeto]
**Estado Atual**: [O que foi concluído até agora — seja específico]
**Arquivos Relevantes**:
- [file/path/1] — [o que contém]
- [file/path/2] — [o que contém]
**Dependências**: [Do que este trabalho depende para estar completo]
**Restrições**: [Restrições técnicas, de timeline ou de recursos]

## Solicitação de Entregável
**O que é necessário**: [Descrição específica e mensurável do entregável]
**Critérios de aceitação**:
- [ ] [Critério 1 — mensurável]
- [ ] [Critério 2 — mensurável]
- [ ] [Critério 3 — mensurável]
**Materiais de referência**: [Links para specs, designs, trabalho anterior]

## Expectativas de Qualidade
**Precisa passar**: [Critérios específicos de qualidade para este entregável]
**Evidência obrigatória**: [Como é a prova de conclusão]
**Handoff para o próximo**: [Quem recebe o output e em qual formato precisa]
```

---

## 2. Loop de Feedback de QA — PASS

Use quando Evidence Collector ou outro agente de QA aprovar uma tarefa.

```markdown
# Veredito QA NEXUS: PASS ✅

## Tarefa
| Campo | Valor |
|-------|-------|
| **Task ID** | [ID] |
| **Descrição da Tarefa** | [Descrição] |
| **Developer Agent** | [Nome do Agente] |
| **QA Agent** | [Nome do Agente] |
| **Tentativa** | [N] de 3 |
| **Timestamp** | [YYYY-MM-DDTHH:MM:SSZ] |

## Veredito: PASS

## Evidência
**Screenshots**:
- Desktop (1920x1080): [filename/path]
- Tablet (768x1024): [filename/path]
- Mobile (375x667): [filename/path]

**Verificação Funcional**:
- [x] [Critério de aceitação 1] — verificado
- [x] [Critério de aceitação 2] — verificado
- [x] [Critério de aceitação 3] — verificado

**Consistência de Marca**: Verificada — cores, tipografia, spacing batem com o design system
**Acessibilidade**: Verificada — navegação por teclado, contrast ratios, HTML semântico
**Performance**: [Tempo de carregamento medido] — dentro da faixa aceitável

## Observações
[Quaisquer observações, sugestões menores para melhoria futura ou destaques positivos]

## Próxima Ação
→ Agents Orchestrator: Marcar tarefa como completa, avançar para a próxima tarefa no backlog
```

---

## 3. Loop de Feedback de QA — FAIL

Use quando Evidence Collector ou outro agente de QA rejeitar uma tarefa.

```markdown
# Veredito QA NEXUS: FAIL ❌

## Tarefa
| Campo | Valor |
|-------|-------|
| **Task ID** | [ID] |
| **Descrição da Tarefa** | [Descrição] |
| **Developer Agent** | [Nome do Agente] |
| **QA Agent** | [Nome do Agente] |
| **Tentativa** | [N] de 3 |
| **Timestamp** | [YYYY-MM-DDTHH:MM:SSZ] |

## Veredito: FAIL

## Issues Encontradas

### Issue 1: [Categoria] — [Severidade: Crítica/Alta/Média/Baixa]
**Descrição**: [Descrição exata do problema]
**Esperado**: [O que deveria acontecer segundo os critérios de aceitação]
**Atual**: [O que realmente acontece]
**Evidência**: [Nome do arquivo de screenshot ou output de teste]
**Instrução de fix**: [Instrução específica e acionável para resolver]
**Arquivo(s) a modificar**: [Paths exatos dos arquivos]

### Issue 2: [Categoria] — [Severidade]
**Descrição**: [...]
**Esperado**: [...]
**Atual**: [...]
**Evidência**: [...]
**Instrução de fix**: [...]
**Arquivo(s) a modificar**: [...]

[Continue para todas as issues encontradas]

## Status dos Critérios de Aceitação
- [x] [Critério 1] — passou
- [ ] [Critério 2] — FALHOU (ver Issue 1)
- [ ] [Critério 3] — FALHOU (ver Issue 2)

## Instruções de Retry
**Para Developer Agent**:
1. Corrija APENAS as issues listadas acima
2. NÃO introduza novas features ou mudanças
3. Reenvie para QA quando todas as issues forem tratadas
4. Esta é a tentativa [N] de 3 no máximo

**Se a tentativa 3 falhar**: A tarefa será escalada para Agents Orchestrator
```

---

## 4. Relatório de Escalonamento

Use quando uma tarefa exceder 3 tentativas de retry.

```markdown
# Relatório de Escalonamento NEXUS 🚨

## Tarefa
| Campo | Valor |
|-------|-------|
| **Task ID** | [ID] |
| **Descrição da Tarefa** | [Descrição] |
| **Developer Agent** | [Nome do Agente] |
| **QA Agent** | [Nome do Agente] |
| **Tentativas Esgotadas** | 3/3 |
| **Escalonamento Para** | [Agents Orchestrator / Studio Producer] |
| **Timestamp** | [YYYY-MM-DDTHH:MM:SSZ] |

## Histórico de Falhas

### Tentativa 1
- **Issues encontradas**: [Resumo]
- **Fixes aplicados**: [O que o developer mudou]
- **Resultado**: FAIL — [Por que ainda falhou]

### Tentativa 2
- **Issues encontradas**: [Resumo]
- **Fixes aplicados**: [O que o developer mudou]
- **Resultado**: FAIL — [Por que ainda falhou]

### Tentativa 3
- **Issues encontradas**: [Resumo]
- **Fixes aplicados**: [O que o developer mudou]
- **Resultado**: FAIL — [Por que ainda falhou]

## Análise de Causa Raiz
**Por que a tarefa continua falhando**: [Análise do problema subjacente]
**Issue sistêmica**: [Isso é pontual ou um padrão?]
**Avaliação de complexidade**: [A tarefa foi escopada adequadamente?]

## Resolução Recomendada
- [ ] **Reatribuir** a outro developer agent ([agente recomendado])
- [ ] **Decompor** em subtarefas menores ([breakdown proposto])
- [ ] **Revisar abordagem** — mudança de arquitetura/design necessária
- [ ] **Aceitar** estado atual com limitações documentadas
- [ ] **Adiar** para sprint futuro

## Avaliação de Impacto
**Bloqueio**: [Quais outras tarefas são bloqueadas por isso]
**Impacto na Timeline**: [Como isso afeta o cronograma geral]
**Impacto de Qualidade**: [Quais compromissos de qualidade existem se aceitarmos o estado atual]

## Decisão Obrigatória
**Decisor**: [Agents Orchestrator / Studio Producer]
**Prazo**: [Quando a decisão é necessária para evitar mais atraso]
```

---

## 5. Handoff de Phase Gate

Use ao transicionar entre fases NEXUS.

```markdown
# Handoff de Phase Gate NEXUS

## Transição
| Campo | Valor |
|-------|-------|
| **Da Fase** | Fase [N] — [Nome] |
| **Para a Fase** | Fase [N+1] — [Nome] |
| **Gate Keeper(s)** | [Nome(s) do(s) Agente(s)] |
| **Resultado do Gate** | [PASSED / FAILED] |
| **Timestamp** | [YYYY-MM-DDTHH:MM:SSZ] |

## Resultados dos Critérios do Gate
| # | Critério | Threshold | Resultado | Evidência |
|---|-----------|-----------|--------|----------|
| 1 | [Critério] | [Threshold] | ✅ PASS / ❌ FAIL | [Referência de evidência] |
| 2 | [Critério] | [Threshold] | ✅ PASS / ❌ FAIL | [Referência de evidência] |
| 3 | [Critério] | [Threshold] | ✅ PASS / ❌ FAIL | [Referência de evidência] |

## Documentos Carregados Adiante
1. [Nome do documento] — [Finalidade para a próxima fase]
2. [Nome do documento] — [Finalidade para a próxima fase]
3. [Nome do documento] — [Finalidade para a próxima fase]

## Restrições-Chave para a Próxima Fase
- [Restrição 1 a partir dos findings desta fase]
- [Restrição 2 a partir dos findings desta fase]

## Ativação de Agentes para a Próxima Fase
| Agente | Papel | Prioridade |
|-------|------|----------|
| [Agente 1] | [Papel na próxima fase] | [Imediato / Dia 2 / Conforme necessário] |
| [Agente 2] | [Papel na próxima fase] | [Imediato / Dia 2 / Conforme necessário] |

## Riscos Carregados Adiante
| Risco | Severidade | Mitigação | Owner |
|------|----------|------------|-------|
| [Risco] | [P0-P3] | [Plano de mitigação] | [Agente] |
```

---

## 6. Handoff de Sprint

Use nas fronteiras de sprint.

```markdown
# Handoff de Sprint NEXUS

## Sumário do Sprint
| Campo | Valor |
|-------|-------|
| **Sprint** | [Número] |
| **Duração** | [Data de início] → [Data final] |
| **Objetivo do Sprint** | [Declaração do objetivo] |
| **Velocity** | [Planejada] / [Real] story points |

## Status de Conclusão
| Task ID | Descrição | Status | Tentativas de QA | Observações |
|---------|-------------|--------|-------------|-------|
| [ID] | [Descrição] | ✅ Complete | [N] | [Observações] |
| [ID] | [Descrição] | ✅ Complete | [N] | [Observações] |
| [ID] | [Descrição] | ⚠️ Carried Over | [N] | [Motivo] |

## Métricas de Qualidade
- **Taxa de QA first-pass**: [X]%
- **Média de retries**: [N]
- **Tarefas concluídas**: [X/Y]
- **Story points entregues**: [N]

## Carregado para o Próximo Sprint
| Task ID | Descrição | Motivo | Prioridade |
|---------|-------------|--------|----------|
| [ID] | [Descrição] | [Por que não foi concluída] | [Score RICE] |

## Insights da Retrospectiva
**O que foi bem**: [Principais sucessos]
**O que melhorar**: [Principais melhorias]
**Itens de ação**: [Mudanças específicas para o próximo sprint]

## Preview do Próximo Sprint
**Objetivo do sprint**: [Objetivo proposto]
**Tarefas-chave**: [Itens de maior prioridade]
**Dependências**: [Dependências cross-team]
```

---

## 7. Handoff de Incidente

Use durante incident response.

```markdown
# Handoff de Incidente NEXUS

## Incidente
| Campo | Valor |
|-------|-------|
| **Severidade** | [P0 / P1 / P2 / P3] |
| **Detectado por** | [Agente ou sistema] |
| **Horário de detecção** | [Timestamp] |
| **Atribuído a** | [Nome do Agente] |
| **Status** | [Investigating / Mitigating / Resolved / Post-mortem] |

## Descrição
**O que aconteceu**: [Descrição clara do incidente]
**Impacto**: [Quem/o que foi afetado e com qual severidade]
**Timeline**:
- [HH:MM] — [Evento]
- [HH:MM] — [Evento]
- [HH:MM] — [Evento]

## Estado Atual
**Sistemas afetados**: [Lista]
**Workaround disponível**: [Sim/Não — descreva se sim]
**Estimativa de resolução**: [Estimativa de tempo]

## Ações Tomadas
1. [Ação tomada e resultado]
2. [Ação tomada e resultado]

## Contexto de Handoff
**Para o próximo responder**:
- [O que já foi tentado]
- [O que ainda não foi tentado]
- [Causa raiz suspeita]
- [Logs/métricas relevantes a checar]

## Comunicação com Stakeholders
**Último update enviado**: [Timestamp]
**Próximo update até**: [Timestamp]
**Canal de comunicação**: [Onde updates são publicados]
```

---

## Guia de Uso

| Situação | Template a Usar |
|-----------|----------------|
| Atribuir trabalho a outro agente | Handoff Padrão (#1) |
| QA aprova uma tarefa | QA PASS (#2) |
| QA rejeita uma tarefa | QA FAIL (#3) |
| Tarefa excede 3 retries | Relatório de Escalonamento (#4) |
| Mover entre fases | Handoff de Phase Gate (#5) |
| Fim de sprint | Handoff de Sprint (#6) |
| Incidente de sistema | Handoff de Incidente (#7) |
