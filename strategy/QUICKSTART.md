# ⚡ Guia Quick-Start NEXUS

> **Saia do zero para um pipeline multiagente orquestrado em 5 minutos.**

---

## O que é NEXUS?

**NEXUS** (Network of EXperts, Unified in Strategy) transforma os especialistas de IA da The Agency em um pipeline coordenado. Em vez de ativar agentes um por vez e esperar que trabalhem juntos, NEXUS define exatamente quem faz o quê, quando e como a qualidade é verificada em cada etapa.

## Escolha Seu Modo

| Eu quero... | Use | Agentes | Tempo |
|-------------|-----|--------|------|
| Construir um produto completo do zero | **NEXUS-Full** | Todos | 12-24 semanas |
| Construir uma feature ou MVP | **NEXUS-Sprint** | 15-25 | 2-6 semanas |
| Fazer uma tarefa específica (bug fix, campanha, auditoria) | **NEXUS-Micro** | 5-10 | 1-5 dias |

---

## 🚀 NEXUS-Full: Começar um Projeto Completo

**Copie este prompt para ativar o pipeline completo:**

```
Activate Agents Orchestrator in NEXUS-Full mode.

Project: [YOUR PROJECT NAME]
Specification: [DESCRIBE YOUR PROJECT OR LINK TO SPEC]

Execute the complete NEXUS pipeline:
- Phase 0: Discovery (Trend Researcher, Feedback Synthesizer, UX Researcher, Analytics Reporter, Legal Compliance Checker, Tool Evaluator)
- Phase 1: Strategy (Studio Producer, Senior Project Manager, Sprint Prioritizer, UX Architect, Brand Guardian, Backend Architect, Finance Tracker)
- Phase 2: Foundation (DevOps Automator, Frontend Developer, Backend Architect, UX Architect, Infrastructure Maintainer)
- Phase 3: Build (Dev↔QA loops — all engineering + Evidence Collector)
- Phase 4: Harden (Reality Checker, Performance Benchmarker, API Tester, Legal Compliance Checker)
- Phase 5: Launch (Growth Hacker, Content Creator, all marketing agents, DevOps Automator)
- Phase 6: Operate (Analytics Reporter, Infrastructure Maintainer, Support Responder, ongoing)

Quality gates between every phase. Evidence required for all assessments.
Maximum 3 retries per task before escalation.
```

---

## 🏃 NEXUS-Sprint: Construir uma Feature ou MVP

**Copie este prompt:**

```
Activate Agents Orchestrator in NEXUS-Sprint mode.

Feature/MVP: [DESCRIBE WHAT YOU'RE BUILDING]
Timeline: [TARGET WEEKS]
Skip Phase 0 (market already validated).

Sprint team:
- PM: Senior Project Manager, Sprint Prioritizer
- Design: UX Architect, Brand Guardian
- Engineering: Frontend Developer, Backend Architect, DevOps Automator
- QA: Evidence Collector, Reality Checker, API Tester
- Support: Analytics Reporter

Begin at Phase 1 with architecture and sprint planning.
Run Dev↔QA loops for all implementation tasks.
Reality Checker approval required before launch.
```

---

## 🎯 NEXUS-Micro: Fazer uma Tarefa Específica

**Escolha seu cenário e copie o prompt:**

### Corrigir um Bug
```
Activate Backend Architect to investigate and fix [BUG DESCRIPTION].
After fix, activate API Tester to verify the fix.
Then activate Evidence Collector to confirm no visual regressions.
```

### Rodar uma Campanha de Marketing
```
Activate Social Media Strategist as campaign lead for [CAMPAIGN DESCRIPTION].
Team: Content Creator, Twitter Engager, Instagram Curator, Reddit Community Builder.
Brand Guardian reviews all content before publishing.
Analytics Reporter tracks performance daily.
Growth Hacker optimizes channels weekly.
```

### Conduzir uma Auditoria de Compliance
```
Activate Legal Compliance Checker for comprehensive compliance audit.
Scope: [GDPR / CCPA / HIPAA / ALL]
After audit, activate Executive Summary Generator to create stakeholder report.
```

### Investigar Problemas de Performance
```
Activate Performance Benchmarker to diagnose performance issues.
Scope: [API response times / Page load / Database queries / All]
After diagnosis, activate Infrastructure Maintainer for optimization.
DevOps Automator deploys any infrastructure changes.
```

### Pesquisa de Mercado
```
Activate Trend Researcher for market intelligence on [DOMAIN].
Deliverables: Competitive landscape, market sizing, trend forecast.
After research, activate Executive Summary Generator for executive brief.
```

### Melhoria de UX
```
Activate UX Researcher to identify usability issues in [FEATURE/PRODUCT].
After research, activate UX Architect to design improvements.
Frontend Developer implements changes.
Evidence Collector verifies improvements.
```

---

## 📁 Documentos de Estratégia

| Documento | Finalidade | Localização |
|----------|---------|----------|
| **Estratégia Mestre** | Doutrina NEXUS completa | `strategy/nexus-strategy.md` |
| **Playbook Fase 0** | Discovery & inteligência | `strategy/playbooks/phase-0-discovery.md` |
| **Playbook Fase 1** | Estratégia & arquitetura | `strategy/playbooks/phase-1-strategy.md` |
| **Playbook Fase 2** | Fundação & scaffolding | `strategy/playbooks/phase-2-foundation.md` |
| **Playbook Fase 3** | Build & iterar | `strategy/playbooks/phase-3-build.md` |
| **Playbook Fase 4** | Qualidade & hardening | `strategy/playbooks/phase-4-hardening.md` |
| **Playbook Fase 5** | Launch & growth | `strategy/playbooks/phase-5-launch.md` |
| **Playbook Fase 6** | Operar & evoluir | `strategy/playbooks/phase-6-operate.md` |
| **Prompts de Ativação** | Prompts de agentes prontos para uso | `strategy/coordination/agent-activation-prompts.md` |
| **Templates de Handoff** | Formatos de handoff padronizados | `strategy/coordination/handoff-templates.md` |
| **Runbook Startup MVP** | Build de MVP em 4-6 semanas | `strategy/runbooks/scenario-startup-mvp.md` |
| **Runbook Enterprise Feature** | Desenvolvimento de feature enterprise | `strategy/runbooks/scenario-enterprise-feature.md` |
| **Runbook Marketing Campaign** | Campanha multicanal | `strategy/runbooks/scenario-marketing-campaign.md` |
| **Runbook Incident Response** | Tratamento de incidente em produção | `strategy/runbooks/scenario-incident-response.md` |

---

## 🔑 Conceitos-Chave em 30 Segundos

1. **Quality Gates** — Nenhuma fase avança sem aprovação baseada em evidências
2. **Loop Dev↔QA** — Toda tarefa é construída e depois testada; PASS para prosseguir, FAIL para tentar de novo (máx. 3)
3. **Handoffs** — Transferência estruturada de contexto entre agentes (nunca começar frio)
4. **Reality Checker** — Autoridade final de qualidade; default para "NEEDS WORK"
5. **Agents Orchestrator** — Controlador de pipeline que gerencia o fluxo inteiro
6. **Evidence Over Claims** — Screenshots, resultados de testes e dados — não afirmações

---

## 🎭 Os Agentes em uma Visão Rápida

```
ENGINEERING         │ DESIGN              │ MARKETING
Frontend Developer  │ UI Designer         │ Growth Hacker
Backend Architect   │ UX Researcher       │ Content Creator
Mobile App Builder  │ UX Architect        │ Twitter Engager
AI Engineer         │ Brand Guardian      │ TikTok Strategist
DevOps Automator    │ Visual Storyteller  │ Instagram Curator
Rapid Prototyper    │ Whimsy Injector     │ Reddit Community Builder
Senior Developer    │ Image Prompt Eng.   │ App Store Optimizer
                    │                     │ Social Media Strategist
────────────────────┼─────────────────────┼──────────────────────
PRODUCT             │ PROJECT MGMT        │ TESTING
Sprint Prioritizer  │ Studio Producer     │ Evidence Collector
Trend Researcher    │ Project Shepherd    │ Reality Checker
Feedback Synthesizer│ Studio Operations   │ Test Results Analyzer
                    │ Experiment Tracker  │ Performance Benchmarker
                    │ Senior Project Mgr  │ API Tester
                    │                     │ Tool Evaluator
                    │                     │ Workflow Optimizer
────────────────────┼─────────────────────┼──────────────────────
SUPPORT             │ SPATIAL             │ SPECIALIZED
Support Responder   │ XR Interface Arch.  │ Agents Orchestrator
Analytics Reporter  │ macOS Spatial/Metal │ Analytics Reporter
Finance Tracker     │ XR Immersive Dev    │ LSP/Index Engineer
Infra Maintainer    │ XR Cockpit Spec.    │ Sales Data Extraction
Legal Compliance    │ visionOS Spatial    │ Data Consolidation
Exec Summary Gen.   │ Terminal Integration│ Report Distribution
```

---

<div align="center">

**Comece com um modo. Siga o playbook. Confie no pipeline.**

`strategy/nexus-strategy.md` — A doutrina completa

</div>
