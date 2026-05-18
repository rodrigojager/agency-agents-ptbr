# 🛡️ Playbook Fase 4 — Qualidade & Hardening

> **Duração**: 3-7 dias | **Agentes**: 8 | **Gate Keeper**: Reality Checker (autoridade única)

---

## Objetivo

O desafio final de qualidade. O Reality Checker assume "NEEDS WORK" por padrão — você precisa provar prontidão para produção com evidência esmagadora. Esta fase existe porque primeiras implementações normalmente precisam de 2-3 ciclos de revisão, e isso é saudável.

## Pré-Condições

- [ ] Quality Gate da Fase 3 aprovado (todas as tarefas passaram por QA)
- [ ] Pacote de Handoff da Fase 3 recebido
- [ ] Todas as features implementadas e verificadas individualmente

## Mentalidade Crítica

> **O veredito padrão do Reality Checker é NEEDS WORK.**
> 
> Isso não é pessimismo — é realismo. Prontidão para produção exige:
> - Jornadas completas de usuário funcionando end-to-end
> - Consistência cross-device (desktop, tablet, mobile)
> - Performance sob carga (não apenas happy path)
> - Validação de segurança (não apenas "adicionamos auth")
> - Conformidade com a especificação (todo requisito, não a maioria)
>
> Uma nota B/B+ na primeira passada é normal e esperada.

## Sequência de Ativação dos Agentes

### Passo 1: Coleta de Evidências (Dia 1-2, Tudo em Paralelo)

#### 📸 Evidence Collector — Evidência Visual Abrangente
```
Ative Evidence Collector para evidência abrangente do sistema em [PROJETO].

Entregáveis obrigatórios:
1. Suite completa de screenshots:
   - Desktop (1920x1080) — toda página/view
   - Tablet (768x1024) — toda página/view
   - Mobile (375x667) — toda página/view
2. Evidência de interação:
   - Fluxos de navegação (antes/depois dos cliques)
   - Interações de formulário (vazio, preenchido, enviado, estados de erro)
   - Interações de modal/dialog
   - Accordion/conteúdo expansível
3. Evidência de tema:
   - Light mode — todas as páginas
   - Dark mode — todas as páginas
   - Detecção de preferência do sistema
4. Evidência de estados de erro:
   - Páginas 404
   - Erros de validação de formulário
   - Tratamento de erro de rede
   - Empty states

Formato: Pacote de Evidências em Screenshots com test-results.json
Timeline: 2 dias
```

#### 🔌 API Tester — Regressão Completa de API
```
Ative API Tester para regressão completa de API em [PROJETO].

Entregáveis obrigatórios:
1. Suite de regressão de endpoints:
   - Todos os endpoints testados (GET, POST, PUT, DELETE)
   - Verificação de autenticação/autorização
   - Testes de validação de input
   - Verificação de respostas de erro
2. Testes de integração:
   - Comunicação cross-service
   - Verificação de operações de banco de dados
   - Integração com APIs externas
3. Testes de edge cases:
   - Comportamento de rate limiting
   - Tratamento de payloads grandes
   - Tratamento de requests concorrentes
   - Tratamento de input malformado

Formato: Relatório de Testes de API com pass/fail por endpoint
Timeline: 2 dias
```

#### ⚡ Performance Benchmarker — Load Testing
```
Ative Performance Benchmarker para load testing em [PROJETO].

Entregáveis obrigatórios:
1. Load test com 10x o tráfego esperado:
   - Distribuição de tempo de resposta (P50, P95, P99)
   - Throughput sob carga
   - Taxa de erro sob carga
   - Utilização de recursos (CPU, memória, rede)
2. Medição de Core Web Vitals:
   - LCP (Largest Contentful Paint) < 2.5s
   - FID (First Input Delay) < 100ms
   - CLS (Cumulative Layout Shift) < 0.1
3. Performance de banco de dados:
   - Tempos de execução de queries
   - Utilização do connection pool
   - Efetividade dos índices
4. Resultados de stress test:
   - Identificação do ponto de quebra
   - Comportamento de graceful degradation
   - Tempo de recuperação após overload

Formato: Relatório de Certificação de Performance
Timeline: 2 dias
```

#### ⚖️ Legal Compliance Checker — Auditoria Final de Compliance
```
Ative Legal Compliance Checker para auditoria final de compliance em [PROJETO].

Entregáveis obrigatórios:
1. Verificação de privacy compliance:
   - Precisão da privacy policy
   - Funcionalidade de consent management
   - Implementação de direitos do titular de dados
   - Implementação de cookie consent
2. Compliance de segurança:
   - Criptografia de dados (em repouso e em trânsito)
   - Segurança de autenticação
   - Sanitização de input
   - Checagem OWASP Top 10
3. Compliance regulatório:
   - Requisitos GDPR (se aplicável)
   - Requisitos CCPA (se aplicável)
   - Requisitos específicos do setor
4. Compliance de acessibilidade:
   - Verificação WCAG 2.1 AA
   - Compatibilidade com screen reader
   - Navegação por teclado

Formato: Relatório de Certificação de Compliance
Timeline: 2 dias
```

### Passo 2: Análise (Dia 3-4, Paralelo, após o Passo 1)

#### 📊 Test Results Analyzer — Agregação de Métricas de Qualidade
```
Ative Test Results Analyzer para agregação de métricas de qualidade em [PROJETO].

Input: TODOS os relatórios do Passo 1
Entregáveis obrigatórios:
1. Dashboard agregado de qualidade:
   - Score geral de qualidade
   - Breakdown por categoria (visual, funcional, performance, segurança, compliance)
   - Distribuição de severidade de issues
   - Análise de tendência (se houver múltiplos ciclos de teste)
2. Priorização de issues:
   - Issues críticas (precisam corrigir antes de produção)
   - Issues altas (devem corrigir antes de produção)
   - Issues médias (corrigir no próximo sprint)
   - Issues baixas (backlog)
3. Avaliação de risco:
   - Probabilidade de prontidão para produção
   - Áreas de risco restantes
   - Mitigações recomendadas

Formato: Dashboard de Métricas de Qualidade
Timeline: 1 dia
```

#### 🔄 Workflow Optimizer — Review de Eficiência de Processo
```
Ative Workflow Optimizer para review de eficiência de processo em [PROJETO].

Input: dados de execução da Fase 3 + findings do Passo 1
Entregáveis obrigatórios:
1. Análise de eficiência do processo:
   - Eficiência do loop Dev↔QA (taxa de first-pass, média de retries)
   - Identificação de bottlenecks
   - Time-to-resolution para diferentes tipos de issue
2. Recomendações de melhoria:
   - Mudanças de processo para operações da Fase 6
   - Oportunidades de automação
   - Sugestões de melhoria de qualidade

Formato: Relatório de Recomendações de Otimização
Timeline: 1 dia
```

#### 🏗️ Infrastructure Maintainer — Checagem de Prontidão de Produção
```
Ative Infrastructure Maintainer para prontidão de produção em [PROJETO].

Entregáveis obrigatórios:
1. Validação do ambiente de produção:
   - Todos os serviços saudáveis e respondendo
   - Auto-scaling configurado e testado
   - Configuração de load balancer verificada
   - Certificados SSL/TLS válidos
2. Validação de monitoramento:
   - Todas as métricas críticas sendo coletadas
   - Regras de alerta configuradas e testadas
   - Acesso a dashboards verificado
   - Agregação de logs funcionando
3. Validação de disaster recovery:
   - Sistemas de backup operacionais
   - Procedimentos de recovery documentados e testados
   - Mecanismos de failover verificados
4. Validação de segurança:
   - Regras de firewall revisadas
   - Controles de acesso verificados
   - Gestão de secrets confirmada
   - Scan de vulnerabilidades limpo

Formato: Relatório de Prontidão de Infraestrutura
Timeline: 1 dia
```

### Passo 3: Julgamento Final (Dia 5-7, Sequencial)

#### 🔍 Reality Checker — O VEREDITO FINAL
```
Ative Reality Checker para testes finais de integração em [PROJETO].

PROCESSO OBRIGATÓRIO — NÃO PULAR:

Passo 1: Comandos de Reality Check
- Verificar o que foi realmente construído (ls, grep para features alegadas)
- Cruzar features alegadas com a especificação
- Rodar captura abrangente de screenshots
- Revisar todas as evidências do Passo 1 e Passo 2

Passo 2: Cross-Validation de QA
- Revisar findings do Evidence Collector
- Cruzar com resultados do API Tester
- Verificar dados do Performance Benchmarker
- Confirmar findings do Legal Compliance Checker

Passo 3: Validação End-to-End do Sistema
- Testar jornadas COMPLETAS de usuário (não features individuais)
- Verificar comportamento responsivo em TODOS os dispositivos
- Checar fluxos de interação end-to-end
- Revisar dados reais de performance

Passo 4: Reality Check da Especificação
- Citar texto EXATO da especificação original
- Comparar com evidência da implementação REAL
- Documentar TODO gap entre spec e realidade
- Sem suposições — apenas evidência

OPÇÕES DE VEREDITO:
- READY: Evidência esmagadora de prontidão para produção (raro na primeira passada)
- NEEDS WORK: Issues específicas identificadas com lista de correção (esperado)
- NOT READY: Grandes issues arquiteturais exigindo revisita à Fase 1/2

Formato: Relatório de Integração Baseado em Realidade
Default: NEEDS WORK a menos que o contrário seja provado
```

## Quality Gate — O GATE FINAL

| # | Critério | Threshold | Evidência Obrigatória |
|---|-----------|-----------|-------------------|
| 1 | Jornadas de usuário completas | Todos os caminhos críticos funcionando end-to-end | Screenshots do Reality Checker |
| 2 | Consistência cross-device | Desktop + Tablet + Mobile todos funcionando | Screenshots responsivos |
| 3 | Performance certificada | P95 < 200ms, LCP < 2.5s, uptime > 99.9% | Relatório do Performance Benchmarker |
| 4 | Segurança validada | Zero vulnerabilidades críticas | Security scan + relatório de compliance |
| 5 | Compliance certificado | Todos os requisitos regulatórios atendidos | Relatório do Legal Compliance Checker |
| 6 | Conformidade com especificação | 100% dos requisitos da spec implementados | Verificação ponto a ponto |
| 7 | Infraestrutura pronta | Ambiente de produção validado | Relatório do Infrastructure Maintainer |

## Decisão de Gate

**Autoridade única**: Reality Checker

### Se READY (prosseguir para Fase 5):
```markdown
## Pacote de Handoff Fase 4 → Fase 5

### Para Launch Team:
- Relatório de certificação do Reality Checker
- Certificação de performance
- Certificação de compliance
- Relatório de prontidão de infraestrutura
- Limitações conhecidas (se houver)

### Para Growth Hacker:
- Produto pronto para usuários
- Lista de features para marketing messaging
- Dados de performance para credibilidade

### Para DevOps Automator:
- Deployment em produção aprovado
- Plano de deployment blue-green
- Procedimentos de rollback confirmados
```

### Se NEEDS WORK (retornar à Fase 3):
```markdown
## Pacote de Retorno Fase 4 → Fase 3

### Lista de Correções (do Reality Checker):
1. [Issue Crítica 1]: [Descrição + evidência + instrução de correção]
2. [Issue Crítica 2]: [Descrição + evidência + instrução de correção]
3. [Issue Alta 1]: [Descrição + evidência + instrução de correção]
...

### Processo:
- Issues entram no loop Dev↔QA (mecânica da Fase 3)
- Cada fix deve passar pelo QA do Evidence Collector
- Quando todos os fixes concluírem → Retornar à Fase 4 Passo 3
- Reality Checker reavalia com evidência atualizada

### Esperado: 2-3 ciclos de revisão são normais
```

### Se NOT READY (retornar à Fase 1/2):
```markdown
## Pacote de Retorno Fase 4 → Fase 1/2

### Issues Arquiteturais Identificadas:
1. [Issue Fundamental]: [Por que não pode ser corrigida na Fase 3]
2. [Problema Estrutural]: [O que precisa mudar no nível de arquitetura]

### Ação Recomendada:
- [ ] Revisar arquitetura de sistema (Fase 1)
- [ ] Reconstruir fundação (Fase 2)
- [ ] Reduzir escopo e redefinir (Fase 1)

### Decisão do Studio Producer Obrigatória
```

---

*A Fase 4 está completa quando o Reality Checker emite um veredito READY com evidência esmagadora. NEEDS WORK é o resultado esperado na primeira passada — significa que o sistema funciona, mas precisa de polish.*
