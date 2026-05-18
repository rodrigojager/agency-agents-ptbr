# 🚀 Runbook: Build de Startup MVP

> **Modo**: NEXUS-Sprint | **Duração**: 4-6 semanas | **Agentes**: 18-22

---

## Cenário

Você está construindo um MVP de startup — um novo produto que precisa validar product-market fit rapidamente. Velocidade importa, mas qualidade também. Você precisa sair da ideia para um produto live com usuários reais em 4-6 semanas.

## Roster de Agentes

### Time Core (Sempre Ativo)
| Agente | Papel |
|-------|------|
| Agents Orchestrator | Controlador de pipeline |
| Senior Project Manager | Conversão de spec em tarefas |
| Sprint Prioritizer | Gestão de backlog |
| UX Architect | Fundação técnica |
| Frontend Developer | Implementação de UI |
| Backend Architect | API e banco de dados |
| DevOps Automator | CI/CD e deployment |
| Evidence Collector | QA para cada tarefa |
| Reality Checker | Quality gate final |

### Time de Growth (Ativado na Semana 3+)
| Agente | Papel |
|-------|------|
| Growth Hacker | Estratégia de aquisição |
| Content Creator | Conteúdo de launch |
| Social Media Strategist | Campanha social |

### Time de Support (Conforme Necessário)
| Agente | Papel |
|-------|------|
| Brand Guardian | Identidade de marca |
| Analytics Reporter | Métricas e dashboards |
| Rapid Prototyper | Experimentos rápidos de validação |
| AI Engineer | Se o produto incluir features de IA |
| Performance Benchmarker | Load testing antes do launch |
| Infrastructure Maintainer | Setup de produção |

## Execução Semana a Semana

### Semana 1: Discovery + Arquitetura (Fase 0 + Fase 1 comprimidas)

```
Dia 1-2: Discovery Comprimido
├── Trend Researcher → Scan competitivo rápido (1 dia, não relatório completo)
├── UX Architect → Wireframe dos principais fluxos de usuário
└── Senior Project Manager → Converter spec em lista de tarefas

Dia 3-4: Arquitetura
├── UX Architect → Design system CSS + arquitetura de componentes
├── Backend Architect → Arquitetura de sistema + schema de banco
├── Brand Guardian → Fundação rápida de marca (cores, tipografia, voz)
└── Sprint Prioritizer → Backlog pontuado por RICE + plano de sprint

Dia 5: Setup de Fundação
├── DevOps Automator → Pipeline CI/CD + ambientes
├── Frontend Developer → Scaffolding do projeto
├── Backend Architect → Banco de dados + scaffold de API
└── Quality Gate: Pacote de Arquitetura aprovado
```

### Semana 2-3: Core Build (Fase 2 + Fase 3)

```
Sprint 1 (Semana 2):
├── Agents Orchestrator gerencia o loop Dev↔QA
├── Frontend Developer → UI core (auth, views principais, navegação)
├── Backend Architect → API core (auth, CRUD, business logic)
├── Evidence Collector → QA em toda tarefa concluída
├── AI Engineer → Features de ML se aplicável
└── Sprint Review no fim da semana

Sprint 2 (Semana 3):
├── Continuar loop Dev↔QA para features restantes
├── Growth Hacker → Desenhar mecânicas virais + sistema de referral
├── Content Creator → Começar criação de conteúdo de launch
├── Analytics Reporter → Configurar tracking e dashboards
└── Sprint Review no fim da semana
```

### Semana 4: Polish + Hardening (Fase 4)

```
Dia 1-2: Sprint de Qualidade
├── Evidence Collector → Suite completa de screenshots
├── Performance Benchmarker → Load testing
├── Frontend Developer → Corrigir issues de QA
├── Backend Architect → Corrigir issues de API
└── Brand Guardian → Auditoria de consistência de marca

Dia 3-4: Reality Check
├── Reality Checker → Testes finais de integração
├── Infrastructure Maintainer → Prontidão de produção
└── DevOps Automator → Preparação de deployment em produção

Dia 5: Decisão de Gate
├── Veredito do Reality Checker
├── IF NEEDS WORK: Ciclo rápido de correção (2-3 dias)
├── IF READY: Prosseguir para launch
└── Executive Summary Generator → Briefing para stakeholders
```

### Semana 5-6: Launch + Growth (Fase 5)

```
Semana 5: Launch
├── DevOps Automator → Deployment em produção
├── Growth Hacker → Ativar canais de aquisição
├── Content Creator → Publicar conteúdo de launch
├── Social Media Strategist → Campanha cross-platform
├── Analytics Reporter → Monitoramento em tempo real
└── Support Responder → Suporte ao usuário ativo

Semana 6: Otimizar
├── Growth Hacker → Analisar e otimizar canais
├── Feedback Synthesizer → Coletar feedback inicial de usuários
├── Experiment Tracker → Lançar testes A/B
├── Analytics Reporter → Análise da semana 1
└── Sprint Prioritizer → Planejar sprint de iteração
```

## Decisões-Chave

| Ponto de Decisão | Quando | Quem Decide |
|---------------|------|-------------|
| Go/No-Go no conceito | Fim do Dia 2 | Studio Producer |
| Aprovação de arquitetura | Fim do Dia 4 | Senior Project Manager |
| Escopo de features para MVP | Sprint planning | Sprint Prioritizer |
| Prontidão de produção | Semana 4 Dia 5 | Reality Checker |
| Timing de launch | Após Reality Checker READY | Studio Producer |

## Critérios de Sucesso

| Métrica | Meta |
|--------|--------|
| Tempo até produto live | ≤ 6 semanas |
| Features core completas | 100% do escopo do MVP |
| Primeiros usuários onboarded | Em até 48 horas após launch |
| Uptime do sistema | > 99% na primeira semana |
| Feedback de usuário coletado | ≥ 50 respostas nas primeiras 2 semanas |

## Armadilhas Comuns & Mitigações

| Armadilha | Mitigação |
|---------|-----------|
| Scope creep durante o build | Sprint Prioritizer reforça MoSCoW — "Won't" significa won't |
| Over-engineering para escala | Mentalidade Rapid Prototyper — valide primeiro, escale depois |
| Pular QA por velocidade | Evidence Collector roda em TODA tarefa — sem exceções |
| Launch sem monitoramento | Infrastructure Maintainer configura monitoramento na Semana 1 |
| Sem mecanismo de feedback | Analytics + coleta de feedback embutidos no Sprint 1 |
