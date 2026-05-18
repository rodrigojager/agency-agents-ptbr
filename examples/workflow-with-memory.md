# Workflow Multi-Agent: MVP de Startup com Memória Persistente

> O mesmo workflow de MVP de startup de [workflow-startup-mvp.md](workflow-startup-mvp.md), mas com um servidor de memória MCP cuidando do estado entre agentes. Sem mais handoffs por copy-paste.

## O Problema dos Handoffs Manuais

No workflow padrão, toda transição de agente para agente se parece com isto:

```
Activate Backend Architect.

Here's our sprint plan: [paste Sprint Prioritizer output]
Here's our research brief: [paste UX Researcher output]

Design the API and database schema for RetroBoard.
...
```

Você é a cola. Você copia e cola saídas entre agentes, acompanha o que já foi feito e torce para não perder contexto pelo caminho. Funciona para projetos pequenos, mas quebra quando:

- Sessões expiram e você perde a saída
- Múltiplos agentes precisam do mesmo contexto
- QA falha e você precisa voltar para um estado anterior
- O projeto se estende por dias ou semanas em muitas sessões

## A Correção

Com um servidor de memória MCP instalado, agentes armazenam seus entregáveis na memória e recuperam automaticamente o que precisam. Handoffs se tornam:

```
Activate Backend Architect.

Project: RetroBoard. Recall previous context for this project
and design the API and database schema.
```

O agente pesquisa na memória por contexto do RetroBoard, encontra o sprint plan e o research brief armazenados por agentes anteriores e continua a partir dali.

## Setup

Instale qualquer servidor de memória compatível com MCP que dê suporte às operações `remember`, `recall` e `rollback`. Veja [integrations/mcp-memory/README.md](../integrations/mcp-memory/README.md) para setup.

## O Cenário

Igual ao workflow padrão: uma ferramenta SaaS de retrospectiva de equipe (RetroBoard), 4 semanas até o MVP, desenvolvedor solo.

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

Cada agente tem uma seção Memory Integration em seu prompt (veja [integrations/mcp-memory/README.md](../integrations/mcp-memory/README.md) para saber como adicioná-la).

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
Remember your sprint plan tagged for this project when done.
```

O Sprint Prioritizer produz o sprint plan e o armazena na memória com as tags `sprint-prioritizer`, `retroboard` e `sprint-plan`.

**Etapa 2 — Ativar UX Researcher (em paralelo)**

```
Activate UX Researcher.

I'm building a team retrospective tool for remote teams (5-20 people).
Competitors: EasyRetro, Retrium, Parabol.

Run a quick competitive analysis and identify:
1. What features are table stakes
2. Where competitors fall short
3. One differentiator we could own

Output a 1-page research brief. Remember it tagged for this project when done.
```

O UX Researcher armazena o research brief com as tags `ux-researcher`, `retroboard` e `research-brief`.

**Etapa 3 — Handoff para Backend Architect**

```
Activate Backend Architect.

Project: RetroBoard. Recall the sprint plan and research brief from previous agents.
Stack: Node.js, Express, PostgreSQL, Socket.io for real-time.

Design:
1. Database schema (SQL)
2. REST API endpoints list
3. WebSocket events for real-time board updates
4. Auth strategy recommendation

Remember each deliverable tagged for this project and for the frontend-developer.
```

O Backend Architect recupera o sprint plan e o research brief da memória automaticamente. Sem copy-paste. Ele armazena seu schema e sua API spec com as tags `backend-architect`, `retroboard`, `api-spec` e `frontend-developer`.

### Semana 2: Construir Features Centrais

**Etapa 4 — Ativar Frontend Developer + Rapid Prototyper**

```
Activate Frontend Developer.

Project: RetroBoard. Recall the API spec and schema from the Backend Architect.

Build the RetroBoard React app:
- Stack: React, TypeScript, Tailwind, Socket.io-client
- Pages: Login, Dashboard, Board view
- Components: RetroCard, VoteButton, ActionItem, BoardColumn

Start with the Board view — it's the core experience.
Focus on real-time: when one user adds a card, everyone sees it.
Remember your progress tagged for this project.
```

O Frontend Developer puxa a API spec da memória e constrói contra ela.

**Etapa 5 — Reality Check no meio do caminho**

```
Activate Reality Checker.

Project: RetroBoard. We're at week 2 of a 4-week MVP build.

Recall all deliverables from previous agents for this project.

Evaluate:
1. Can we realistically ship in 2 more weeks?
2. What should we cut to make the deadline?
3. Any technical debt that will bite us at launch?

Remember your verdict tagged for this project.
```

O Reality Checker tem visibilidade total de tudo que foi produzido até aqui — sprint plan, research brief, schema, API spec e progresso frontend — sem você precisar coletar e colar tudo.

### Semana 3: Polish + Landing Page

**Etapa 6 — Frontend Developer continua, Growth Hacker começa**

```
Activate Growth Hacker.

Product: RetroBoard — team retrospective tool, launching in 1 week.
Target: Engineering managers and scrum masters at remote-first companies.
Budget: $0 (organic launch only).

Recall the project context and Reality Checker's verdict.

Create a launch plan:
1. Landing page copy (hero, features, CTA)
2. Launch channels (Product Hunt, Reddit, Hacker News, Twitter)
3. Day-by-day launch sequence
4. Metrics to track in week 1

Remember the launch plan tagged for this project.
```

### Semana 4: Launch

**Etapa 7 — Reality Check Final**

```
Activate Reality Checker.

Project: RetroBoard, ready to launch.

Recall all project context, previous verdicts, and the launch plan.

Evaluate production readiness:
- Live URL: [url]
- Test accounts created: yes
- Error monitoring: Sentry configured
- Database backups: daily automated

Run through the launch checklist and give a GO / NO-GO decision.
Require evidence for each criterion.
```

### Quando o QA Falha: Rollback

No workflow padrão, quando o Reality Checker rejeita um entregável, você volta ao agente responsável e tenta explicar o que deu errado. Com memória, o loop de recuperação é mais direto:

```
Activate Backend Architect.

Project: RetroBoard. The Reality Checker flagged issues with the API design.
Recall the Reality Checker's feedback and your previous API spec.
Roll back to your last known-good schema and address the specific issues raised.
Remember the updated deliverables when done.
```

O Backend Architect consegue ver exatamente o que o Reality Checker sinalizou, recuperar seu próprio trabalho anterior, voltar para um checkpoint e produzir uma correção — tudo sem você rastrear versões manualmente.

## Antes e Depois

| Aspecto | Workflow Padrão | Com Memória |
|--------|------------------|-------------|
| **Handoffs** | Copy-paste da saída completa entre agentes | Agentes recuperam automaticamente o que precisam |
| **Perda de contexto** | Timeouts de sessão perdem tudo | Memórias persistem entre sessões |
| **Contexto multi-agent** | Compilar contexto de N agentes manualmente | Agente pesquisa na memória pela tag do projeto |
| **Recuperação de falha de QA** | Descrever manualmente o que deu errado | Agente recupera feedback + faz rollback |
| **Projetos multi-dia** | Reestabelecer contexto a cada sessão | Agente continua de onde parou |
| **Setup necessário** | Nenhum | Instalar um servidor de memória MCP |

## Padrões-Chave

1. **Marque tudo com o nome do projeto**: É isso que faz o recall funcionar. Toda memória recebe a tag `retroboard` (ou qualquer que seja o nome do seu projeto).
2. **Marque entregáveis para o agente receptor**: Quando o Backend Architect termina uma API spec, ele marca a memória com `frontend-developer` para que o Frontend Developer a encontre no recall.
3. **Reality Checker tem visibilidade total**: Como todos os agentes armazenam seu trabalho na memória, o Reality Checker consegue recuperar tudo do projeto sem você compilar.
4. **Rollback substitui undo manual**: Quando algo falha, volte ao último checkpoint em vez de tentar descobrir o que mudou.

## Dicas

- Você não precisa modificar todos os agentes de uma vez. Comece adicionando Memory Integration aos agentes que você mais usa e expanda a partir daí.
- As instruções de memória são prompts, não código. O LLM interpreta e chama as ferramentas MCP conforme necessário. Você pode ajustar a redação ao seu estilo.
- Qualquer servidor de memória compatível com MCP que suporte as ferramentas `remember`, `recall`, `rollback` e `search` funcionará com este workflow.
