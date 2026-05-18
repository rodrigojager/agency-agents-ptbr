# 🔨 Playbook Fase 3 — Build & Iterar

> **Duração**: 2-12 semanas (varia conforme o escopo) | **Agentes**: 15-30+ | **Gate Keeper**: Agents Orchestrator

---

## Objetivo

Implementar todas as features por loops contínuos Dev↔QA. Toda tarefa é validada antes de a próxima começar. É aqui que a maior parte do trabalho acontece — e onde a orquestração do NEXUS entrega mais valor.

## Pré-Condições

- [ ] Quality Gate da Fase 2 aprovado (fundação verificada)
- [ ] Backlog do Sprint Prioritizer disponível com scores RICE
- [ ] Pipeline CI/CD operacional
- [ ] Design system e biblioteca de componentes prontos
- [ ] Scaffold de API com sistema de auth pronto

## O Loop Dev↔QA — Mecânica Core

O Agents Orchestrator gerencia toda tarefa por este ciclo:

```
PARA CADA tarefa EM sprint_backlog (ordenado por score RICE):

  1. ATRIBUIR tarefa ao Developer Agent apropriado (ver matriz de atribuição)
  2. Developer IMPLEMENTA a tarefa
  3. Evidence Collector TESTA a tarefa
     - Screenshots visuais (desktop, tablet, mobile)
     - Verificação funcional contra critérios de aceitação
     - Checagem de consistência de marca
  4. IF veredito == PASS:
       Marcar tarefa como completa
       Mover para a próxima tarefa
     ELIF veredito == FAIL AND tentativas < 3:
       Enviar feedback de QA ao Developer
       Developer CORRIGE issues específicas
       Retornar ao passo 3
     ELIF tentativas >= 3:
       ESCALONAR para Agents Orchestrator
       Orchestrator decide: reatribuir, decompor, adiar ou aceitar
  5. ATUALIZAR relatório de status do pipeline
```

## Matriz de Atribuição de Agentes

### Atribuição Primária de Developer

| Categoria de Tarefa | Agente Primário | Agente Backup | Agente de QA |
|--------------|--------------|-------------|----------|
| **UI React/Vue/Angular** | Frontend Developer | Rapid Prototyper | Evidence Collector |
| **API REST/GraphQL** | Backend Architect | Senior Developer | API Tester |
| **Operações de banco de dados** | Backend Architect | — | API Tester |
| **Mobile (iOS/Android)** | Mobile App Builder | — | Evidence Collector |
| **Modelo/pipeline de ML** | AI Engineer | — | Test Results Analyzer |
| **CI/CD/Infraestrutura** | DevOps Automator | Infrastructure Maintainer | Performance Benchmarker |
| **Feature premium/complexa** | Senior Developer | Backend Architect | Evidence Collector |
| **Protótipo rápido/POC** | Rapid Prototyper | Frontend Developer | Evidence Collector |
| **WebXR/imersivo** | XR Immersive Developer | — | Evidence Collector |
| **visionOS** | visionOS Spatial Engineer | macOS Spatial/Metal Engineer | Evidence Collector |
| **Controles de cockpit** | XR Cockpit Interaction Specialist | XR Interface Architect | Evidence Collector |
| **Tools CLI/terminal** | Terminal Integration Specialist | — | API Tester |
| **Inteligência de código** | LSP/Index Engineer | — | Test Results Analyzer |
| **Otimização de performance** | Performance Benchmarker | Infrastructure Maintainer | Performance Benchmarker |

### Suporte Especialista (ativado conforme necessário)

| Especialista | Quando Ativar | Trigger |
|-----------|-----------------|---------|
| UI Designer | Componente precisa de refinamento visual | Developer solicita orientação de design |
| Whimsy Injector | Feature precisa de delight/personalidade | UX review identifica oportunidade |
| Visual Storyteller | Conteúdo narrativo visual necessário | Conteúdo exige assets visuais |
| Brand Guardian | Preocupação com consistência de marca | QA encontra desvio de marca |
| XR Interface Architect | Design de interação espacial necessário | Feature XR exige orientação de UX |
| Analytics Reporter | Análise profunda de dados necessária | Feature exige integração de analytics |

## Tracks Paralelas de Build

Para deployments NEXUS-Full, quatro tracks rodam simultaneamente:

### Track A: Desenvolvimento Core do Produto
```
Gerenciado por: Agents Orchestrator (loop Dev↔QA)
Agentes: Frontend Developer, Backend Architect, AI Engineer,
        Mobile App Builder, Senior Developer
QA: Evidence Collector, API Tester, Test Results Analyzer

Cadência de sprint: sprints de 2 semanas
Diariamente: Implementação de tarefas + validação de QA
Fim do sprint: Sprint review + retrospectiva
```

### Track B: Preparação de Growth & Marketing
```
Gerenciado por: Project Shepherd
Agentes: Growth Hacker, Content Creator, Social Media Strategist,
        App Store Optimizer

Cadência de sprint: Alinhada aos milestones da Track A
Atividades:
- Growth Hacker → Desenhar viral loops e mecânicas de referral
- Content Creator → Construir pipeline de conteúdo de launch
- Social Media Strategist → Planejar campanha cross-platform
- App Store Optimizer → Preparar store listing (se mobile)
```

### Track C: Qualidade & Operações
```
Gerenciado por: Agents Orchestrator
Agentes: Evidence Collector, API Tester, Performance Benchmarker,
        Workflow Optimizer, Experiment Tracker

Atividades contínuas:
- Evidence Collector → QA com screenshots para toda tarefa
- API Tester → Validação de endpoint para toda tarefa de API
- Performance Benchmarker → Load testing periódico
- Workflow Optimizer → Identificação de melhoria de processo
- Experiment Tracker → Setup de teste A/B para features validadas
```

### Track D: Polish de Marca & Experiência
```
Gerenciado por: Brand Guardian
Agentes: UI Designer, Brand Guardian, Visual Storyteller,
        Whimsy Injector

Atividades disparadas:
- UI Designer → Refinamento de componentes quando QA identifica issues visuais
- Brand Guardian → Auditoria periódica de consistência de marca
- Visual Storyteller → Assets narrativos visuais conforme features são concluídas
- Whimsy Injector → Microinterações e momentos de delight
```

## Template de Execução de Sprint

### Sprint Planning (Dia 1)

```
Sprint Prioritizer ativa:
1. Revisar backlog com scores RICE atualizados
2. Selecionar tarefas para o sprint com base na velocity do time
3. Atribuir tarefas a developer agents
4. Identificar dependências e ordenação
5. Definir objetivo do sprint e critérios de sucesso

Output: Plano de Sprint com atribuições de tarefas
```

### Execução Diária (Dia 2 até Dia N-1)

```
Agents Orchestrator gerencia:
1. Checagem de status da tarefa atual
2. Execução do loop Dev↔QA
3. Identificação e resolução de blockers
4. Tracking e reporting de progresso

Formato do relatório de status:
- Tarefas concluídas hoje: [lista]
- Tarefas em QA: [lista]
- Tarefas em desenvolvimento: [lista]
- Tarefas bloqueadas: [lista com motivo]
- Taxa de aprovação de QA: [X/Y]
```

### Sprint Review (Dia N)

```
Project Shepherd facilita:
1. Demo das features concluídas
2. Review das evidências de QA para cada tarefa
3. Coletar feedback de stakeholders
4. Atualizar backlog com base nos aprendizados

Participantes: Todos os agentes ativos + stakeholders
Output: Sumário de Sprint Review
```

### Sprint Retrospective

```
Workflow Optimizer facilita:
1. O que foi bem?
2. O que pode melhorar?
3. O que vamos mudar no próximo sprint?
4. Métricas de eficiência do processo

Output: Itens de Ação da Retrospectiva
```

## Lógica de Decisão do Orchestrator

### Tratamento de Falhas de Tarefa

```
QUANDO a tarefa falha no QA:
  IF tentativa == 1:
    → Enviar feedback específico de QA ao developer
    → Developer corrige APENAS as issues identificadas
    → Reenviar para QA
    
  IF tentativa == 2:
    → Enviar feedback acumulado de QA
    → Considerar: o developer agent é o mais adequado?
    → Developer corrige com contexto adicional
    → Reenviar para QA
    
  IF tentativa == 3:
    → ESCALONAR
    → Opções:
      a) Reatribuir a outro developer agent
      b) Decompor tarefa em subtarefas menores
      c) Revisar abordagem/arquitetura
      d) Aceitar com limitações conhecidas (documentar)
      e) Adiar para sprint futuro
    → Documentar decisão e racional
```

### Gestão de Tarefas Paralelas

```
QUANDO múltiplas tarefas não têm dependências:
  → Atribuir simultaneamente a developer agents diferentes
  → Cada uma roda um loop Dev↔QA independente
  → Orchestrator acompanha todos os loops em paralelo
  → Fazer merge das tarefas concluídas na ordem de dependência

QUANDO a tarefa tem dependências:
  → Aguardar dependência passar no QA
  → Então atribuir tarefa dependente
  → Incluir contexto da dependência no handoff
```

## Checklist do Quality Gate

| # | Critério | Fonte de Evidência | Status |
|---|-----------|----------------|--------|
| 1 | Todas as tarefas do sprint passam no QA (100% concluídas) | Screenshots do Evidence Collector por tarefa | ☐ |
| 2 | Todos os endpoints de API validados | Relatório de regressão do API Tester | ☐ |
| 3 | Baselines de performance atingidos (P95 < 200ms) | Relatório do Performance Benchmarker | ☐ |
| 4 | Consistência de marca verificada (95%+ aderência) | Auditoria do Brand Guardian | ☐ |
| 5 | Nenhum bug crítico (zero P0/P1 aberto) | Sumário do Test Results Analyzer | ☐ |
| 6 | Todos os critérios de aceitação atendidos | Verificação tarefa por tarefa | ☐ |
| 7 | Code review concluído para todos os PRs | Evidência no histórico Git | ☐ |

## Decisão de Gate

**Gate Keeper**: Agents Orchestrator

- **PASS**: Aplicação feature-complete → ativação da Fase 4
- **CONTINUE**: Mais sprints necessários → continuar Fase 3
- **ESCALATE**: Issues sistêmicas → intervenção do Studio Producer

## Handoff para Fase 4

```markdown
## Pacote de Handoff Fase 3 → Fase 4

### Para Reality Checker:
- Aplicação completa (todas as features implementadas)
- Todas as evidências de QA dos loops Dev↔QA
- Resultados de regressão do API Tester
- Dados baseline do Performance Benchmarker
- Auditoria de consistência do Brand Guardian
- Lista de issues conhecidas (se houver limitações aceitas)

### Para Legal Compliance Checker:
- Detalhes de implementação de tratamento de dados
- Implementação de privacy policy
- Implementação de gestão de consentimento
- Medidas de segurança implementadas

### Para Performance Benchmarker:
- URLs da aplicação para load testing
- Padrões de tráfego esperados
- Performance budgets da arquitetura

### Para Infrastructure Maintainer:
- Requisitos de ambiente de produção
- Necessidades de configuração de escala
- Thresholds de alerta de monitoramento
```

---

*A Fase 3 está completa quando todas as tarefas do sprint passam no QA, todos os endpoints de API são validados, os baselines de performance são atingidos e nenhum bug crítico permanece aberto.*
