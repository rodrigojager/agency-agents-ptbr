# Workflow Multi-Agent: MVP de Startup

> Um exemplo passo a passo de como coordenar múltiplos agentes para ir de ideia a MVP lançado.

## O Cenário

Você está construindo um MVP SaaS — uma ferramenta de retrospectiva de equipe para times remotos. Você tem 4 semanas para lançar um produto funcional com cadastros de usuários, uma feature central e uma landing page.

## Time de Agentes

| Agente | Função neste workflow |
|-------|---------------------|
| Sprint Prioritizer | Quebrar o projeto em sprints semanais |
| UX Researcher | Validar a ideia com entrevistas rápidas com usuários |
| Backend Architect | Desenhar a API e o modelo de dados |
| Frontend Developer | Construir o app React |
| Rapid Prototyper | Colocar a primeira versão rodando rápido |
| Growth Hacker | Planejar estratégia de lançamento enquanto o build acontece |
| Reality Checker | Validar cada milestone antes de avançar |

## O Workflow

### Semana 1: Discovery + Arquitetura

**Etapa 1 — Ativar Sprint Prioritizer**

```
Activate Sprint Prioritizer.

Project: RetroBoard — a real-time team retrospective tool for remote teams.
Timeline: 4 weeks to MVP launch.
Core features: user auth, create retro boards, add cards, vote, action items.
Constraints: solo developer, React + Node.js stack, deploy to Vercel + Railway.

Break this into 4 weekly sprints with clear deliverables and acceptance criteria.
```

**Etapa 2 — Ativar UX Researcher (em paralelo)**

```
Activate UX Researcher.

I'm building a team retrospective tool for remote teams (5-20 people).
Competitors: EasyRetro, Retrium, Parabol.

Run a quick competitive analysis and identify:
1. What features are table stakes
2. Where competitors fall short
3. One differentiator we could own

Output a 1-page research brief.
```

**Etapa 3 — Handoff para Backend Architect**

```
Activate Backend Architect.

Here's our sprint plan: [paste Sprint Prioritizer output]
Here's our research brief: [paste UX Researcher output]

Design the API and database schema for RetroBoard.
Stack: Node.js, Express, PostgreSQL, Socket.io for real-time.

Deliver:
1. Database schema (SQL)
2. REST API endpoints list
3. WebSocket events for real-time board updates
4. Auth strategy recommendation
```

### Semana 2: Construir Features Centrais

**Etapa 4 — Ativar Frontend Developer + Rapid Prototyper**

```
Activate Frontend Developer.

Here's the API spec: [paste Backend Architect output]

Build the RetroBoard React app:
- Stack: React, TypeScript, Tailwind, Socket.io-client
- Pages: Login, Dashboard, Board view
- Components: RetroCard, VoteButton, ActionItem, BoardColumn

Start with the Board view — it's the core experience.
Focus on real-time: when one user adds a card, everyone sees it.
```

**Etapa 5 — Reality Check no meio do caminho**

```
Activate Reality Checker.

We're at week 2 of a 4-week MVP build for RetroBoard.

Here's what we have so far:
- Database schema: [paste]
- API endpoints: [paste]
- Frontend components: [paste]

Evaluate:
1. Can we realistically ship in 2 more weeks?
2. What should we cut to make the deadline?
3. Any technical debt that will bite us at launch?
```

### Semana 3: Polish + Landing Page

**Etapa 6 — Frontend Developer continua, Growth Hacker começa**

```
Activate Growth Hacker.

Product: RetroBoard — team retrospective tool, launching in 1 week.
Target: Engineering managers and scrum masters at remote-first companies.
Budget: $0 (organic launch only).

Create a launch plan:
1. Landing page copy (hero, features, CTA)
2. Launch channels (Product Hunt, Reddit, Hacker News, Twitter)
3. Day-by-day launch sequence
4. Metrics to track in week 1
```

### Semana 4: Launch

**Etapa 7 — Reality Check Final**

```
Activate Reality Checker.

RetroBoard is ready to launch. Evaluate production readiness:

- Live URL: [url]
- Test accounts created: yes
- Error monitoring: Sentry configured
- Database backups: daily automated

Run through the launch checklist and give a GO / NO-GO decision.
Require evidence for each criterion.
```

## Padrões-Chave

1. **Handoffs sequenciais**: A saída de cada agente vira a entrada do agente seguinte
2. **Trabalho paralelo**: UX Researcher e Sprint Prioritizer podem rodar simultaneamente na Semana 1
3. **Quality gates**: Reality Checker no meio e antes do launch evita envio de código quebrado
4. **Passagem de contexto**: Sempre cole as saídas dos agentes anteriores no próximo prompt — agentes não compartilham memória

## Dicas

- Copie e cole as saídas dos agentes entre etapas — não resuma, use a saída completa
- Se um Reality Checker sinalizar uma issue, volte ao especialista relevante para corrigi-la
- Tenha o agente Orchestrator em mente para automatizar esse fluxo quando você estiver confortável com a versão manual
