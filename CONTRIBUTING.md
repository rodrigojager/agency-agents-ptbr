# 🤝 Contribuindo para The Agency

Antes de tudo, obrigado por considerar contribuir para The Agency! Pessoas como você tornam esta coleção de agentes de IA melhor para todo mundo.

## 📋 Sumário

- [Código de Conduta](#código-de-conduta)
- [Como Posso Contribuir?](#como-posso-contribuir)
- [Diretrizes de Design de Agentes](#diretrizes-de-design-de-agentes)
- [Processo de Pull Request](#processo-de-pull-request)
- [Guia de Estilo](#guia-de-estilo)
- [Comunidade](#comunidade)

---

## 📜 Código de Conduta

Este projeto e todas as pessoas que participam dele são regidos pelo nosso Código de Conduta. Ao participar, espera-se que você siga este código:

- **Seja respeitoso**: Trate todos com respeito. Debates saudáveis são incentivados, mas ataques pessoais não são tolerados.
- **Seja inclusivo**: Acolha e apoie pessoas de todas as origens e identidades.
- **Seja colaborativo**: O que criamos juntos é melhor do que o que criamos sozinhos.
- **Seja profissional**: Mantenha as discussões focadas em melhorar os agentes e a comunidade.

---

## 🎯 Como Posso Contribuir?

### 1. Crie um Novo Agente

Tem uma ideia para um agente especializado? Ótimo! Veja como adicionar um:

1. **Faça um fork do repositório**
2. **Escolha a categoria apropriada** (ou proponha uma nova):
   - `engineering/` - Especialistas em desenvolvimento de software
   - `design/` - Especialistas em UX/UI e criação
   - `finance/` - Especialistas em planejamento financeiro, contabilidade e investimentos
   - `game-development/` - Especialistas em design e desenvolvimento de games
   - `marketing/` - Especialistas em growth e marketing
   - `paid-media/` - Especialistas em mídia e aquisição paga
   - `product/` - Especialistas em gestão de produto
   - `project-management/` - Especialistas em PM e coordenação
   - `testing/` - Especialistas em QA e testes
   - `support/` - Especialistas em operações e suporte
   - `spatial-computing/` - Especialistas em AR/VR/XR
   - `specialized/` - Especialistas únicos que não se encaixam em outras categorias

3. **Crie seu arquivo de agente** seguindo o template abaixo
4. **Teste seu agente** em cenários reais
5. **Envie um Pull Request** com seu agente

### 2. Melhore Agentes Existentes

Encontrou uma forma de melhorar um agente? Contribuições são bem-vindas:

- Adicione exemplos e casos de uso do mundo real
- Aprimore exemplos de código com padrões modernos
- Atualize workflows com base em novas boas práticas
- Adicione métricas de sucesso e benchmarks
- Corrija typos, melhore a clareza e aprimore a documentação

### 3. Compartilhe Histórias de Sucesso

Usou estes agentes com sucesso? Compartilhe sua história:

- Publique em [GitHub Discussions](https://github.com/msitarzewski/agency-agents/discussions)
- Adicione um case study ao README
- Escreva um post de blog e coloque o link
- Crie um tutorial em vídeo

### 4. Reporte Issues

Encontrou um problema? Avise:

- Verifique se a issue já existe
- Forneça passos claros de reprodução
- Inclua contexto sobre seu caso de uso
- Sugira soluções possíveis, se tiver ideias

---

## 🎨 Diretrizes de Design de Agentes

### Estrutura do Arquivo de Agente

Todo agente deve seguir esta estrutura:

```markdown
---
name: Nome do Agente
description: Descrição em uma linha da especialidade e do foco do agente
color: nome-da-cor ou "#hexcode"
emoji: 🎯
vibe: Gancho de personalidade em uma linha - o que torna este agente memorável
services:                              # opcional - apenas se o agente exigir serviços externos
  - name: Nome do Serviço
    url: https://service-url.com
    tier: free                         # free, freemium ou paid
---

# Nome do Agente

## 🧠 Sua Identidade & Memória
- **Papel**: Descrição clara do papel
- **Personalidade**: Traços de personalidade e estilo de comunicação
- **Memória**: O que o agente lembra e aprende
- **Experiência**: Expertise e perspectiva no domínio

## 🎯 Sua Missão Principal
- Responsabilidade primária 1 com entregáveis claros
- Responsabilidade primária 2 com entregáveis claros
- Responsabilidade primária 3 com entregáveis claros
- **Requisito padrão**: Boas práticas sempre ativas

## 🚨 Regras Críticas que Você Deve Seguir
Regras e restrições específicas do domínio que definem a abordagem do agente

## 📋 Seus Entregáveis Técnicos
Exemplos concretos do que o agente produz:
- Exemplos de código
- Templates
- Frameworks
- Documentos

## 🔄 Seu Processo de Workflow
Processo passo a passo que o agente segue:
1. Fase 1: Descoberta e pesquisa
2. Fase 2: Planejamento e estratégia
3. Fase 3: Execução e implementação
4. Fase 4: Revisão e otimização

## 💭 Seu Estilo de Comunicação
- Como o agente se comunica
- Frases e padrões de exemplo
- Tom e abordagem

## 🔄 Aprendizado & Memória
Do que o agente aprende:
- Padrões bem-sucedidos
- Abordagens que falharam
- Feedback do usuário
- Evolução do domínio

## 🎯 Suas Métricas de Sucesso
Resultados mensuráveis:
- Métricas quantitativas (com números)
- Indicadores qualitativos
- Benchmarks de performance

## 🚀 Capacidades Avançadas
Técnicas e abordagens avançadas que o agente domina
```

### Estrutura do Agente

Arquivos de agentes são organizados em dois grupos semânticos que mapeiam para o formato de workspace do OpenClaw e ajudam outras ferramentas a interpretar seu agente:

#### Persona (quem o agente é)
- **Identidade & Memória** - papel, personalidade, background
- **Estilo de Comunicação** - tom, voz, abordagem
- **Regras Críticas** - limites e restrições

#### Operações (o que o agente faz)
- **Missão Principal** - responsabilidades primárias
- **Entregáveis Técnicos** - outputs concretos e templates
- **Processo de Workflow** - metodologia passo a passo
- **Métricas de Sucesso** - resultados mensuráveis
- **Capacidades Avançadas** - técnicas especializadas

Nenhuma formatação especial é exigida - apenas mantenha seções relacionadas à persona (identidade, comunicação, regras) agrupadas separadamente das seções operacionais (missão, entregáveis, workflow, métricas). O script `convert.sh` usa esses cabeçalhos de seção para dividir automaticamente agentes em formatos específicos de ferramentas.

### Princípios de Design de Agentes

1. **🎭 Personalidade Forte**
   - Dê ao agente uma voz e um caráter distintos
   - Não use "I am a helpful assistant" - seja específico e memorável
   - Exemplo: "I default to finding 3-5 issues and require visual proof" (Evidence Collector)

2. **📋 Entregáveis Claros**
   - Forneça exemplos concretos de código
   - Inclua templates e frameworks
   - Mostre outputs reais, não descrições vagas

3. **✅ Métricas de Sucesso**
   - Inclua métricas específicas e mensuráveis
   - Exemplo: "Page load times under 3 seconds on 3G"
   - Exemplo: "10,000+ combined karma across accounts"

4. **🔄 Workflows Comprovados**
   - Processos passo a passo
   - Abordagens testadas no mundo real
   - Nada teórico - precisa ser battle-tested

5. **💡 Memória de Aprendizado**
   - Quais padrões o agente reconhece
   - Como ele melhora com o tempo
   - O que ele lembra entre sessões

### Serviços Externos

Agentes podem depender de serviços externos (APIs, plataformas, ferramentas SaaS) quando esses serviços são essenciais para a função do agente. Quando dependerem:

1. **Declare as dependências** no frontmatter usando o campo `services`
2. **O agente deve se sustentar sozinho** - remova as chamadas de API e ainda deve existir uma persona, um workflow e uma expertise úteis por baixo
3. **Não duplique a documentação do vendor** - referencie, não reproduza. O arquivo do agente deve parecer um agente, não um guia de getting started
4. **Prefira serviços com tiers gratuitos** para que contribuidores consigam testar o agente

O teste: *este agente é para o usuário ou para o vendor?* Um agente que resolve o problema do usuário usando um serviço pertence aqui. Um guia de quickstart de um serviço vestido de agente, não.

### Compatibilidade Específica de Ferramentas

**Compatibilidade com Qwen Code**: Os corpos dos agentes suportam templates `${variable}` para contexto dinâmico (por exemplo, `${project_name}`, `${task_description}`). Qwen SubAgents usam frontmatter mínimo: apenas `name` e `description` são obrigatórios; os campos `color`, `emoji` e `version` são omitidos porque o Qwen não os utiliza.

### O que Faz um Ótimo Agente?

**Ótimos agentes têm**:
- ✅ Especialização estreita e profunda
- ✅ Personalidade e voz distintas
- ✅ Exemplos concretos de código/template
- ✅ Métricas de sucesso mensuráveis
- ✅ Workflows passo a passo
- ✅ Testes e iteração no mundo real

**Evite**:
- ❌ Personalidade genérica de "helpful assistant"
- ❌ Descrições vagas como "I will help you with..."
- ❌ Ausência de exemplos de código ou entregáveis
- ❌ Escopo amplo demais (jack of all trades)
- ❌ Abordagens teóricas não testadas

---

## 🔄 Processo de Pull Request

### O que Pertence em um PR (e o que Não Pertence)

O caminho mais rápido para um PR aceito é **um arquivo markdown** - um agente novo ou melhorado. Esse é o ponto ideal.

Para qualquer coisa além disso, veja como mantemos o processo fluido:

#### Sempre bem-vindo como PR
- Adicionar um novo agente (um arquivo `.md`)
- Melhorar conteúdo, exemplos ou personalidade de um agente existente
- Corrigir typos ou clarificar documentação

#### Comece com uma Discussion primeiro
- Novas ferramentas, sistemas de build ou workflows de CI
- Mudanças arquiteturais (novos diretórios, novos scripts, site generators)
- Mudanças que tocam muitos arquivos no repo
- Novos formatos ou plataformas de integração

Gostamos de ideias ambiciosas - uma [Discussion](https://github.com/msitarzewski/agency-agents/discussions) apenas dá à comunidade a chance de alinhar a abordagem antes de código ser escrito. Isso economiza tempo de todo mundo, especialmente o seu.

#### Coisas que sempre fecharemos
- **Output de build commitado**: Arquivos gerados (`_site/`, assets compilados, arquivos de agentes convertidos) nunca devem entrar no repo. Usuários executam `convert.sh` localmente; todo output fica no gitignore.
- **PRs que modificam agentes existentes em massa** sem uma discussion prévia - até uma reformatação bem-intencionada pode criar conflitos de merge para outros contribuidores.

### Antes de Enviar

1. **Teste Seu Agente**: Use-o em cenários reais e itere com base no feedback
2. **Siga o Template**: Mantenha a estrutura dos agentes existentes
3. **Adicione Exemplos**: Inclua pelo menos 2-3 exemplos de código/template
4. **Defina Métricas**: Inclua critérios de sucesso específicos e mensuráveis
5. **Revise**: Verifique typos, problemas de formatação e clareza

### Enviando Seu PR

1. **Faça um fork** do repositório
2. **Crie uma branch**: `git checkout -b add-agent-name`
3. **Faça suas mudanças**: Adicione seu(s) arquivo(s) de agente
4. **Commit**: `git commit -m "Add [Agent Name] specialist"`
5. **Push**: `git push origin add-agent-name`
6. **Abra um Pull Request** com:
   - Título claro: "Add [Agent Name] - [Category]"
   - Descrição do que o agente faz
   - Por que esse agente é necessário (caso de uso)
   - Qualquer teste que você tenha feito

### Processo de Revisão de PR

1. **Revisão da Comunidade**: Outros contribuidores podem fornecer feedback
2. **Iteração**: Responda ao feedback e faça melhorias
3. **Aprovação**: Mantenedores aprovarão quando estiver pronto
4. **Merge**: Sua contribuição passa a fazer parte de The Agency!

### Template de PR

```markdown
## Informações do Agente
**Nome do Agente**: [Nome]
**Categoria**: [engineering/design/marketing/etc.]
**Especialidade**: [Descrição em uma linha]

## Motivação
[Por que este agente é necessário? Que lacuna ele preenche?]

## Testes
[Como você testou este agente? Casos de uso do mundo real?]

## Checklist
- [ ] Segue a estrutura do template de agente
- [ ] Inclui personalidade e voz
- [ ] Tem exemplos concretos de código/template
- [ ] Define métricas de sucesso
- [ ] Inclui workflow passo a passo
- [ ] Revisado e formatado corretamente
- [ ] Testado em cenários reais
```

---

## 📐 Guia de Estilo

### Estilo de Escrita

- **Seja específico**: "Reduce page load by 60%" em vez de "Make it faster"
- **Seja concreto**: "Create React components with TypeScript" em vez de "Build UIs"
- **Seja memorável**: Dê personalidade aos agentes, não corporate speak genérico
- **Seja prático**: Inclua código real, não pseudo-code

### Formatação

- Use **formatação Markdown** de forma consistente
- Inclua **emojis** nos cabeçalhos de seção (facilita a leitura rápida)
- Use **blocos de código** para todos os exemplos de código, com syntax highlighting adequado
- Use **tabelas** para comparar opções ou mostrar métricas
- Use **negrito** para ênfase, `code` para termos técnicos

### Exemplos de Código

```markdown
## Example Code Block

\`\`\`typescript
// Always include:
// 1. Language specification for syntax highlighting
// 2. Comments explaining key concepts
// 3. Real, runnable code (not pseudo-code)
// 4. Modern best practices

interface AgentExample {
  name: string;
  specialty: string;
  deliverables: string[];
}
\`\`\`
```

### Tom

- **Profissional, mas acessível**: Nem formal demais, nem casual demais
- **Confiante, mas não arrogante**: "Here's the best approach" em vez de "Maybe you could try..."
- **Útil, mas sem tratar como iniciante**: Presuma competência e ofereça profundidade
- **Guiado por personalidade**: Cada agente deve ter uma voz única

---

## 🌟 Reconhecimento

Contribuidores que fizerem contribuições significativas serão:

- Listados na seção de agradecimentos do README
- Destacados nas release notes
- Apresentados nos showcases "Agent of the Week" (se aplicável)
- Creditados no próprio arquivo do agente

---

## 🤔 Perguntas?

- **Perguntas Gerais**: [GitHub Discussions](https://github.com/msitarzewski/agency-agents/discussions)
- **Bug Reports**: [GitHub Issues](https://github.com/msitarzewski/agency-agents/issues)
- **Feature Requests**: [GitHub Issues](https://github.com/msitarzewski/agency-agents/issues)
- **Chat da Comunidade**: [Participe das discussões](https://github.com/msitarzewski/agency-agents/discussions)

---

## 📚 Recursos

### Para Novos Contribuidores

- [README.md](README.md) - Visão geral e catálogo de agentes
- [Exemplo: Frontend Developer](engineering/engineering-frontend-developer.md) - Exemplo de agente bem estruturado
- [Exemplo: Reddit Community Builder](marketing/marketing-reddit-community-builder.md) - Ótimo exemplo de personalidade
- [Exemplo: Whimsy Injector](design/design-whimsy-injector.md) - Exemplo de especialista criativo

### Para Design de Agentes

- Leia agentes existentes para se inspirar
- Estude os padrões que funcionam bem
- Teste seus agentes em cenários reais
- Itere com base em feedback

---

## 🎉 Obrigado!

Suas contribuições tornam The Agency melhor para todo mundo. Seja você alguém que está:

- Adicionando um novo agente
- Melhorando a documentação
- Corrigindo bugs
- Compartilhando histórias de sucesso
- Ajudando outros contribuidores

**Você está fazendo a diferença. Obrigado!**

---

<div align="center">

**Perguntas? Ideias? Feedback?**

[Abra uma Issue](https://github.com/msitarzewski/agency-agents/issues) • [Inicie uma Discussion](https://github.com/msitarzewski/agency-agents/discussions) • [Envie um PR](https://github.com/msitarzewski/agency-agents/pulls)

Feito com ❤️ pela comunidade

</div>
