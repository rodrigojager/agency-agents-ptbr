# ⚙️ Playbook Fase 2 — Fundação & Scaffolding

> **Duração**: 3-5 dias | **Agentes**: 6 | **Gate Keepers**: DevOps Automator + Evidence Collector

---

## Objetivo

Construir a fundação técnica e operacional da qual todo trabalho posterior depende. Levantar o esqueleto antes de adicionar músculo. Depois desta fase, todo developer terá um ambiente funcional, um pipeline deployável e um design system para construir.

## Pré-Condições

- [ ] Quality Gate da Fase 1 aprovado (Pacote de Arquitetura aprovado)
- [ ] Pacote de Handoff da Fase 1 recebido
- [ ] Todos os documentos de arquitetura finalizados

## Sequência de Ativação dos Agentes

### Workstream A: Infraestrutura (Dia 1-3, Paralelo)

#### 🚀 DevOps Automator — Pipeline CI/CD + Infraestrutura
```
Ative DevOps Automator para setup de infraestrutura em [PROJETO].

Input: arquitetura de sistema do Backend Architect + requisitos de deployment
Entregáveis obrigatórios:
1. Pipeline CI/CD (GitHub Actions / GitLab CI)
   - Stage de security scanning
   - Stage de testes automatizados
   - Stage de build e containerização
   - Stage de deployment (blue-green ou canary)
   - Capacidade de rollback automatizado
2. Infrastructure as Code
   - Provisionamento de ambientes (dev, staging, production)
   - Setup de orquestração de containers
   - Configuração de rede e segurança
3. Configuração de Ambiente
   - Gestão de secrets
   - Gestão de variáveis de ambiente
   - Paridade multiambiente

Arquivos a criar:
- .github/workflows/ci-cd.yml (ou equivalente)
- infrastructure/ (templates Terraform/CDK)
- docker-compose.yml
- Dockerfile(s)

Formato: Pipeline CI/CD funcional com templates IaC
Timeline: 3 dias
```

#### 🏗️ Infrastructure Maintainer — Infraestrutura Cloud + Monitoramento
```
Ative Infrastructure Maintainer para setup de monitoramento em [PROJETO].

Input: infraestrutura do DevOps Automator + arquitetura do Backend Architect
Entregáveis obrigatórios:
1. Provisionamento de Recursos Cloud
   - Recursos de compute, storage e networking
   - Configuração de auto-scaling
   - Setup de load balancer
2. Stack de Monitoramento
   - Métricas de aplicação (Prometheus/DataDog)
   - Métricas de infraestrutura
   - Dashboards customizados (Grafana)
3. Logging e Alertas
   - Agregação centralizada de logs
   - Regras de alerta para thresholds críticos
   - Setup de notificações on-call
4. Security Hardening
   - Regras de firewall
   - Configuração SSL/TLS
   - Políticas de controle de acesso

Formato: Relatório de Prontidão de Infraestrutura com acesso a dashboards
Timeline: 3 dias
```

#### ⚙️ Studio Operations — Setup de Processo
```
Ative Studio Operations para setup de processos em [PROJETO].

Input: plano do Sprint Prioritizer + necessidades de coordenação do Project Shepherd
Entregáveis obrigatórios:
1. Workflow Git
   - Estratégia de branch (GitFlow / trunk-based)
   - Processo de PR review
   - Políticas de merge
2. Canais de Comunicação
   - Setup de canais do time
   - Roteamento de notificações
   - Cadência de status update
3. Templates de Documentação
   - Template de PR
   - Template de issue
   - Template de decision log
4. Ferramentas de Colaboração
   - Setup de project board
   - Configuração de sprint tracking

Formato: Playbook de Operações
Timeline: 2 dias
```

### Workstream B: Fundação da Aplicação (Dia 1-4, Paralelo)

#### 🎨 Frontend Developer — Scaffolding do Projeto + Biblioteca de Componentes
```
Ative Frontend Developer para scaffolding do projeto em [PROJETO].

Input: CSS Design System do UX Architect + identidade do Brand Guardian
Entregáveis obrigatórios:
1. Scaffolding do Projeto
   - Setup de framework (React/Vue/Angular conforme arquitetura)
   - Configuração TypeScript
   - Build tooling (Vite/Webpack/Next.js)
   - Framework de testes (Jest/Vitest + Testing Library)
2. Implementação do Design System
   - Design tokens CSS do UX Architect
   - Biblioteca de componentes base (Button, Input, Card, Layout)
   - Theme system (toggle light/dark/system)
   - Utilitários responsivos
3. Application Shell
   - Setup de routing
   - Componentes de layout (Header, Footer, Sidebar)
   - Implementação de error boundary
   - Loading states

Arquivos a criar:
- src/ (source da aplicação)
- src/components/ (biblioteca de componentes)
- src/styles/ (design tokens)
- src/layouts/ (componentes de layout)

Formato: Esqueleto funcional da aplicação com biblioteca de componentes
Timeline: 3 dias
```

#### 🏗️ Backend Architect — Fundação de Banco + API
```
Ative Backend Architect para fundação de API em [PROJETO].

Input: System Architecture Specification + Database Schema Design
Entregáveis obrigatórios:
1. Setup de Banco de Dados
   - Deployment de schema (migrations)
   - Criação de índices
   - Seed data para desenvolvimento
   - Configuração de connection pooling
2. Scaffold de API
   - Setup de framework (Express/FastAPI/etc.)
   - Estrutura de rotas alinhada à arquitetura
   - Stack de middleware (auth, validação, tratamento de erro, CORS)
   - Endpoints de health check
3. Sistema de Autenticação
   - Integração com auth provider
   - Gestão JWT/session
   - Scaffold de controle de acesso baseado em roles
4. Comunicação de Serviços
   - Setup de versionamento de API
   - Serialização de request/response
   - Padronização de respostas de erro

Arquivos a criar:
- api/ ou server/ (source backend)
- migrations/ (migrations de banco)
- docs/api-spec.yaml (especificação OpenAPI)

Formato: Scaffold funcional de API com banco de dados e auth
Timeline: 4 dias
```

#### 🏛️ UX Architect — Implementação do Sistema CSS
```
Ative UX Architect para implementação do sistema CSS em [PROJETO].

Input: identidade do Brand Guardian + própria spec de CSS Design System da Fase 1
Entregáveis obrigatórios:
1. Implementação de Design Tokens
   - CSS custom properties (cores, tipografia, spacing)
   - Paleta de cores de marca com nomenclatura semântica
   - Escala tipográfica com ajustes responsivos
2. Layout System
   - Sistema de containers (breakpoints responsivos)
   - Padrões de grid (2-col, 3-col, sidebar)
   - Utilitários Flexbox
3. Theme System
   - Variáveis de tema claro
   - Variáveis de tema escuro
   - Detecção de preferência do sistema
   - Componente de theme toggle
   - Transição suave entre temas

Arquivos a criar/atualizar:
- css/design-system.css (ou equivalente no framework)
- css/layout.css
- css/components.css
- js/theme-manager.js

Formato: CSS design system implementado com theme toggle
Timeline: 2 dias
```

## Checkpoint de Verificação (Dia 4-5)

### Verificação do Evidence Collector
```
Ative Evidence Collector para verificação da fundação da Fase 2.

Verifique o seguinte com evidência em screenshot:
1. Pipeline CI/CD executa com sucesso (mostrar logs do pipeline)
2. Esqueleto da aplicação carrega no browser (screenshot desktop)
3. Esqueleto da aplicação carrega no mobile (screenshot mobile)
4. Theme toggle funciona (screenshots light + dark)
5. Health check da API responde (output curl)
6. Banco de dados está acessível (status das migrations)
7. Dashboards de monitoramento estão ativos (screenshot do dashboard)
8. Biblioteca de componentes renderiza (página demo de componentes)

Formato: Pacote de Evidências com screenshots
Veredito: PASS / FAIL com issues específicas
```

## Checklist do Quality Gate

| # | Critério | Fonte de Evidência | Status |
|---|-----------|----------------|--------|
| 1 | Pipeline CI/CD faz build, testes e deploy | Logs de execução do pipeline | ☐ |
| 2 | Schema de banco implantado com todas as tabelas/índices | Output de sucesso das migrations | ☐ |
| 3 | Scaffold de API responde no health check | Evidência de resposta curl | ☐ |
| 4 | Esqueleto frontend renderiza no browser | Screenshots do Evidence Collector | ☐ |
| 5 | Dashboards de monitoramento mostram métricas | Screenshots dos dashboards | ☐ |
| 6 | Tokens do design system implementados | Demo da biblioteca de componentes | ☐ |
| 7 | Theme toggle funcional (light/dark/system) | Screenshots before/after | ☐ |
| 8 | Workflow Git e processos documentados | Playbook do Studio Operations | ☐ |

## Decisão de Gate

**Assinatura dupla obrigatória**: DevOps Automator (infraestrutura) + Evidence Collector (visual)

- **PASS**: Esqueleto funcional com pipeline DevOps completo → ativação da Fase 3
- **FAIL**: Issues específicas de infraestrutura ou aplicação → corrigir e reverificar

## Handoff para Fase 3

```markdown
## Pacote de Handoff Fase 2 → Fase 3

### Para todos os Developer Agents:
- Pipeline CI/CD funcional (auto-deploy em merge)
- Design system tokens e biblioteca de componentes
- Scaffold de API com auth e health checks
- Banco de dados com schema e seed data
- Workflow Git e processo de PR

### Para Evidence Collector (QA contínuo):
- URLs da aplicação (dev, staging)
- Metodologia de captura de screenshots
- Referência da biblioteca de componentes
- Guidelines de marca para verificação visual

### Para Agents Orchestrator (gestão do loop Dev↔QA):
- Backlog do Sprint Prioritizer (da Fase 1)
- Lista de tarefas com critérios de aceitação (da Fase 1)
- Matriz de atribuição de agentes (da estratégia NEXUS)
- Thresholds de qualidade para cada tipo de tarefa

### Acesso aos Ambientes:
- Ambiente dev: [URL]
- Ambiente staging: [URL]
- Dashboard de monitoramento: [URL]
- Pipeline CI/CD: [URL]
- Documentação da API: [URL]
```

---

*A Fase 2 está completa quando o skeleton da aplicação está rodando, o pipeline CI/CD está operacional e o Evidence Collector verificou todos os elementos da fundação com screenshots.*
