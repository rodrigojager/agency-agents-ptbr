# 🚨 Runbook: Incident Response

> **Modo**: NEXUS-Micro | **Duração**: Minutos a horas | **Agentes**: 3-8

---

## Cenário

Algo quebrou em produção. Usuários foram afetados. Velocidade de resposta importa, mas fazer do jeito certo também. Este runbook cobre da detecção ao post-mortem.

## Classificação de Severidade

| Nível | Definição | Exemplos | Tempo de Resposta |
|-------|-----------|----------|--------------|
| **P0 — Crítico** | Serviço completamente fora, perda de dados, breach de segurança | Corrupção de banco de dados, ataque DDoS, falha no sistema de auth | Imediato (all hands) |
| **P1 — Alto** | Feature principal quebrada, degradação significativa de performance | Processamento de pagamento fora, taxa de erro 50%+, latência 10x | < 1 hora |
| **P2 — Médio** | Feature menor quebrada, workaround disponível | Busca não funciona, erros de API não críticos | < 4 horas |
| **P3 — Baixo** | Issue cosmética, inconveniente menor | Bug de estilo, typo, glitch menor de UI | Próximo sprint |

## Times de Resposta por Severidade

### P0 — Time de Resposta Crítica
| Agente | Papel | Ação |
|-------|------|--------|
| **Infrastructure Maintainer** | Incident commander | Avaliar escopo, coordenar resposta |
| **DevOps Automator** | Deployment/rollback | Executar rollback se necessário |
| **Backend Architect** | Investigação de causa raiz | Diagnosticar issues de sistema |
| **Frontend Developer** | Investigação no lado da UI | Diagnosticar issues client-side |
| **Support Responder** | Comunicação com usuários | Updates na status page, notificações para usuários |
| **Executive Summary Generator** | Comunicação com stakeholders | Updates executivos em tempo real |

### P1 — Time de Resposta Alta
| Agente | Papel |
|-------|------|
| **Infrastructure Maintainer** | Incident commander |
| **DevOps Automator** | Suporte a deployment |
| **Relevant Developer Agent** | Implementação de fix |
| **Support Responder** | Comunicação com usuários |

### P2 — Resposta Média
| Agente | Papel |
|-------|------|
| **Relevant Developer Agent** | Implementação de fix |
| **Evidence Collector** | Verificar fix |

### P3 — Resposta Baixa
| Agente | Papel |
|-------|------|
| **Sprint Prioritizer** | Adicionar ao backlog |

## Sequência de Incident Response

### Passo 1: Detecção & Triagem (0-5 minutos)

```
TRIGGER: Alerta de monitoramento / Relato de usuário / Detecção por agente

Infrastructure Maintainer:
1. Confirmar alerta
2. Avaliar escopo e impacto
   - Quantos usuários afetados?
   - Quais serviços foram impactados?
   - Há dados em risco?
3. Classificar severidade (P0/P1/P2/P3)
4. Ativar time de resposta apropriado
5. Criar canal/thread de incidente

Output: Classificação do incidente + time de resposta ativado
```

### Passo 2: Investigação (5-30 minutos)

```
INVESTIGAÇÃO PARALELA:

Infrastructure Maintainer:
├── Checar métricas de sistema (CPU, memória, rede, disco)
├── Revisar logs de erro
├── Checar deployments recentes
└── Verificar dependências externas

Backend Architect (se P0/P1):
├── Checar saúde do banco de dados
├── Revisar taxas de erro de API
├── Checar comunicação entre serviços
└── Identificar componente em falha

DevOps Automator:
├── Revisar histórico de deployment recente
├── Checar status do pipeline CI/CD
├── Preparar rollback se necessário
└── Verificar estado da infraestrutura

Output: Causa raiz identificada (ou reduzida a um componente)
```

### Passo 3: Mitigação (15-60 minutos)

```
ÁRVORE DE DECISÃO:

IF causado por deployment recente:
  → DevOps Automator: Executar rollback
  → Infrastructure Maintainer: Verificar recuperação
  → Evidence Collector: Confirmar fix

IF causado por issue de infraestrutura:
  → Infrastructure Maintainer: Escalar/reiniciar/failover
  → DevOps Automator: Apoiar mudanças de infraestrutura
  → Verificar recuperação

IF causado por bug de código:
  → Relevant Developer Agent: Implementar hotfix
  → Evidence Collector: Verificar fix
  → DevOps Automator: Deploy hotfix
  → Infrastructure Maintainer: Monitorar recuperação

IF causado por dependência externa:
  → Infrastructure Maintainer: Ativar fallback/cache
  → Support Responder: Comunicar aos usuários
  → Monitorar recuperação externa

DURANTE TODO O PROCESSO:
  → Support Responder: Atualizar status page a cada 15 minutos
  → Executive Summary Generator: Briefar stakeholders (somente P0)
```

### Passo 4: Verificação de Resolução (Pós-fix)

```
Evidence Collector:
1. Verificar que o fix resolve a issue
2. Capturar evidência em screenshot do estado funcional
3. Confirmar que nenhuma nova issue foi introduzida

Infrastructure Maintainer:
1. Verificar que todas as métricas voltaram ao normal
2. Confirmar ausência de cascading failures
3. Monitorar por 30 minutos pós-fix

API Tester (se relacionado a API):
1. Rodar regressão nos endpoints afetados
2. Verificar que tempos de resposta normalizaram
3. Confirmar taxas de erro no baseline

Output: Confirmação de incidente resolvido
```

### Passo 5: Post-Mortem (Em até 48 horas)

```
Workflow Optimizer lidera o post-mortem:

1. Reconstrução da timeline
   - Quando a issue foi introduzida?
   - Quando foi detectada?
   - Quando foi resolvida?
   - Duração total do impacto em usuários

2. Análise de causa raiz
   - O que falhou?
   - Por que falhou?
   - Por que não foi capturado antes?
   - Análise dos 5 Whys

3. Avaliação de impacto
   - Usuários afetados
   - Impacto em receita
   - Impacto em reputação
   - Impacto em dados

4. Medidas de prevenção
   - Que monitoramento teria capturado isso antes?
   - Que teste teria prevenido isso?
   - Que mudanças de processo são necessárias?
   - Que mudanças de infraestrutura são necessárias?

5. Itens de ação
   - [Ação] → [Owner] → [Prazo]
   - [Ação] → [Owner] → [Prazo]
   - [Ação] → [Owner] → [Prazo]

Output: Relatório de Post-Mortem → Sprint Prioritizer adiciona tarefas de prevenção ao backlog
```

## Templates de Comunicação

### Update de Status Page (Support Responder)
```
[TIMESTAMP] — Incidente em [SERVICE NAME]

Status: [Investigating / Identified / Monitoring / Resolved]
Impacto: [Descrição do impacto no usuário]
Ação atual: [O que estamos fazendo sobre isso]
Próximo update: [Quando esperar o próximo update]
```

### Update Executivo (Executive Summary Generator — somente P0)
```
BRIEF DE INCIDENTE — [TIMESTAMP]

SITUAÇÃO: [Service] está [fora/degradado] afetando [N usuários/% do tráfego]
CAUSA: [Conhecida/Em investigação] — [Breve descrição se conhecida]
AÇÃO: [O que está sendo feito] — ETA [estimativa de tempo]
IMPACTO: [Impacto no negócio — receita, usuários, reputação]
PRÓXIMO UPDATE: [Timestamp]
```

## Matriz de Escalonamento

| Condição | Escalar Para | Ação |
|-----------|------------|--------|
| P0 não resolvido em 30 min | Studio Producer | Recursos adicionais, escalonamento com vendor |
| P1 não resolvido em 2 horas | Project Shepherd | Realocação de recursos |
| Suspeita de data breach | Legal Compliance Checker | Avaliação de notificação regulatória |
| Dados de usuários afetados | Legal Compliance Checker + Executive Summary Generator | Notificação GDPR/CCPA |
| Impacto em receita > $X | Finance Tracker + Studio Producer | Avaliação de impacto de negócio |
