# 🎭 The Agency (Fork pt-BR): Especialistas de IA para Transformar seu Workflow

> **Este repositório é um fork do projeto original [`msitarzewski/agency-agents`](https://github.com/msitarzewski/agency-agents), com foco principal em tradução manual dos agentes para português brasileiro (pt-BR).**

[![Fork base](https://img.shields.io/badge/fork-msitarzewski%2Fagency--agents-blue)](https://github.com/msitarzewski/agency-agents)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

---

## 📌 Objetivo deste fork

Este fork existe para:

- Traduzir os agentes para **pt-BR** com qualidade editorial e contexto técnico.
- Preservar termos em inglês quando já são naturais no Brasil (ex.: bug, commit, deploy, pull request, branch, merge, CEO).
- Manter compatibilidade estrutural dos arquivos (frontmatter YAML, blocos de código, templates, seções técnicas).

Além disso, este fork **pode seguir decisões diferentes do repositório original** ao longo do tempo, incluindo:

- Ajustes de linguagem e estilo para melhor aderência ao público brasileiro.
- Reorganizações de conteúdo para facilitar uso local.
- Inclusão de novos agentes que **não existem no original**, quando fizer sentido para o contexto deste fork.
- Agentes inspirados em outros repositórios, práticas de mercado e demandas reais de uso.

---

## ⚠️ Sobre diferenças entre fork e original

Embora a base venha do projeto original, este fork não é apenas um espelho. Em algum momento, ele pode:

1. Divergir na forma de documentar agentes.
2. Ter agentes adicionais e categorias novas.
3. Priorizar casos de uso específicos do ecossistema brasileiro.

Se você busca alinhamento total com o upstream, consulte também o repositório original.

---

## 🚀 Como usar

### 1) Instalação dos agentes

```bash
# instala para Claude Code (exemplo)
./scripts/install.sh --tool claude-code

# instalação interativa para ferramentas suportadas
./scripts/install.sh
```

### 2) Conversão para integrações

```bash
./scripts/convert.sh
```

### 3) Uso prático

Abra seu agente favorito e peça explicitamente o modo, por exemplo:

- “Ative o modo Frontend Developer e construa um componente React acessível.”
- “Ative o modo Code Reviewer e faça review com foco em segurança e performance.”

---

## 🧭 Estrutura do repositório

As principais divisões de agentes ficam em diretórios como:

- `academic/`
- `design/`
- `engineering/`
- `marketing/`
- `product/`
- `project-management/`
- `sales/`
- `testing/`
- `specialized/`

Cada arquivo `.md` descreve um agente com:

- Identidade e estilo de comunicação
- Missão central e regras críticas
- Entregáveis técnicos
- Workflow recomendado
- Métricas de sucesso

---

## 🌍 Política de tradução pt-BR deste fork

- Tradução **manual** e contextual (sem tradução automática em lote).
- Preservação de termos técnicos em inglês quando natural no mercado brasileiro.
- Manutenção da estrutura técnica dos arquivos para não quebrar compatibilidade.
- Evolução contínua com revisão semântica conforme novos agentes forem traduzidos.

O acompanhamento de progresso está em:

- `TRANSLATION_PROGRESS_pt-BR.md`

---

## 🤝 Contribuições

Contribuições são bem-vindas, especialmente para:

- Melhorias de tradução com foco semântico/contextual.
- Revisão técnica de agentes já traduzidos.
- Propostas de novos agentes relevantes para o público pt-BR.

Ao contribuir, siga o padrão deste fork: tradução manual, consistência de termos e preservação da estrutura técnica.

---

## 🙏 Créditos

- Projeto original: [`msitarzewski/agency-agents`](https://github.com/msitarzewski/agency-agents)
- Este fork: adaptação e evolução para pt-BR, com autonomia editorial e técnica.
