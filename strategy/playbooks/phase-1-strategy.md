# 🏗️ Playbook Fase 1 — Estratégia & Arquitetura

> **Duração**: 5-10 dias | **Agentes**: 8 | **Gate Keepers**: Studio Producer + Reality Checker

---

## Objetivo

Definir o que estamos construindo, como será estruturado e como o sucesso será medido — antes de escrever uma única linha de código. Toda decisão arquitetural é documentada. Toda feature é priorizada. Todo dólar é contabilizado.

## Pré-Condições

- [ ] Quality Gate da Fase 0 aprovado (decisão GO)
- [ ] Pacote de Handoff da Fase 0 recebido
- [ ] Alinhamento de stakeholders sobre o escopo do projeto

## Sequência de Ativação dos Agentes

### Passo 1: Enquadramento Estratégico (Dia 1-3, Paralelo)

#### 🎬 Studio Producer — Alinhamento Estratégico de Portfólio
```
Ative Studio Producer para alinhamento estratégico de portfólio em [PROJETO].

Input: Executive Summary da Fase 0 + Market Analysis Report
Entregáveis obrigatórios:
1. Strategic Portfolio Plan com posicionamento do projeto
2. Visão, objetivos e metas de ROI
3. Estratégia de alocação de recursos
4. Avaliação de risco/recompensa
5. Critérios de sucesso e definições de milestones

Alinhar com: objetivos estratégicos organizacionais
Formato: Template de Strategic Portfolio Plan
Timeline: 3 dias
```

#### 🎭 Brand Guardian — Sistema de Identidade de Marca
```
Ative Brand Guardian para desenvolvimento de identidade de marca em [PROJETO].

Input: UX Research da Fase 0 (personas, journey maps)
Entregáveis obrigatórios:
1. Fundação de Marca (propósito, visão, missão, valores, personalidade)
2. Sistema de Identidade Visual (cores, tipografia, spacing como variáveis CSS)
3. Voz de Marca e Arquitetura de Messaging
4. Especificações do sistema de logo (se for uma marca nova)
5. Guidelines de uso de marca

Formato: Documento de Sistema de Identidade de Marca
Timeline: 3 dias
```

#### 💰 Finance Tracker — Planejamento de Orçamento e Recursos
```
Ative Finance Tracker para planejamento financeiro em [PROJETO].

Input: plano estratégico do Studio Producer + Tech Stack Assessment da Fase 0
Entregáveis obrigatórios:
1. Orçamento abrangente do projeto com breakdown por categoria
2. Projeções de custo de recursos (agentes, infraestrutura, tools)
3. Modelo de ROI com análise de break-even
4. Timeline de cash flow
5. Avaliação de risco financeiro com reservas de contingência

Formato: Plano Financeiro com Projeções de ROI
Timeline: 2 dias
```

### Passo 2: Arquitetura Técnica (Dia 3-7, Paralelo, depois dos outputs do Passo 1 disponíveis)

#### 🏛️ UX Architect — Arquitetura Técnica + Fundação de UX
```
Ative UX Architect para arquitetura técnica em [PROJETO].

Input: identidade visual do Brand Guardian + UX Research da Fase 0
Entregáveis obrigatórios:
1. CSS Design System (variáveis, tokens, escalas)
2. Layout Framework (padrões Grid/Flexbox, breakpoints responsivos)
3. Component Architecture (convenções de nomenclatura, hierarquia)
4. Information Architecture (fluxo de páginas, hierarquia de conteúdo)
5. Theme System (toggle light/dark/system)
6. Accessibility Foundation (baseline WCAG 2.1 AA)

Arquivos a criar:
- css/design-system.css
- css/layout.css
- css/components.css
- docs/ux-architecture.md

Formato: Pacote de Fundação Developer-Ready
Timeline: 4 dias
```

#### 🏗️ Backend Architect — Arquitetura de Sistema
```
Ative Backend Architect para arquitetura de sistema em [PROJETO].

Input: Tech Stack Assessment da Fase 0 + Compliance Requirements
Entregáveis obrigatórios:
1. System Architecture Specification
   - Padrão de arquitetura (microservices/monolith/serverless/hybrid)
   - Padrão de comunicação (REST/GraphQL/gRPC/event-driven)
   - Padrão de dados (CQRS/Event Sourcing/CRUD)
2. Design de Schema de Banco com estratégia de indexação
3. Especificação de Design de API com versionamento
4. Arquitetura de Autenticação e Autorização
5. Arquitetura de Segurança (defense in depth)
6. Plano de Escalabilidade (estratégia de escala horizontal)

Formato: System Architecture Specification
Timeline: 4 dias
```

#### 🤖 AI Engineer — Arquitetura de ML (se aplicável)
```
Ative AI Engineer para arquitetura de sistema de ML em [PROJETO].

Input: arquitetura de sistema do Backend Architect + Data Audit da Fase 0
Entregáveis obrigatórios:
1. ML System Design
   - Seleção de modelo e estratégia de treinamento
   - Arquitetura de data pipeline
   - Estratégia de inferência (real-time/batch/edge)
2. Framework de Ética e Segurança de IA
3. Plano de monitoramento e retreinamento de modelo
4. Pontos de integração com a aplicação principal
5. Projeções de custo para infraestrutura de ML

Condição: ativar apenas se o projeto incluir features de IA/ML
Formato: Documento de ML System Design
Timeline: 3 dias
```

#### 👔 Senior Project Manager — Conversão de Spec em Tarefas
```
Ative Senior Project Manager para criação de lista de tarefas em [PROJETO].

Input: TODOS os documentos da Fase 0 + specs de arquitetura (conforme disponíveis)
Entregáveis obrigatórios:
1. Lista de Tarefas Abrangente
   - Citar requisitos EXATOS da spec (sem features de luxo)
   - Cada tarefa tem critérios de aceitação claros
   - Dependências mapeadas entre tarefas
   - Estimativas de esforço (story points ou horas)
2. Work Breakdown Structure
3. Identificação do caminho crítico
4. Registro de riscos para implementação

Regras:
- NÃO adicione features que não estejam na especificação
- Cite o texto exato dos requisitos
- Seja realista nas estimativas de esforço

Formato: Lista de Tarefas com critérios de aceitação
Timeline: 3 dias
```

### Passo 3: Priorização (Dia 7-10, Sequencial, depois do Passo 2)

#### 🎯 Sprint Prioritizer — Priorização de Features
```
Ative Sprint Prioritizer para priorização de backlog em [PROJETO].

Input:
- Senior Project Manager → Task List
- Backend Architect → System Architecture
- UX Architect → UX Architecture
- Finance Tracker → Budget Framework
- Studio Producer → Strategic Plan

Entregáveis obrigatórios:
1. Backlog pontuado por RICE (Reach, Impact, Confidence, Effort)
2. Atribuições de sprint com estimativa baseada em velocity
3. Mapa de dependências com caminho crítico
4. Classificação MoSCoW (Must/Should/Could/Won't)
5. Plano de release com mapeamento de milestones

Validação: Studio Producer confirma alinhamento estratégico
Formato: Plano de Sprint Priorizado
Timeline: 2 dias
```

## Checklist do Quality Gate

| # | Critério | Fonte de Evidência | Status |
|---|-----------|----------------|--------|
| 1 | Arquitetura cobre 100% dos requisitos da spec | Lista de tarefas do Senior PM cruzada com arquitetura | ☐ |
| 2 | Sistema de marca completo (logo, cores, tipografia, voz) | Entregável do Brand Guardian | ☐ |
| 3 | Todos os componentes técnicos têm caminho de implementação | Specs do Backend Architect + UX Architect | ☐ |
| 4 | Orçamento aprovado e dentro das restrições | Plano do Finance Tracker | ☐ |
| 5 | Plano de sprint é baseado em velocidade e realista | Backlog do Sprint Prioritizer | ☐ |
| 6 | Arquitetura de segurança definida | Spec de segurança do Backend Architect | ☐ |
| 7 | Requisitos de compliance integrados à arquitetura | Requisitos legais mapeados para decisões técnicas | ☐ |

## Decisão de Gate

**Assinatura dupla obrigatória**: Studio Producer (estratégica) + Reality Checker (técnica)

- **APPROVED**: Prosseguir para Fase 2 com o Pacote de Arquitetura completo
- **REVISE**: Itens específicos precisam de retrabalho (retornar ao Passo relevante)
- **RESTRUCTURE**: Issues fundamentais de arquitetura (reiniciar Fase 1)

## Handoff para Fase 2

```markdown
## Pacote de Handoff Fase 1 → Fase 2

### Pacote de Arquitetura:
1. Strategic Portfolio Plan (Studio Producer)
2. Brand Identity System (Brand Guardian)
3. Financial Plan (Finance Tracker)
4. CSS Design System + UX Architecture (UX Architect)
5. System Architecture Specification (Backend Architect)
6. ML System Design (AI Engineer — if applicable)
7. Comprehensive Task List (Senior Project Manager)
8. Prioritized Sprint Plan (Sprint Prioritizer)

### Para DevOps Automator:
- Arquitetura de deployment do Backend Architect
- Requisitos de ambiente da System Architecture
- Requisitos de monitoramento das necessidades de infraestrutura

### Para Frontend Developer:
- CSS Design System do UX Architect
- Brand Identity do Brand Guardian
- Arquitetura de componentes do UX Architect
- Especificação de API do Backend Architect

### Para Backend Architect (continuação):
- Schema de banco pronto para deployment
- Scaffold de API pronto para implementação
- Arquitetura do sistema de auth definida
```

---

*A Fase 1 está completa quando Studio Producer e Reality Checker assinam o Pacote de Arquitetura.*
