# 🤝 Contribuindo para The Agency
Antes de tudo, muito obrigado por querer contribuir para The Agency! É com participantes como você que esta coleção de agentes de IA fica cada vez melhor.

## 📋 **Sumário**
- [Código de Conduta](#-código-de-conduta)
- [Como Posso Contribuir?](#-como-posso-contribuir)
- [Diretrizes de Design de Agentes](#-diretrizes-de-design-de-agentes)
- [Processo de Pull Request (PR)](#-processo-de-pull-request-pr)
- [Guia de Estilo](#-guia-de-estilo)
- [Comunidade](#-dúvidas)

---

## 📜 Código de Conduta
Este projeto e todas as pessoas participantes são regidos pelo Código de Conduta. Ao participar, você concorda em seguir estas diretrizes:

- **Mantenha o respeito**: Trate todas as pessoas com gentileza. Discussões racionais são incentivadas, mas ataques pessoais são proibidos.
- **Inclua a diversidade**: Acolha e apoie participantes de diferentes origens e identidades.
- **Colabore**: O resultado que criamos juntos é muito melhor do que o trabalho individual isolado.
- **Seja profissional**: Mantenha as conversas focadas em otimizar os agentes e fortalecer a comunidade.

---

## 🎯 Como Contribuir?

### 1. Crie um Agente Novo
Tem uma ideia para um agente específico? Excelente! Adicione seguindo estes passos:

1. Faça fork deste repositório
2. Escolha a categoria adequada (ou proponha uma nova categoria):
   - `engineering/` —— Especialistas em desenvolvimento de software
   - `design/` —— Especialistas em UX/UI e design criativo
   - `marketing/` —— Especialistas em growth e marketing
   - `product/` —— Especialistas em gestão de produto
   - `project-management/` —— Especialistas em gestão de projetos e coordenação
   - `testing/` —— Especialistas em QA e testes
   - `support/` —— Especialistas em operações e suporte
   - `spatial-computing/` —— Especialistas em AR/VR/XR
   - `specialized/` —— Especialistas únicos que não entram em outras categorias
3. Crie o arquivo do agente seguindo o template abaixo
4. Teste seu agente em cenários reais
5. Envie um Pull Request

### 2. Otimize Agentes Existentes
Encontrou uma forma de melhorar um agente existente? Contribuições são muito bem-vindas:
- Acrescente casos reais e cenários de uso
- Melhore exemplos de código usando padrões modernos
- Atualize workflows com base nas melhores práticas mais recentes
- Adicione métricas de sucesso e benchmarks
- Corrija erros de escrita, melhore a clareza e complete a documentação

### 3. Compartilhe Casos de Sucesso
Se você usou estes agentes com sucesso:
- Publique sua experiência em [GitHub Discussions](https://github.com/msitarzewski/agency-agents/discussions)
- Adicione um case study ao README
- Escreva um post de blog e inclua o link
- Crie um tutorial em vídeo

### 4. Reporte Problemas
Encontrou um problema? Conte para nós:
- Primeiro verifique se já existe uma issue igual
- Forneça passos claros para reprodução
- Explique seu cenário de uso e o contexto
- Se tiver ideias, proponha possíveis soluções

---

# 🎨 Diretrizes de Design de Agentes

### Estrutura do Arquivo de Agente
Cada agente deve seguir esta estrutura:

```yaml
---
name: Nome do Agente
description: Uma frase descrevendo a especialidade e o posicionamento do agente
color: Nome da cor ou "#valor-hexadecimal"
---
```

## Nome do Agente

### 🧠 Identidade e Memória
- **Papel**: Descrição clara do papel
- **Personalidade**: Traços de personalidade e estilo de comunicação
- **Memória**: O que o agente precisa lembrar e aprender
- **Experiência**: Competência de domínio e perspectiva

### 🎯 Missão Principal
- Responsabilidade principal 1, com entregável claro
- Responsabilidade principal 2, com entregável claro
- Responsabilidade principal 3, com entregável claro
- **Requisito padrão**: Seguir sempre as melhores práticas

### 🚨 Regras Críticas que Devem Ser Seguidas
Regras e restrições específicas do domínio que definem como o agente trabalha.

### 📋 Entregáveis Técnicos
Conteúdos concretos que o agente produz:
- Exemplos de código
- Templates
- Frameworks
- Documentos

### 🔄 Workflow
Processo passo a passo seguido pelo agente:
1. Fase 1: descoberta e pesquisa
2. Fase 2: planejamento e estratégia
3. Fase 3: execução e implementação
4. Fase 4: revisão e otimização

### 💭 Estilo de Comunicação
- Como o agente se comunica
- Frases e padrões de expressão de exemplo
- Tom e estilo

### 🔄 Aprendizado e Memória
O agente aprende continuamente a partir de:
- Padrões bem-sucedidos
- Casos que falharam
- Feedback do usuário
- Evolução do domínio

### 🎯 Métricas de Sucesso
Resultados mensuráveis:
- Métricas quantitativas (com valores específicos)
- Indicadores qualitativos
- Benchmarks de performance

### 🚀 Capacidades Avançadas
Técnicas e métodos avançados dominados pelo agente.

---

## Princípios de Design de Agentes
 1. 🎭 **Personalidade Marcante**
- Dê ao agente um tom e uma persona únicos
- Evite "sou um assistente útil"; seja específico e memorável
- Exemplo: "Por padrão, encontro 3-5 problemas e exijo evidência visual" (especialista em coleta de evidências)

 2. 📋 **Entregáveis Claros**
- Forneça exemplos de código aplicáveis
- Inclua templates e frameworks
- Mostre outputs reais, não descrições vagas

 3. ✅ **Métricas de Sucesso**
- Inclua métricas específicas e quantificáveis
- Exemplo: "Tempo de carregamento abaixo de 3 segundos em rede 3G"
- Exemplo: "10.000+ pontos de karma somados entre contas"

 4. 🔄 **Workflows Validados**
- Processo passo a passo claro
- Validado em cenários reais
- Nada de teoria pura ou solução só no papel

 5. 💡 **Memória de Aprendizado**
- Quais padrões o agente consegue reconhecer
- Como ele evolui e melhora com o tempo
- O que ele lembra entre sessões

### Critérios de um Excelente Agente
 - ✅ Posicionamento especializado e profundo
 - ✅ Personalidade e tom únicos
 - ✅ Exemplos concretos de código/template
 - ✅ Métricas de sucesso quantificáveis
 - ✅ Workflow passo a passo
 - ✅ Testes e iteração em cenários reais

**Evite:**
 - ❌ Persona genérica de "assistente útil"
 - ❌ Descrições vagas como "vou ajudar você..."
 - ❌ Ausência de exemplos de código e entregáveis
 - ❌ Escopo amplo demais
 - ❌ Soluções teóricas não testadas

---

## 🔄 Processo de Pull Request (PR)

### Antes de Enviar
- **Teste o agente**: Use em cenários reais e itere com base no feedback
- **Siga o template**: Mantenha consistência com a estrutura dos agentes existentes
- **Adicione exemplos**: Inclua pelo menos 2-3 exemplos de código/template
- **Defina métricas**: Inclua padrões de sucesso específicos e mensuráveis
- **Revise**: Verifique erros de escrita, formatação e clareza

### Enviando o PR
1. Faça fork do repositório
2. Crie uma branch:
   ```bash
   git checkout -b add-agent-name
   ```
3. Conclua as alterações: adicione o arquivo do agente
4. Faça commit:
   ```bash
   git commit -m "Add [Nome do Agente] specialist"
   ```
5. Faça push:
   ```bash
   git push origin add-agent-name
   ```
6. Abra um Pull Request contendo:
   - Título claro: `Add [Nome do Agente] - [Categoria]`
   - Descrição da função do agente
   - Por que este agente é necessário (cenário de uso)
   - Testes realizados

### Processo de Revisão de PR
- **Revisão da comunidade**: Outras pessoas contribuidoras podem fornecer feedback
- **Iteração e melhoria**: Ajuste conforme o feedback recebido
- **Aprovação**: Mantenedores aprovam quando tudo estiver correto
- **Merge**: Sua contribuição entra oficialmente em The Agency!

### Template de PR
```markdown
## Informações do Agente
**Nome do Agente**: [Nome]
**Categoria**: [engineering/design/marketing etc.]
**Especialidade**: Uma frase descritiva

## Motivação
[Por que este agente é necessário? Que lacuna ele cobre?]

## Testes
[Como você testou este agente? Quais cenários reais?]

## Checklist
- [ ] Segue a estrutura do template de agente
- [ ] Inclui personalidade e tom
- [ ] Tem exemplos concretos de código/template
- [ ] Define métricas de sucesso
- [ ] Inclui workflow passo a passo
- [ ] Foi revisado e formatado corretamente
- [ ] Foi testado em cenários reais
```

---

## 📐 Guia de Estilo

### Estilo de Escrita
- **Seja específico**: escreva "reduzir o tempo de carregamento da página em 60%" em vez de "deixar mais rápido"
- **Seja prático**: escreva "criar componentes React com TypeScript" em vez de "fazer interfaces"
- **Seja memorável**: dê personalidade ao agente, evitando linguagem corporativa genérica
- **Seja útil de verdade**: forneça código real, não pseudo-code

### Formatação
- Use Markdown de forma consistente
- Use emojis nos títulos de seção 🎯🧠📋 para facilitar a leitura rápida
- Use blocos de código com syntax highlighting para todos os exemplos
- Use tabelas para comparar opções ou exibir métricas
- Use **negrito** para ênfase e `` `código` `` para termos técnicos

### Exemplo de Código
```typescript
// Sempre inclua:
// 1. Indicação da linguagem para syntax highlighting
// 2. Comentários sobre a lógica principal
// 3. Código real executável (não pseudo-code)
// 4. Melhores práticas modernas

interface AgentExample {
  name: string;
  specialty: string;
  deliverables: string[];
}
```

### Tom
- Profissional e próximo: nem formal demais, nem casual demais
- Confiante sem arrogância: use "esta é a melhor solução" em vez de "talvez você possa tentar..."
- Útil sem conduzir cada passo: presuma capacidade básica do usuário e ofereça profundidade
- Personalidade clara: cada agente deve ter um tom próprio

---

## 🌟 Reconhecimento aos Contribuidores
Participantes que fizerem contribuições importantes receberão:
- Nome na área de agradecimentos do README
- Destaque nas release notes
- Inclusão na vitrine "Agente da Semana" (quando aplicável)
- Crédito no próprio arquivo do agente

---

## 🤔 Dúvidas?
- Perguntas gerais: [GitHub Discussions](https://github.com/msitarzewski/agency-agents/discussions)
- Bug reports: [GitHub Issues](https://github.com/msitarzewski/agency-agents/issues)
- Feature requests: [GitHub Issues](https://github.com/msitarzewski/agency-agents/issues)
- Comunidade: participe das [Discussions](https://github.com/msitarzewski/agency-agents/discussions)

---

## 📚 Recursos

### Guia para Novos Contribuidores
- [README.md](https://github.com/msitarzewski/agency-agents/blob/main/README.md) —— Visão geral do projeto e catálogo de agentes
- [Exemplo: Frontend Developer](https://github.com/msitarzewski/agency-agents/blob/main/engineering/engineering-frontend-developer.md ) —— Exemplo de agente com boa estrutura
- [Exemplo: Reddit Community Builder](https://github.com/msitarzewski/agency-agents/blob/main/marketing/marketing-reddit-community-builder.md) —— Ótimo exemplo de construção de personalidade
- [Exemplo: Whimsy Injector](https://github.com/msitarzewski/agency-agents/blob/main/design/design-whimsy-injector.md) —— Exemplo de especialista criativo

### Referência para Design de Agentes
- Leia agentes existentes para buscar inspiração
- Estude padrões que já foram validados
- Teste seus agentes em cenários reais
- Itere continuamente com base no feedback

---

## 🎉 Obrigado Novamente!
Cada contribuição sua torna The Agency melhor. Seja você alguém que:
- Adiciona um novo agente
- Melhora a documentação
- Corrige bugs
- Compartilha casos de sucesso
- Ajuda outras pessoas contribuidoras

Você está criando valor real. Obrigado!
