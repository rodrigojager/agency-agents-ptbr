# 🔍 Playbook Fase 0 — Inteligência & Discovery

> **Duração**: 3-7 dias | **Agentes**: 6 | **Gate Keeper**: Executive Summary Generator

---

## Objetivo

Validar a oportunidade antes de comprometer recursos. Nada de construir até que o problema, o mercado e o cenário regulatório estejam compreendidos.

## Pré-Condições

- [ ] Brief do projeto ou conceito inicial existe
- [ ] Sponsor stakeholder identificado
- [ ] Orçamento para a fase de discovery aprovado

## Sequência de Ativação dos Agentes

### Onda 1: Launch Paralelo (Dia 1)

#### 🔍 Trend Researcher — Lead de Inteligência de Mercado
```
Ative Trend Researcher para inteligência de mercado em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Análise do cenário competitivo (concorrentes diretos + indiretos)
2. Dimensionamento de mercado: TAM, SAM, SOM com metodologia
3. Mapeamento do ciclo de vida da tendência: onde este mercado está na curva de adoção?
4. Forecast de tendências para 3-6 meses com intervalos de confiança
5. Tendências de investimento e funding no espaço

Fontes: mínimo de 15 fontes únicas e verificadas
Formato: Relatório Estratégico com sumário executivo
Timeline: 3 dias
```

#### 💬 Feedback Synthesizer — Análise de Necessidades de Usuário
```
Ative Feedback Synthesizer para análise de necessidades de usuários em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Plano multicanal de coleta de feedback (surveys, entrevistas, reviews, social)
2. Análise de sentimento nos touchpoints existentes com usuários
3. Identificação e priorização de pain points (pontuados por RICE)
4. Análise de feature requests com estimativa de valor de negócio
5. Indicadores de risco de churn a partir de padrões de feedback

Formato: Relatório de Feedback Sintetizado com matriz de prioridade
Timeline: 3 dias
```

#### 🔍 UX Researcher — Análise de Comportamento do Usuário
```
Ative UX Researcher para análise de comportamento de usuários em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Plano de entrevistas com usuários (5-10 usuários-alvo)
2. Desenvolvimento de personas (3-5 personas primárias)
3. Mapeamento de jornada para fluxos principais de usuário
4. Avaliação heurística de usabilidade de produtos concorrentes
5. Insights comportamentais com validação estatística

Formato: Relatório de Findings de Pesquisa com personas e journey maps
Timeline: 5 dias
```

### Onda 2: Launch Paralelo (Dia 1, independente da Onda 1)

#### 📊 Analytics Reporter — Avaliação do Cenário de Dados
```
Ative Analytics Reporter para avaliação do cenário de dados em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Auditoria de fontes de dados existentes (quais dados estão disponíveis?)
2. Identificação de sinais (o que conseguimos medir?)
3. Estabelecimento de métricas baseline
4. Avaliação de qualidade de dados com pontuação de completude
5. Recomendações de infraestrutura de analytics

Formato: Relatório de Auditoria de Dados com mapa de sinais
Timeline: 2 dias
```

#### ⚖️ Legal Compliance Checker — Scan Regulatório
```
Ative Legal Compliance Checker para scan regulatório em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Frameworks regulatórios aplicáveis (GDPR, CCPA, HIPAA etc.)
2. Requisitos e restrições de tratamento de dados
3. Mapeamento de jurisdições para mercados-alvo
4. Avaliação de riscos de compliance com ratings de severidade
5. Issues de compliance bloqueantes vs. gerenciáveis

Formato: Matriz de Requisitos de Compliance
Timeline: 3 dias
```

#### 🛠️ Tool Evaluator — Cenário Tecnológico
```
Ative Tool Evaluator para avaliação do cenário tecnológico em [DOMÍNIO DO PROJETO].

Entregáveis obrigatórios:
1. Avaliação de stack tecnológica para o domínio do problema
2. Análise build vs. buy para componentes-chave
3. Viabilidade de integração com sistemas existentes
4. Avaliação open source vs. comercial
5. Avaliação de risco tecnológico

Formato: Avaliação de Tech Stack com matriz de recomendação
Timeline: 2 dias
```

## Ponto de Convergência (Dia 5-7)

Todos os seis agentes entregam seus relatórios. O Executive Summary Generator sintetiza:

```
Ative Executive Summary Generator para sintetizar os findings da Fase 0.

Documentos de entrada:
1. Trend Researcher → Market Analysis Report
2. Feedback Synthesizer → Synthesized Feedback Report
3. UX Researcher → Research Findings Report
4. Analytics Reporter → Data Audit Report
5. Legal Compliance Checker → Compliance Requirements Matrix
6. Tool Evaluator → Tech Stack Assessment

Output: Executive Summary (≤500 palavras, formato SCQA)
Decisão obrigatória: GO / NO-GO / PIVOT
Inclua: oportunidade de mercado quantificada, necessidades de usuário validadas, caminho regulatório, viabilidade tecnológica
```

## Checklist do Quality Gate

| # | Critério | Fonte de Evidência | Status |
|---|-----------|----------------|--------|
| 1 | Oportunidade de mercado validada com TAM > threshold mínimo viável | Relatório do Trend Researcher | ☐ |
| 2 | ≥3 pain points de usuário validados com dados de apoio | Feedback Synthesizer + UX Researcher | ☐ |
| 3 | Nenhuma issue bloqueante de compliance identificada | Matriz do Legal Compliance Checker | ☐ |
| 4 | Métricas-chave e fontes de dados identificadas | Auditoria do Analytics Reporter | ☐ |
| 5 | Stack tecnológica viável e avaliada | Avaliação do Tool Evaluator | ☐ |
| 6 | Sumário executivo entregue com recomendação GO/NO-GO | Executive Summary Generator | ☐ |

## Decisão de Gate

- **GO**: Prosseguir para Fase 1 — Estratégia & Arquitetura
- **NO-GO**: Arquivar findings, documentar aprendizados, redirecionar recursos
- **PIVOT**: Modificar escopo/direção com base nos findings, rodar discovery direcionado novamente

## Handoff para Fase 1

```markdown
## Pacote de Handoff Fase 0 → Fase 1

### Documentos a carregar adiante:
1. Market Analysis Report (Trend Researcher)
2. Synthesized Feedback Report (Feedback Synthesizer)
3. User Personas and Journey Maps (UX Researcher)
4. Data Audit Report (Analytics Reporter)
5. Compliance Requirements Matrix (Legal Compliance Checker)
6. Tech Stack Assessment (Tool Evaluator)
7. Executive Summary with GO decision (Executive Summary Generator)

### Restrições-chave identificadas:
- [Restrições regulatórias do Legal Compliance Checker]
- [Restrições técnicas do Tool Evaluator]
- [Restrições de timing de mercado do Trend Researcher]

### Necessidades prioritárias dos usuários (para Sprint Prioritizer):
1. [Pain point 1 — do Feedback Synthesizer]
2. [Pain point 2 — do UX Researcher]
3. [Pain point 3 — do Feedback Synthesizer]
```

---

*A Fase 0 está completa quando o Executive Summary Generator entrega uma decisão GO com evidências de apoio de todos os seis agentes de discovery.*
