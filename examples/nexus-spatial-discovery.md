# Nexus Spatial: Exercício de Discovery com a Agência Completa

> **Tipo de exercício:** Product discovery multi-agent
> **Data:** 5 de março de 2026
> **Agentes acionados:** 8 (em paralelo)
> **Duração:** ~10 minutos de tempo real
> **Objetivo:** Demonstrar orquestração full-agency desde identificação de oportunidade até planejamento abrangente

---

## Sumário

1. [A Oportunidade](#1-a-oportunidade)
2. [Validação de Mercado](#2-validação-de-mercado)
3. [Arquitetura Técnica](#3-arquitetura-técnica)
4. [Estratégia de Marca](#4-estratégia-de-marca)
5. [Go-to-Market e Growth](#5-go-to-market-e-growth)
6. [Blueprint de Customer Support](#6-blueprint-de-customer-support)
7. [Pesquisa UX e Direção de Design](#7-pesquisa-ux-e-direção-de-design)
8. [Plano de Execução do Projeto](#8-plano-de-execução-do-projeto)
9. [Arquitetura de Interface Espacial](#9-arquitetura-de-interface-espacial)
10. [Síntese Cross-Agent](#10-síntese-cross-agent)

---

## 1. A Oportunidade

### Como Foi Encontrada

Pesquisa web em múltiplas fontes identificou três tendências convergentes:

- **Infraestrutura/orquestração de IA** é a categoria de software de crescimento mais rápido (mercado de orquestração de IA avaliado em ~$13,5B em 2026, CAGR de 22%+)
- **Spatial computing** (Vision Pro, WebXR) está amadurecendo, mas ainda carece de killer apps enterprise
- Toda ferramenta existente de workflow de IA (LangSmith, n8n, Flowise, CrewAI) é um **dashboard 2D plano**

### O Conceito: Nexus Spatial

Um AI Agent Command Center em spatial computing -- uma aplicação VisionOS + WebXR que fornece um command center 3D imersivo para orquestrar, monitorar e interagir com agentes de IA. Usuários visualizam pipelines de agentes como grafos de nós 3D, monitoram saídas em tempo real em painéis espaciais, constroem workflows com drag-and-drop em espaço 3D e colaboram em ambientes espaciais compartilhados.

### Por Que Esta Agência Está Unicamente Bem Posicionada

A agência tem expertise profunda em spatial computing (desenvolvedores XR, engenheiros VisionOS, especialistas Metal, arquitetos de interface) junto com uma stack completa de engenharia, design, marketing e operações -- uma combinação rara para um produto que exige tanto domínio de spatial computing quanto rigor de software enterprise.

### Fontes

- [Profitable SaaS Ideas 2026 (273K+ Reviews)](https://bigideasdb.com/profitable-saas-micro-saas-ideas-2026)
- [2026 SaaS and AI Revolution: 20 Top Trends](https://fungies.io/the-2026-saas-and-ai-revolution-20-top-trends/)
- [Top 21 Underserved Markets 2026](https://mktclarity.com/blogs/news/list-underserved-niches)
- [Fastest Growing Products 2026 - G2](https://www.g2.com/best-software-companies/fastest-growing)
- [PwC 2026 AI Business Predictions](https://www.pwc.com/us/en/tech-effect/ai-analytics/ai-predictions.html)

---

## 2. Validação de Mercado

**Agente:** Product Trend Researcher

### Veredito: CONDITIONAL GO -- 2D-First, Spatial-Second

### Tamanho de Mercado

| Segmento | Valor em 2026 | Crescimento |
|---------|-----------|--------|
| Ferramentas de Orquestração de IA | $13,5B | CAGR de 22,3% |
| Agentes de IA Autônomos | $8,5B | CAGR de 45,8% até $50,3B em 2030 |
| Extended Reality | $10,64B | CAGR de 40,95% |
| Spatial Computing (amplo) | $170-220B | Varia conforme definição |

### Cenário Competitivo

**Orquestração de Agentes de IA (todos 2D):**

| Ferramenta | Força | Gap de UX |
|------|----------|--------|
| LangChain/LangSmith | Orquestração baseada em grafos, $39/usuário/mês | Dashboard plano; grafos complexos ilegíveis em escala |
| CrewAI | 100K+ desenvolvedores, execução rápida | CLI-first, ferramental visual mínimo |
| Microsoft Agent Framework | Integração enterprise | Embutido no portal Azure, sem UI standalone |
| n8n | Visual workflow builder, $20-50/mês | Canvas 2D sofre com relações entre agentes |
| Flowise | Fluxos de IA drag-and-drop | Limitado a fluxos lineares, sem monitoramento multi-agent |

**Produtos de "Mission Control" (emergentes, todos 2D):**
- cmd-deck: Kanban board para agentes de codificação de IA
- Supervity Agent Command Center: Observabilidade enterprise
- OpenClaw Command Center: Gestão de frotas de agentes
- Mission Control AI: Gestão de synthetic workers
- Mission Control HQ: Coordenação baseada em squads

**O gap:** Produtos são ou espaciais mas não focados em IA, ou focados em IA mas 2D planos. Nenhum produto está na interseção.

### Reality Check do Vision Pro

- Base instalada: ~1M de unidades globalmente (vendas caíram 95% desde o lançamento)
- Apple mudou foco para óculos AR leves
- Existem apenas ~3.000 apps específicos para VisionOS
- **Implicação:** NÃO liderar com VisionOS. Liderar com web, adicionar WebXR, deixar VisionOS nativo por último.

### WebXR como Desbloqueio de Distribuição

- Safari adotou WebXR Device API no fim de 2025
- Adoção de WebXR cresceu 40% em 2026
- WebGPU entrega renderização quase nativa em browsers
- Android XR dá suporte aos padrões WebXR e OpenXR

### Personas-Alvo e Pricing

| Tier | Preço | Alvo |
|------|-------|--------|
| Explorer | Free | Desenvolvedores, solo builders (3 agentes, viewer WebXR) |
| Pro | $99/usuário/mês | Times pequenos (25 agentes, colaboração) |
| Team | $249/usuário/mês | Times de IA mid-market (agentes ilimitados, analytics) |
| Enterprise | Custom ($2K-10K/mês) | Grandes empresas (SSO, RBAC, on-prem, SLA) |

### Estratégia Faseada Recomendada

1. **Meses 1-6:** Construir um dashboard web 2D premium com capacidades Three.js 2.5D. Meta: 50 times pagantes, $60K MRR.
2. **Meses 6-12:** Adicionar modo espacial WebXR opcional (baseado em browser). Meta: 200 times, $300K MRR.
3. **Meses 12-18:** App VisionOS nativo somente se demanda espacial for validada. Meta: 500 times, $1M+ MRR.

### Principais Riscos

| Risco | Severidade |
|------|----------|
| Base instalada do Vision Pro é criticamente pequena | ALTA |
| "Solução espacial em busca de problema" -- 3D é realmente 10x melhor que 2D? | ALTA |
| Posicionamento "mission control" já concorrido (5+ produtos existentes) | MODERADA |
| Adoção enterprise de spatial computing ainda inicial | MODERADA |
| Complexidade de integração entre frameworks de IA | MODERADA |

### Fontes

- [MarketsandMarkets - AI Orchestration Market](https://www.marketsandmarkets.com/Market-Reports/ai-orchestration-market-148121911.html)
- [Deloitte - AI Agent Orchestration Predictions 2026](https://www.deloitte.com/us/en/insights/industry/technology/technology-media-and-telecom-predictions/2026/ai-agent-orchestration.html)
- [Mordor Intelligence - Extended Reality Market](https://www.mordorintelligence.com/industry-reports/extended-reality-xr-market)
- [Fintool - Vision Pro Production Halted](https://fintool.com/news/apple-vision-pro-production-halt)
- [MadXR - WebXR Browser-Based Experiences 2026](https://www.madxr.io/webxr-browser-immersive-experiences-2026.html)

---

## 3. Arquitetura Técnica

**Agente:** Backend Architect

### Visão Geral do Sistema

Uma arquitetura de 8 serviços com fronteiras claras de ownership, desenhada para scaling horizontal e integração de IA agnóstica a providers.

```
+------------------------------------------------------------------+
|                     CLIENT TIER                                   |
|  VisionOS Native (Swift/RealityKit)  |  WebXR (React Three Fiber) |
+------------------------------------------------------------------+
                              |
+-----------------------------v------------------------------------+
|                      API GATEWAY (Kong / AWS API GW)              |
|  Rate limiting | JWT validation | WebSocket upgrade | TLS        |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                      SERVICE TIER                                 |
|  Auth | Workspace | Workflow | Orchestration (Rust) |             |
|  Collaboration (Yjs CRDT) | Streaming (WS) | Plugin | Billing    |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                      DATA TIER                                    |
|  PostgreSQL 16 | Redis 7 Cluster | S3 | ClickHouse | NATS        |
+------------------------------------------------------------------+
                              |
+------------------------------------------------------------------+
|                    AI PROVIDER TIER                                |
|  OpenAI | Anthropic | Google | Local Models | Custom Plugins      |
+------------------------------------------------------------------+
```

### Tech Stack

| Componente | Tecnologia | Racional |
|-----------|------------|-----------|
| Orchestration Engine | **Rust** | Scheduling sub-ms, zero pausas de GC, memory safety para sandboxing de agentes |
| API Services | TypeScript / NestJS | Velocidade de desenvolvimento para serviços CRUD-heavy |
| Cliente VisionOS | Swift 6, SwiftUI, RealityKit | Spatial computing first-class com Liquid Glass |
| Cliente WebXR | TypeScript, React Three Fiber | WebXR production-grade com modelo de componentes React |
| Message Broker | NATS JetStream | Leve, entrega exactly-once, mais simples que Kafka |
| Colaboração | Yjs (CRDT) + WebRTC | Edição concorrente de grafo 3D sem conflitos |
| Banco Primário | PostgreSQL 16 | JSONB para configs flexíveis, Row-Level Security para isolamento de tenants |

### Modelo de Dados Central

14 tabelas cobrindo:
- **Identidade e Acesso:** users, workspaces, team_memberships, api_keys
- **Workflows:** workflows, workflow_versions, nodes, edges
- **Execuções:** executions, execution_steps, step_output_chunks
- **Colaboração:** collaboration_sessions, session_participants
- **Credenciais:** provider_credentials (criptografadas com AES-256-GCM)
- **Billing:** subscriptions, usage_records
- **Audit:** audit_log (append-only)

### Registro de Tipos de Nó

```
Built-in Node Types:
  ai_agent          -- Calls an AI provider with a prompt
  prompt_template   -- Renders a template with variables
  conditional       -- Routes based on expression
  transform         -- Sandboxed code snippet (JS/Python)
  input / output    -- Workflow entry/exit points
  human_review      -- Pauses for human approval
  loop              -- Repeats subgraph
  parallel_split    -- Fans out to branches
  parallel_join     -- Waits for branches
  webhook_trigger   -- External HTTP trigger
  delay             -- Timed pause
```

### Canais WebSocket

Streaming em tempo real via WSS com:
- Números de sequência por canal para ordenação
- Detecção de gaps com solicitações de replay
- Recuperação por snapshot quando >1000 eventos atrasado
- Throttling client-side para dispositivos de menor potência

### Arquitetura de Segurança

| Camada | Mecanismo |
|-------|-----------|
| Auth de Usuário | OAuth 2.0 (GitHub, Google, Apple) + email/senha + TOTP MFA opcional |
| API Keys | Hash SHA-256, escopo definido, expiração opcional |
| Service-to-Service | mTLS via service mesh |
| Auth WebSocket | Tickets de uso único com expiração de 30 segundos |
| Armazenamento de Credenciais | Envelope encryption (AES-256-GCM + AWS KMS) |
| Code Sandboxing | microVMs gVisor/Firecracker (sem rede, 256MB RAM, 30s CPU) |
| Isolamento de Tenant | PostgreSQL Row-Level Security + policies IAM S3 + scoping de subjects NATS |

### Metas de Scaling

| Métrica | Ano 1 | Ano 2 |
|--------|--------|--------|
| Execuções concorrentes de agentes | 5.000 | 50.000 |
| Conexões WebSocket | 10.000 | 100.000 |
| Latência P95 de API | < 150ms | < 100ms |
| Latência P95 de evento WS | < 80ms | < 50ms |

### Fases do MVP

1. **Semanas 1-6:** Editor web 2D, execução sequencial, adapters OpenAI + Anthropic
2. **Semanas 7-12:** Modo WebXR 3D, execução paralela, hand tracking, RBAC
3. **Semanas 13-20:** Colaboração multi-user, VisionOS nativo, billing
4. **Semanas 21-30:** SSO enterprise, plugin SDK, SOC 2, hardening de escala

---

## 4. Estratégia de Marca

**Agente:** Brand Guardian

### Posicionamento

**Criação de categoria acima de competição em categoria.** Nexus Spatial define uma nova categoria -- **Spatial AI Operations (SpatialAIOps)** -- em vez de disputar posição no espaço concorrido de dashboards de observabilidade de IA.

**Declaração de posicionamento:** Para times técnicos que gerenciam workflows complexos de agentes de IA, Nexus Spatial é o command center 3D imersivo que fornece consciência espacial da orquestração de agentes, diferente de dashboards 2D planos, porque spatial computing transforma monitoramento de leitura de dashboards em habitar sua infraestrutura.

### Validação do Nome

"Nexus Spatial" é **validado como forte:**
- "Nexus" conecta ao framework de orquestração NEXUS (Network of EXperts, Unified in Strategy)
- "Nexus" também significa independentemente "ponto central de conexão" -- perfeito para um command center
- "Spatial" é o descritor padrão da indústria que Apple e o mercado normalizaram
- Foneticamente equilibrado: três sílabas, depois duas
- **Ação necessária:** Clearance de trademark nas Classes Nice 9, 42 e 38

### Personalidade da Marca: O Comandante

| Traço | Expressão | Evita |
|-------|------------|--------|
| **Autoritativa** | Clara, direta, tecnicamente precisa | Hype, superlativos, futurismo vago |
| **Composta** | Design limpo, ritmo medido, white space | Urgência pela urgência, caos |
| **Pioneira** | Orgulho discreto, referências sutis ao novo paradigma | "Revolucionário", "game-changing" |
| **Precisa** | Specs exatas, métricas reais, requisitos honestos | Claims vagos, buzzwords de marketing |
| **Acessível** | Linguagem natural de interação, metáforas espaciais | Condescendência, gatekeeping |

### Taglines (Ranqueadas)

1. **"Mission Control for the Agent Era"** -- PRIMÁRIA RECOMENDADA
2. "See Your Agents in Space"
3. "Orchestrate in Three Dimensions"
4. "Where AI Operations Become Spatial"
5. "Command Center. Reimagined in Space."
6. "The Dimension Your Dashboards Are Missing"
7. "AI Agents Deserve More Than Flat Screens"

### Sistema de Cores

| Cor | Hex | Uso |
|-------|-----|-------|
| Deep Space Indigo | `#1B1F3B` | Canvas escuro fundamental, backgrounds |
| Nexus Blue | `#4A7BF7` | Marca assinatura, ações primárias |
| Signal Cyan | `#00D4FF` | Destaques espaciais, conexões de dados |
| Command Green | `#00E676` | Sistemas saudáveis, sucesso |
| Alert Amber | `#FFB300` | Avisos, atenção necessária |
| Critical Red | `#FF3D71` | Erros, falhas |

Proporção de uso: Deep Space Indigo 60%, Nexus Blue 25%, Signal Cyan 10%, Semânticas 5%.

### Tipografia

- **Primária:** Inter (UI, corpo, labels)
- **Monospace:** JetBrains Mono (código, logs, saída de agentes)
- **Display:** Space Grotesk (apenas headlines de marketing)

### Conceitos de Logo

Três direções para exploração:

1. **The Spatial Nexus Mark** -- Linhas convergentes se encontrando em um nó central luminoso com profundidade sutil de perspectiva
2. **The Dimensional Window** -- Viewport estilizado com linhas de perspectiva criando o efeito de olhar para um espaço 3D
3. **The Orbital Array** -- Anéis orbitais ao redor de um ponto central sugerindo agentes coordenados em movimento

### Valores da Marca

- **Spatial Truthfulness** -- Representação honesta do estado do sistema, sem suavização cosmética
- **Operational Gravity** -- Construído para produção, não demos
- **Dimensional Generosity** -- WebXR garante que valor espacial seja acessível a todos
- **Composure Under Complexity** -- Quanto mais complexo o sistema, mais calma a interface

### Design Tokens

```css
:root {
  --nxs-deep-space:       #1B1F3B;
  --nxs-blue:             #4A7BF7;
  --nxs-cyan:             #00D4FF;
  --nxs-green:            #00E676;
  --nxs-amber:            #FFB300;
  --nxs-red:              #FF3D71;
  --nxs-void:             #0A0E1A;
  --nxs-slate-900:        #141829;
  --nxs-slate-700:        #2A2F45;
  --nxs-slate-500:        #4A5068;
  --nxs-slate-300:        #8B92A8;
  --nxs-slate-100:        #C8CCE0;
  --nxs-cloud:            #E8EBF5;
  --nxs-white:            #F8F9FC;
  --nxs-font-primary:     'Inter', sans-serif;
  --nxs-font-mono:        'JetBrains Mono', monospace;
  --nxs-font-display:     'Space Grotesk', sans-serif;
}
```

---

## 5. Go-to-Market e Growth

**Agente:** Growth Hacker

### North Star Metric

**Weekly Active Pipelines (WAP)** -- pipelines únicos de agentes com pelo menos uma interação espacial nos últimos 7 dias. Captura criação e engajamento, se correlaciona com valor e não é facilmente manipulável.

### Pricing

| Tier | Anual | Mensal | Alvo |
|------|--------|---------|--------|
| Explorer | Free | Free | 3 pipelines, preview WebXR, comunidade |
| Pro | $29/usuário/mês | $39/usuário/mês | Pipelines ilimitados, VisionOS, histórico de 30 dias |
| Team | $59/usuário/mês | $79/usuário/mês | Colaboração, RBAC, SSO, histórico de 90 dias |
| Enterprise | Custom (~$150+) | Custom | Infra dedicada, SLA, opção on-prem |

Estratégia: reverse trial de 14 dias (features Pro, depois downgrade para Free). Meta de conversão free-to-paid de 5-8%.

### GTM em 3 Fases

**Fase 1: Founder-Led Sales (Meses 1-3)**
- Alvo: Engenheiros de IA individuais em startups que usam LangChain/CrewAI e possuem Vision Pro
- Táticas: DM para 200 engenheiros de IA de alto perfil, posts semanais build-in-public, demos de 30 segundos
- Canais: X/Twitter, LinkedIn, servidores Discord focados em IA, Reddit

**Fase 2: Comunidade de Desenvolvedores (Meses 4-6)**
- Lançamento no Product Hunt (programado para esta fase, não Fase 1)
- Hacker News Show HN, artigos Dev.to, palestras em conferências
- Anúncios de integração com frameworks populares de IA

**Fase 3: Enterprise (Meses 7-12)**
- Pipeline de referral enterprise da Apple, campanhas LinkedIn ABM
- Estudos de caso enterprise, briefings com analistas (Gartner, Forrester)
- Primeira contratação de AE enterprise, compliance SOC 2

### Growth Loops

1. **Loop de Demo "Wow Factor"** -- Demos espaciais são inerentemente compartilháveis. "Share Spatial Preview" com um clique gera link WebXR ou vídeo. Meta K = 0,3-0,5.
2. **Template Marketplace** -- Power users publicam templates de pipeline, descobertos via busca, gerando novos signups.
3. **Expansão de Seats por Colaboração** -- Um engenheiro adota, compartilha com colegas, o time expande para plano pago (playbook Slack/Figma).
4. **Descoberta por Integrações** -- Listagens nos diretórios de parceiros LangChain, n8n, OpenAI/Anthropic.

### Estratégia Open-Source

**Open-source (Apache 2.0):**
- `nexus-spatial-sdk` -- SDK TypeScript/Python para conectar frameworks de agentes
- `nexus-webxr-components` -- Biblioteca de componentes React Three Fiber para pipelines 3D
- `nexus-agent-schemas` -- Schemas padronizados para representar pipelines de agentes em 3D

**Manter proprietário:** App VisionOS nativo, engine de colaboração, features enterprise, infraestrutura hosted.

### Metas de Receita

| Métrica | Mês 6 | Mês 12 |
|--------|---------|----------|
| MRR | $8K-15K | $50K-80K |
| Contas free | 5.000 | 15.000 |
| Seats pagos | 300 | 1.200 |
| Membros no Discord | 2.000 | 5.000 |
| GitHub stars (SDK) | 500 | 2.000 |

### Primeiro Budget de $50K

| Categoria | Valor | % |
|----------|--------|---|
| Produção de Conteúdo | $12.000 | 24% |
| Developer Relations | $10.000 | 20% |
| Testes de Aquisição Paga | $8.000 | 16% |
| Comunidade e Ferramentas | $5.000 | 10% |
| Product Hunt e Launch | $3.000 | 6% |
| Manutenção Open Source | $3.000 | 6% |
| PR e Outreach | $4.000 | 8% |
| Parcerias | $2.000 | 4% |
| Reserva | $3.000 | 6% |

### Principais Parcerias

- **Tier 1 (Crítico):** Anthropic, OpenAI -- integrações de API first-class, listagens em partner programs
- **Tier 2 (Adoção):** LangChain, CrewAI, n8n -- integrações com frameworks, cross-pollination de comunidades
- **Tier 3 (Plataforma):** Apple -- developer kit Vision Pro, destaque na App Store, WWDC
- **Tier 4 (Ecossistema):** GitHub, Hugging Face, Docker -- integrações com plataformas de desenvolvedores

### Fontes

- [AI Orchestration Market Size - MarketsandMarkets](https://www.marketsandmarkets.com/Market-Reports/ai-orchestration-market-148121911.html)
- [Spatial Computing Market - Precedence Research](https://www.precedenceresearch.com/spatial-computing-market)
- [How to Price AI Products - Aakash Gupta](https://www.news.aakashg.com/p/how-to-price-ai-products)
- [Product Hunt Launch Guide 2026](https://calmops.com/indie-hackers/product-hunt-launch-guide/)

---

## 6. Blueprint de Customer Support

**Agente:** Support Responder

### Estrutura de Tiers de Suporte

| Atributo | Explorer (Free) | Builder (Pro) | Command (Enterprise) |
|-----------|-----------------|---------------|---------------------|
| SLA de Primeira Resposta | Best effort (48h) | 4 horas (horário comercial) | 30 min (P1), 2h (P2) |
| SLA de Resolução | 5 dias úteis | 24h (P1/P2), 72h (P3) | 4h (P1), 12h (P2) |
| Canais | Comunidade, KB, assistente de IA | + Live chat, email, vídeo (2/mês) | + Slack dedicado, CSE nomeado, 24/7 |
| Escopo | Perguntas gerais, docs | Troubleshooting técnico, integrações | Integração completa, design customizado, compliance |

### Definições de Prioridade

- **P1 Crítica:** Orquestração fora do ar, risco de perda de dados, violação de segurança
- **P2 Alta:** Feature principal degradada, workaround existe
- **P3 Média:** Issues não bloqueantes, glitches menores
- **P4 Baixa:** Feature requests, issues cosméticas

### The Nexus Guide: Suporte In-Product com IA

A decisão de design de destaque: o agente de suporte vive como um nó visível **dentro do workspace espacial do usuário**. Ele tem contexto completo do layout do usuário, agentes ativos e erros recentes.

**Capacidades:**
- Q&A em linguagem natural sobre features
- Diagnósticos de agentes em tempo real ("Por que o Agente X está lento?")
- Sugestões de configuração ("Sua topologia performaria melhor como uma mesh")
- Walkthroughs guiados de troubleshooting espacial
- Criação de tickets com anexação automática de contexto

**Self-Healing:**

| Cenário | Detecção | Auto-Resolução |
|----------|-----------|-----------------|
| Loop infinito de agente | Spike de CPU/tokens | Encerrar e reiniciar com última config boa |
| Queda de frames de renderização | FPS abaixo do limite | Reduzir fidelidade visual, sugerir fechar painéis |
| Expiração de credenciais | Respostas API 401 | Solicitar re-auth, pausar agentes de forma graciosa |
| Timeout de comunicação | Spike de latência | Rerotear mensagens por caminho alternativo |

### Fluxo de Onboarding

Onboarding adaptativo baseado no perfil do usuário:

| Experiência com IA | Experiência Espacial | Caminho |
|---------------|-------------------|------|
| Baixa | Baixa | Tour guiado completo (20 min) |
| Alta | Baixa | Focado em espacial (12 min) |
| Baixa | Alta | Focado em agentes (12 min) |
| Alta | Alta | Setup expresso (5 min) |

Primeiro passo crítico: calibração espacial de 60 segundos (hand tracking, gaze, comfort check) antes de qualquer interação com o produto.

**Marco de Ativação** (usuário está "onboarded" quando):
- Criou pelo menos um agente customizado
- Conectou dois ou mais agentes em uma topologia
- Ancorou pelo menos um dashboard de monitoramento
- Retornou para uma terceira sessão

### Construção do Time

| Fase | Headcount | Funções |
|-------|-----------|-------|
| Meses 0-6 | 4 | Head of CX, 2 Support Engineers, Technical Writer |
| Meses 6-12 | 8 | + 2 Support Engineers, CSE, Community Manager, Ops Analyst |
| Meses 12-24 | 16 | + 4 Engineers (24/7), Spatial Specialist, Integration Specialist, KB Manager, Engineering Manager |

### Comunidade: Discord-First

```
NEXUS SPATIAL DISCORD
  INFORMATION: #announcements, #changelog, #status
  SUPPORT: #help-getting-started, #help-agents, #help-spatial
  DISCUSSION: #general, #show-your-workspace, #feature-requests
  PLATFORMS: #visionos, #webxr, #api-and-sdk
  EVENTS: office-hours (weekly voice), community-demos (monthly)
  PRO MEMBERS: #pro-lounge, #beta-testing
  ENTERPRISE: per-customer private channels
```

**Champions Program ("Nexus Navigators"):** 5-10 power users iniciais com badge Navigator, Slack direto com o time de produto, tier Pro gratuito, acesso antecipado a features e summit anual.

---

## 7. Pesquisa UX e Direção de Design

**Agente:** UX Researcher

### Personas de Usuário

**Maya Chen -- AI Platform Engineer (32, São Francisco)**
- Gerencia 15-30 workflows ativos de agentes, usa n8n + LangSmith
- Gasta 40% do tempo debugando falhas de agentes por inspeção de logs
- Cética sobre spatial computing: "Isso é realmente mais rápido, ou só mais legal?"
- Necessidade primária: Reduzir mean-time-to-diagnosis de 45 min para menos de 10

**David Okoro -- Technical Product Manager (38, Londres)**
- Revisa e aprova designs de workflows de agentes, apresenta para C-suite
- Não consegue contribuir significativamente para reviews de workflow porque ferramentas exigem entendimento em nível de código
- Necessidade primária: Entender e comunicar arquiteturas de agentes sem ler código

**Dr. Amara Osei -- Research Scientist (45, Zurique)**
- Desenha workflows de pesquisa multi-agent com comparações A/B
- Tem 12 variações do mesmo pipeline sem uma boa forma de comparar
- Necessidade primária: Comparação lado a lado de variantes de pipelines em espaço 3D

**Jordan Rivera -- Creative Technologist (27, Austin)**
- Usuário diário de Vision Pro, constrói instalações artísticas com IA
- Quer ferramentas que pareçam instrumentos, não dashboards
- Necessidade primária: Construir workflows de agentes rapidamente com feedback espacial imediato

### Achado Principal: Debugging É o Killer Use Case

Sobreposição espacial de runtime traces na estrutura do workflow resolve uma dor real e quantificada que nenhuma ferramenta 2D trata bem. Esse workflow deve receber o maior investimento de design e engenharia.

### Insight Crítico de Design

Espacial agrega valor para tarefas **estruturais** (posicionar, conectar, reorganizar nós), mas cria fricção para tarefas de **parâmetros** (entrada de texto, configuração). A interface deve misturar modos espacial e 2D de forma fluida -- painéis 2D ancorados em posições espaciais.

### 7 Princípios de Design

1. **Spatial Earns Its Place** -- Se 2D for mais claro, use 2D. Toda review deve perguntar: "Isso seria melhor plano?"
2. **Glanceable Before Inspectable** -- Informação crítica perceptível em menos de 2 segundos por cor, tamanho, movimento e posição
3. **Hands-Free Is the Baseline** -- Gaze + voz cobre todas as operações de leitura/navegação; mãos adicionam precisão, mas não são obrigatórias
4. **Respect Cognitive Gravity** -- Estenda modelos mentais 2D (fluxo esquerda-para-direita), não os substitua; eixo z adiciona camadas
5. **Progressive Spatial Complexity** -- Novos usuários começam quase-2D; capacidades espaciais aparecem conforme a confiança cresce
6. **Physical Metaphors, Digital Capabilities** -- Nós são "pegos" (físico), mas também duplicados e versionados (digital)
7. **Silence Is a Feature** -- Sistemas saudáveis parecem calmos; cor e movimento sinalizam desvio do normal

### Paradigma de Navegação: Semantic Zoom em 4 Níveis

| Nível | O Que Você Vê |
|-------|-------------|
| Fleet View | Todos os workflows como formas abstratas, codificadas por cor conforme status |
| Workflow View | Grafo de nós com labels e conexões |
| Node View | Configuração expandida, I/O recente, métricas de status |
| Trace View | Trace completo de execução com inspeção de dados |

### Resumo de UX Competitiva

| Capacidade | n8n | Flowise | LangSmith | Langflow | Meta Nexus Spatial |
|-----------|-----|---------|-----------|----------|---------------------|
| Construção visual de workflow | A | B+ | N/A | A | A+ (espacial) |
| Debugging/tracing | C+ | C | A | B | A+ (overlay espacial) |
| Monitoramento | B | C | A | B | A (spatial fleet) |
| Colaboração | D | D | C | D | A (co-presença espacial) |
| Escalabilidade de workflows grandes | C | C | B | C | A (espaço 3D) |

### Requisitos de Acessibilidade

- Toda interação alcançável por pelo menos duas modalidades
- Nenhuma informação transmitida apenas por cor
- Modo high-contrast, modo reduced-motion, modo depth-flattening
- Compatibilidade com screen reader com descrições de elementos espaciais
- Avisos de duração de sessão a cada 20-30 minutos
- Todas as tarefas centrais concluíveis sentado, com uma mão, dentro de um cone de movimento de 30 graus

### Plano de Pesquisa (16 Semanas)

| Fase | Semanas | Estudos |
|-------|-------|---------|
| Foundational | 1-4 | Entrevistas de modelo mental (15-20 participantes), análise competitiva de tarefas |
| Concept Validation | 5-8 | Teste de protótipo espacial Wizard-of-Oz, card sort 3D para IA |
| Usability Testing | 9-14 | Experiência de primeiro uso (20 usuários), diary study longitudinal de 4 semanas, teste de colaboração em pares |
| Accessibility Audit | 12-16 | Avaliação heurística especialista, testes com usuários com deficiência |

---

## 8. Plano de Execução do Projeto

**Agente:** Project Shepherd

### Timeline: 35 Semanas (9 de março -- 6 de novembro de 2026)

| Fase | Semanas | Duração | Objetivo |
|-------|-------|----------|------|
| Discovery e Pesquisa | W1-3 | 3 semanas | Validar viabilidade, definir escopo |
| Foundation | W4-9 | 6 semanas | Infraestrutura central, shells das duas plataformas, design system |
| Build do MVP | W10-19 | 10 semanas | Agent command center single-user com orquestração |
| Beta | W20-27 | 8 semanas | Colaboração, polish, hardening, 50-100 beta users |
| Launch | W28-31 | 4 semanas | Launch na App Store + web, push de marketing |
| Scale | W32-35+ | Contínuo | Plugin marketplace, features avançadas, growth |

### Marco Crítico: Semana 12 (29 de maio)

**Primeira execução end-to-end de workflow.** Um usuário cria e roda um workflow de agentes com 3 nós em 3D. Este é o momento em que o produto prova sua proposta de valor central. Se isso atrasar, tudo a jusante muda.

### Primeiros 6 Sprints (65 Tickets)

**Sprint 1 (9-20 mar):** Auditoria do SDK VisionOS, matriz de compatibilidade WebXR, viabilidade do orchestration engine, entrevistas com stakeholders, protótipos descartáveis para ambas as plataformas.

**Sprint 2 (23 mar - 3 abr):** Architecture decision records, lock de escopo do MVP com MoSCoW, PRD v1.0, pesquisa de padrões de UI espacial, definição do modelo de interação, kickoff do design system.

**Sprint 3 (6-17 abr):** Setup de monorepo, auth service (OAuth2), schema de banco, API gateway, init do projeto Xcode VisionOS, init do projeto WebXR, pipelines CI/CD.

**Sprint 4 (20 abr - 1 mai):** Servidor WebSocket + client SDKs, gestão de janelas espaciais, biblioteca de componentes 3D, camada de input de hand tracking, CRUD de times, integration tests.

**Sprint 5 (4-15 mai):** Core do orchestration engine (Rust), state machine de agentes, renderers de grafo de nós (ambas as plataformas), interface de plugin v0, plugin provider OpenAI.

**Sprint 6 (18-29 mai):** Persistência + versionamento de workflows, execução DAG, visualização de execução em tempo real, plugin provider Anthropic, integração de eye tracking, spatial audio.

### Alocação de Times

5 squads operando ao longo das fases:

| Squad | Membros Centrais | Fases Ativas |
|-------|-------------|---------------|
| Core Architecture | Backend Architect, XR Interface Architect, Senior Dev, VisionOS Engineer | Discovery até MVP |
| Spatial Experience | XR Immersive Dev, XR Cockpit Specialist, Metal Engineer, UX Architect, UI Designer | Foundation até Beta |
| Orchestration | AI Engineer, Backend Architect, Senior Dev, API Tester | MVP até Beta |
| Platform Delivery | Frontend Dev, Mobile App Builder, VisionOS Engineer, DevOps | MVP até Launch |
| Launch | Growth Hacker, Content Creator, App Store Optimizer, Visual Storyteller, Brand Guardian | Beta até Scale |

### Top 5 Riscos

| Risco | Probabilidade | Impacto | Mitigação |
|------|------------|--------|------------|
| Apple rejeita app VisionOS | Média | Crítico | Engajar Apple Developer Relations na Semana 4, pre-review até Semana 20 |
| Fragmentação de browsers WebXR | Alta | Alto | Matriz de suporte de browsers na Semana 1, testes cross-browser automatizados |
| Conflitos de sync multi-user | Média | Alto | Sync baseado em CRDT (Yjs) desde o início, protótipo em Foundation |
| Orquestração não escala | Média | Crítico | Scaling horizontal desde o dia um, load test a 10x até Semana 22 |
| Performance RealityKit para 100+ nós | Média | Alto | Fazer profiling cedo, implementar LOD culling, renderização instanciada |

### Budget: $121.500 -- $155.500 (Não-Pessoal)

| Categoria | Custo Estimado |
|----------|---------------|
| Infraestrutura cloud (35 semanas) | $35.000 - $45.000 |
| Hardware (3 Vision Pro, 2 Quest 3, Mac Studio) | $17.500 |
| Licenças e serviços | $15.000 - $20.000 |
| Serviços externos (jurídico, segurança, PR) | $30.000 - $45.000 |
| Custos de API de IA (dev/teste) | $8.000 |
| Contingência (15%) | $16.000 - $20.000 |

---

## 9. Arquitetura de Interface Espacial

**Agente:** XR Interface Architect

### O Command Theater

O workspace é organizado como um teatro curvo ao redor do usuário:

```
                        OVERVIEW CANOPY
                     (pipeline topology)
                    ~~~~~~~~~~~~~~~~~~~~~~~~
                   /                        \
                  /     FOCUS ARC (120 deg)   \
                 /    primary node graph work   \
                /________________________________\
               |                                  |
    LEFT       |        USER POSITION             |       RIGHT
    UTILITY    |        (origin 0,0,0)            |       UTILITY
    RAIL       |                                  |       RAIL
               |__________________________________|
                \                                /
                 \      SHELF (below sightline) /
                  \   agent status, quick tools/
                   \_________________________ /
```

- **Focus Arc** (120 graus, 1,2-2,0m): Workspace primário do grafo de nós
- **Overview Canopy** (acima, 2,5-4,0m): Topologia miniaturizada do pipeline + health heatmap
- **Utility Rails** (flancos esquerdo/direito): Biblioteca de agentes, monitoramento, logs
- **Shelf** (abaixo da linha de visão, 0,8-1,0m): Run/stop, undo/redo, ferramentas rápidas

### Sistema de Profundidade em Três Camadas

| Camada | Profundidade | Conteúdo | Opacidade |
|-------|-------|---------|---------|
| Foreground | 0,8 - 1,2m | Painéis ativos, inspectors, modals | 100% |
| Midground | 1,2 - 2,5m | Grafo de nós, conexões, workspace | 100% |
| Background | 2,5 - 5,0m | Mapa overview, status ambiente | 40-70% |

### Grafo de Nós em 3D

**Dados fluem em direção ao usuário.** Nós se organizam ao longo do eixo z por ordem de execução:

```
USER (here)
  z=0.0m   [Output Nodes]     -- Results
  z=0.3m   [Transform Nodes]  -- Processors
  z=0.6m   [Agent Nodes]      -- LLM calls
  z=0.9m   [Retrieval Nodes]  -- RAG, APIs
  z=1.2m   [Input Nodes]      -- Triggers
```

Branches paralelos se espalham horizontalmente (eixo x). Branches condicionais se espalham verticalmente (eixo y).

**Representação de nós (3 LODs):**
- **LOD-0** (repouso, >1,5m): Retângulo de vidro fosco 12x8cm com ícone de tipo, nome e brilho de status
- **LOD-1** (hover, 400ms de gaze): Expande para 14x10cm, revela portas e informações da última execução
- **LOD-2** (selecionado): Desliza para foreground, expande para painel de detalhe 30x40cm com edição de config ao vivo

**Conexões como tubos luminosos:**
- 4mm de diâmetro em repouso, 8mm quando carregando dados
- Codificação por cor conforme tipo de dado (branco=texto, cyan=estruturado, magenta=imagens, amber=áudio, verde=tool calls)
- Partículas animadas mostram direção e velocidade do fluxo
- Auto-bundle quando >3 rodam em paralelo entre as mesmas camadas

### 7 Estados de Agente

| Estado | Brilho da Aresta | Interior | Som | Partículas |
|-------|-----------|----------|-------|-----------|
| Idle | Verde estável, baixo | Vidro fosco estático | Nenhum | Nenhuma |
| Queued | Amber pulsando, 1Hz | Rotação sutil | Nenhum | Drift lento na entrada |
| Running | Azul estável, médio | Shimmer animado | Hum espacial suave | Fluxo rápido nas conexões |
| Streaming | Azul + stream de saída | Shimmer + fragmentos de texto | Hum | Fragmentos de texto fluindo para frente |
| Completed | Flash branco, depois verde | Estático | Chime de conclusão | Nenhuma |
| Error | Vermelho pulsando, 2Hz | Tom vermelho | Tom de alerta (uma vez) | Nenhuma |
| Paused | Amber estável | Freeze-frame + ícone de pausa | Nenhum | Congeladas no lugar |

### Modelo de Interação

| Ação | VisionOS | Controllers WebXR | Voz |
|--------|----------|-------------------|-------|
| Selecionar nó | Gaze + pinch | Point ray + trigger | "Select [name]" |
| Mover nó | Pinch + drag | Grip + move | -- |
| Conectar portas | Pinch na porta + drag | Trigger na porta + drag | "Connect [A] to [B]" |
| Pan do workspace | Drag com duas mãos | Thumbstick | "Pan left/right" |
| Zoom | Spread/pinch com duas mãos | Push/pull no thumbstick | "Zoom in/out" |
| Inspecionar nó | Pinch + puxar para si | Double-trigger | "Inspect [name]" |
| Rodar pipeline | Toque no botão Shelf | Botão trigger | "Run pipeline" |
| Undo | Double-tap com dois dedos | Botão B | "Undo" |

### Presença de Colaboração

Cada colaborador representado por:
- **Head proxy:** Esfera translúcida com imagem de perfil, gira com a orientação da cabeça
- **Hand proxies:** Modelos de mão fantasmados mostrando estados de pinch/grab
- **Gaze cone:** Cone sutil de 10 graus mostrando para onde estão olhando
- **Name label:** Renderizado como billboard, mostra ação atual ("editing Node X")

**Resolução de conflitos:** Primeiro editor recebe write lock; o segundo vê "locked by [name]" com opção de solicitar acesso ou duplicar o nó.

### Layout Adaptativo

| Ambiente | Escala dos Nós | Máx. Nós LOD-2 | Z-Spread do Grafo |
|-------------|-----------|-----------------|----------------|
| VisionOS Window | 4x3cm | 5 | 0,05m/camada |
| VisionOS Immersive | 12x8cm | 15 | 0,3m/camada |
| WebXR Desktop | 120x80px | 8 (overlays) | Projeção em perspectiva |
| WebXR Immersive | 12x8cm | 12 | 0,3m/camada |

### Coreografia de Transição

Todas as transições servem wayfinding. Máximo de 600ms para transições grandes, 200ms para menores, 0ms para seleção.

| Transição | Duração | Movimento-Chave |
|-----------|----------|------------|
| Overview para Focus | 600ms | Câmera deriva até o alvo, outras regiões desvanecem para 30% |
| Focus para Detail | 500ms | Nó desliza para frente, expande, conexões destacam |
| Detail para Overview | 600ms | Painel colapsa, nó recua, topologia completa fica visível |
| Troca de Zona | 500ms | Atual desliza lateralmente para fora, nova desliza para dentro |
| Window para Immersive | 1000ms | Bordas dissolvem, nós expandem para posições espaciais completas |

### Medidas de Conforto

- Nenhum movimento iniciado por câmera sem ação do usuário
- Horizonte estável (plano horizontal nunca inclina)
- Interação primária entre 0,8-2,5m, +/-15 graus da linha dos olhos
- Prompt de descanso após 45 minutos (mudança de iluminação ambiente, não modal)
- Vinheta periférica durante movimento rápido
- Todos os controles usados com frequência acessíveis com braços ao lado do corpo (apenas punho/dedos)

---

## 10. Síntese Cross-Agent

### Pontos de Acordo Entre Todos os 8 Agentes

1. **2D-first, spatial-second.** Todo agente chegou independentemente a esta conclusão. Construa primeiro um ótimo dashboard web, depois adicione capacidades espaciais progressivamente.

2. **Debugging é o killer use case.** Product Researcher, UX Researcher e XR Interface Architect convergiram nisso: overlay espacial de runtime traces sobre a estrutura do workflow é onde 3D realmente supera 2D.

3. **WebXR acima de VisionOS para alcance inicial.** A base instalada de ~1M do Vision Pro não sustenta um negócio. WebXR no browser é o desbloqueio de distribuição.

4. **O cenário de colaboração "war room".** Múltiplos agentes destacaram resposta colaborativa a incidentes como a proposta de valor espacial mais forte -- times entrando em um espaço 3D compartilhado para debugar juntos um pipeline com falha.

5. **Progressive disclosure é essencial.** UX Research, Spatial UI e Support enfatizaram que complexidade espacial deve ser revelada gradualmente, nunca despejada sobre um usuário de primeira viagem.

6. **Voz como acelerador de power users.** UX Researcher e XR Interface Architect identificaram comandos de voz como a "linha de comando do spatial computing" -- essencial para acessibilidade e eficiência de especialistas.

### Tensões-Chave a Resolver

| Tensão | Posição A | Posição B | Resolução Necessária |
|---------|-----------|-----------|-------------------|
| **Pricing** | Growth Hacker: $29-59/usuário/mês | Trend Researcher: $99-249/usuário/mês | A/B test no beta |
| **Prioridade VisionOS** | Arquitetura: Fase 3 (Semana 13+) | Spatial UI: Spec completa pronta | Construir WebXR primeiro, VisionOS quando validado |
| **Linguagem de orquestração** | Arquitetura: Rust | Plano de Projeto: Não especificado | Rust é correto para execução DAG crítica de performance |
| **Escopo do MVP** | Arquitetura: Apenas 2D na Fase 1 | Marca: Liderar com espacial | 2D primeiro, mas garantir espacial em toda demo |
| **Plataforma de comunidade** | Support: Discord-first | Marketing: Discord + open-source | Ambos -- Discord para comunidade, GitHub para engajamento developer |

### O Que Este Exercício Demonstra

Este documento de discovery foi produzido por 8 agentes especializados rodando em paralelo, cada um trazendo expertise profunda de domínio para um objetivo compartilhado. Os agentes chegaram independentemente a conclusões consistentes enquanto trouxeram insights específicos de domínio que seriam difíceis para qualquer generalista produzir sozinho:

- O **Product Trend Researcher** encontrou os dados sóbrios de vendas do Vision Pro que reestruturaram a estratégia inteira
- O **Backend Architect** desenhou um orchestration engine em Rust que um time focado em marketing dificilmente teria considerado
- O **Brand Guardian** criou uma categoria ("SpatialAIOps") em vez de competir em uma já existente
- O **UX Researcher** identificou que spatial computing cria fricção em tarefas de parâmetros -- um achado contraintuitivo
- O **XR Interface Architect** desenhou a topologia "dados fluem em sua direção", que mapeia cognição espacial natural
- O **Project Shepherd** identificou os três papéis-gargalo críticos que poderiam descarrilar toda a timeline
- O **Growth Hacker** desenhou loops virais específicos à compartilhabilidade inerente do spatial computing
- O **Support Responder** transformou as próprias capacidades de IA do produto em um diferencial de suporte

O resultado é um plano de produto abrangente e cross-functional que poderia servir como base para desenvolvimento real -- produzido em uma única sessão por uma agência de agentes de IA trabalhando em conjunto.
