# 🎭 The Agency: Especialistas de IA Prontos para Transformar seu Workflow

> **Uma agência de IA completa ao seu alcance** - De magos de frontend a especialistas em comunidades Reddit, de injetores de personalidade a verificadores de realidade. Cada agente é um expert especializado com personalidade, processos e entregáveis comprovados.

[![GitHub stars](https://img.shields.io/github/stars/msitarzewski/agency-agents?style=social)](https://github.com/msitarzewski/agency-agents)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://makeapullrequest.com)
[![Sponsor](https://img.shields.io/badge/Sponsor-%E2%9D%A4-pink?logo=github)](https://github.com/sponsors/msitarzewski)

---

## 🚀 O que é isso?

Nascido de uma thread no Reddit e de meses de iteração, **The Agency** é uma coleção crescente de personalidades de agentes de IA meticulosamente criadas. Cada agente é:

- **🎯 Especializado**: Expertise profunda no seu domínio (não são templates de prompt genéricos)
- **🧠 Guiado por personalidade**: Voz, estilo de comunicação e abordagem únicos
- **📋 Focado em entregáveis**: Código real, processos e resultados mensuráveis
- **✅ Pronto para produção**: Workflows e métricas de sucesso battle-tested

**Pense nisso como**: montar seu dream team, só que eles são especialistas de IA que nunca dormem, nunca reclamam e sempre entregam.

---

## ⚡ Comece Rápido

### Opção 1: Use com Claude Code (Recomendado)

```bash
# Instale todos os agentes no seu diretório do Claude Code
./scripts/install.sh --tool claude-code

# Ou copie manualmente uma categoria se você quiser apenas uma divisão
cp engineering/*.md ~/.claude/agents/

# Então ative qualquer agente nas suas sessões do Claude Code:
# "Hey Claude, activate Frontend Developer mode and help me build a React component"
```

### Opção 2: Use como Referência

Cada arquivo de agente contém:
- Identidade e traços de personalidade
- Missão principal e workflows
- Entregáveis técnicos com exemplos de código
- Métricas de sucesso e estilo de comunicação

Explore os agentes abaixo e copie/adapte os que você precisar!

### Opção 3: Use com Outras Ferramentas (GitHub Copilot, Antigravity, Gemini CLI, OpenCode, OpenClaw, Cursor, Aider, Windsurf, Kimi Code)

```bash
# Passo 1 -- gere arquivos de integração para todas as ferramentas suportadas
./scripts/convert.sh

# Passo 2 -- instale interativamente (detecta automaticamente o que você tem instalado)
./scripts/install.sh

# Ou mire diretamente uma ferramenta específica
./scripts/install.sh --tool antigravity
./scripts/install.sh --tool gemini-cli
./scripts/install.sh --tool opencode
./scripts/install.sh --tool copilot
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool cursor
./scripts/install.sh --tool aider
./scripts/install.sh --tool windsurf
./scripts/install.sh --tool kimi
```

Veja a seção [Integrações Multi-Tool](#-integrações-multi-tool) abaixo para todos os detalhes.

---

## 🎨 O Roster da The Agency

### 💻 Divisão de Engenharia

Construindo o futuro, um commit por vez.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎨 [Frontend Developer](engineering/engineering-frontend-developer.md) | React/Vue/Angular, implementação de UI, performance | Apps web modernos, UIs pixel-perfect, otimização de Core Web Vitals |
| 🏗️ [Backend Architect](engineering/engineering-backend-architect.md) | Design de API, arquitetura de banco de dados, escalabilidade | Sistemas server-side, microsserviços, infraestrutura cloud |
| 📱 [Mobile App Builder](engineering/engineering-mobile-app-builder.md) | iOS/Android, React Native, Flutter | Aplicações mobile nativas e cross-platform |
| 🤖 [AI Engineer](engineering/engineering-ai-engineer.md) | Modelos de ML, deployment, integração de IA | Features de machine learning, data pipelines, apps com IA |
| 🚀 [DevOps Automator](engineering/engineering-devops-automator.md) | CI/CD, automação de infraestrutura, cloud ops | Desenvolvimento de pipelines, automação de deploy, monitoramento |
| ⚡ [Rapid Prototyper](engineering/engineering-rapid-prototyper.md) | Desenvolvimento rápido de POC, MVPs | Proofs of concept rápidos, projetos de hackathon, iteração veloz |
| 💎 [Senior Developer](engineering/engineering-senior-developer.md) | Laravel/Livewire, padrões avançados | Implementações complexas, decisões de arquitetura |
| 🔧 [Filament Optimization Specialist](engineering/engineering-filament-optimization-specialist.md) | UX de admin em Filament PHP, redesign estrutural de forms, otimização de resources | Reestruturar resources/forms/tables do Filament para workflows admin mais rápidos e limpos |
| 🔒 [Security Engineer](engineering/engineering-security-engineer.md) | Threat modeling, secure code review, arquitetura de segurança | Segurança de aplicação, avaliação de vulnerabilidades, security CI/CD |
| ⚡ [Autonomous Optimization Architect](engineering/engineering-autonomous-optimization-architect.md) | Roteamento de LLMs, otimização de custos, shadow testing | Sistemas autônomos que precisam de seleção inteligente de API e guardrails de custo |
| 🔩 [Embedded Firmware Engineer](engineering/engineering-embedded-firmware-engineer.md) | Bare-metal, RTOS, firmware ESP32/STM32/Nordic | Sistemas embarcados e dispositivos IoT production-grade |
| 🚨 [Incident Response Commander](engineering/engineering-incident-response-commander.md) | Gestão de incidentes, post-mortems, on-call | Gerenciar incidentes de produção e criar prontidão para incidentes |
| ⛓️ [Solidity Smart Contract Engineer](engineering/engineering-solidity-smart-contract-engineer.md) | Contratos EVM, otimização de gas, DeFi | Smart contracts seguros e otimizados para gas e protocolos DeFi |
| 🧭 [Codebase Onboarding Engineer](engineering/engineering-codebase-onboarding-engineer.md) | Onboarding rápido de developers, exploração read-only de codebase, explicação factual | Ajudar novos developers a entender repos desconhecidos rapidamente lendo código, rastreando code paths e declarando fatos sobre estrutura e comportamento |
| 📚 [Technical Writer](engineering/engineering-technical-writer.md) | Documentação para developers, referência de API, tutoriais | Documentação técnica clara e precisa |
| 🎯 [Threat Detection Engineer](engineering/engineering-threat-detection-engineer.md) | Regras SIEM, threat hunting, mapeamento ATT&CK | Construir camadas de detecção e threat hunting |
| 💬 [WeChat Mini Program Developer](engineering/engineering-wechat-mini-program-developer.md) | Ecossistema WeChat, Mini Programs, integração de pagamentos | Criar apps performáticos para o ecossistema WeChat |
| 👁️ [Code Reviewer](engineering/engineering-code-reviewer.md) | Code review construtivo, segurança, manutenibilidade | Reviews de PR, quality gates de código, mentoria por review |
| 🗄️ [Database Optimizer](engineering/engineering-database-optimizer.md) | Design de schema, otimização de queries, estratégias de indexação | Tuning PostgreSQL/MySQL, debug de queries lentas, planejamento de migração |
| 🌿 [Git Workflow Master](engineering/engineering-git-workflow-master.md) | Estratégias de branch, conventional commits, Git avançado | Design de workflow Git, limpeza de histórico, gestão de branches amigável a CI |
| 🏛️ [Software Architect](engineering/engineering-software-architect.md) | System design, DDD, padrões arquiteturais, análise de trade-offs | Decisões de arquitetura, modelagem de domínio, estratégia de evolução de sistemas |
| 🛡️ [SRE](engineering/engineering-sre.md) | SLOs, error budgets, observabilidade, chaos engineering | Confiabilidade de produção, redução de toil, planejamento de capacidade |
| 🧬 [AI Data Remediation Engineer](engineering/engineering-ai-data-remediation-engineer.md) | Pipelines self-healing, SLMs air-gapped, clusterização semântica | Corrigir dados quebrados em escala com zero perda de dados |
| 🔧 [Data Engineer](engineering/engineering-data-engineer.md) | Data pipelines, arquitetura lakehouse, ETL/ELT | Construir infraestrutura de dados e warehousing confiáveis |
| 🔗 [Feishu Integration Developer](engineering/engineering-feishu-integration-developer.md) | Feishu/Lark Open Platform, bots, workflows | Criar integrações para o ecossistema Feishu |
| 🧱 [CMS Developer](engineering/engineering-cms-developer.md) | Temas WordPress & Drupal, plugins/modules, arquitetura de conteúdo | Implementação e customização de CMS code-first |
| 📧 [Email Intelligence Engineer](engineering/engineering-email-intelligence-engineer.md) | Parsing de e-mail, extração MIME, dados estruturados para agentes de IA | Transformar threads brutas de e-mail em contexto pronto para raciocínio |
| 🎙️ [Voice AI Integration Engineer](engineering/engineering-voice-ai-integration-engineer.md) | Pipelines speech-to-text, Whisper, ASR, speaker diarization | Pipelines de transcrição end-to-end, pré-processamento de áudio, entrega de transcrições estruturadas |

### 🎨 Divisão de Design

Tornando tudo bonito, usável e encantador.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [UI Designer](design/design-ui-designer.md) | Design visual, bibliotecas de componentes, design systems | Criação de interfaces, consistência de marca, design de componentes |
| 🔍 [UX Researcher](design/design-ux-researcher.md) | Testes com usuários, análise de comportamento, pesquisa | Entender usuários, testes de usabilidade, insights de design |
| 🏛️ [UX Architect](design/design-ux-architect.md) | Arquitetura técnica, sistemas CSS, implementação | Fundações amigáveis a developers, orientação de implementação |
| 🎭 [Brand Guardian](design/design-brand-guardian.md) | Identidade de marca, consistência, posicionamento | Estratégia de marca, desenvolvimento de identidade, guidelines |
| 📖 [Visual Storyteller](design/design-visual-storyteller.md) | Narrativas visuais, conteúdo multimídia | Histórias visuais envolventes, storytelling de marca |
| ✨ [Whimsy Injector](design/design-whimsy-injector.md) | Personalidade, encanto, interações lúdicas | Adicionar alegria, microinterações, Easter eggs, personalidade de marca |
| 📷 [Image Prompt Engineer](design/design-image-prompt-engineer.md) | Prompts de geração de imagem por IA, fotografia | Prompts fotográficos para Midjourney, DALL-E, Stable Diffusion |
| 🌈 [Inclusive Visuals Specialist](design/design-inclusive-visuals-specialist.md) | Representação, mitigação de viés, imagens autênticas | Gerar imagens e vídeos de IA culturalmente precisos |

### 💰 Divisão de Paid Media

Transformando investimento em mídia em resultados de negócio mensuráveis.

| Agente | Especialidade | Quando Usar |
| --- | --- | --- |
| 💰 [PPC Campaign Strategist](paid-media/paid-media-ppc-strategist.md) | Google/Microsoft/Amazon Ads, arquitetura de conta, bidding | Buildouts de conta, alocação de orçamento, escala, diagnóstico de performance |
| 🔍 [Search Query Analyst](paid-media/paid-media-search-query-analyst.md) | Análise de termos de busca, negative keywords, mapeamento de intenção | Auditorias de queries, eliminação de gasto desperdiçado, descoberta de keywords |
| 📋 [Paid Media Auditor](paid-media/paid-media-auditor.md) | Auditorias de conta com 200+ pontos, análise competitiva | Assumir contas, revisões trimestrais, pitches competitivos |
| 📡 [Tracking & Measurement Specialist](paid-media/paid-media-tracking-specialist.md) | GTM, GA4, conversion tracking, CAPI | Novas implementações, auditorias de tracking, migrações de plataforma |
| ✍️ [Ad Creative Strategist](paid-media/paid-media-creative-strategist.md) | Copy RSA, criativos Meta, assets Performance Max | Launches criativos, programas de teste, refresh por fadiga de anúncios |
| 📺 [Programmatic & Display Buyer](paid-media/paid-media-programmatic-buyer.md) | GDN, DSPs, mídia com parceiros, ABM display | Planejamento de display, outreach com parceiros, programas ABM |
| 📱 [Paid Social Strategist](paid-media/paid-media-paid-social-strategist.md) | Meta, LinkedIn, TikTok, social cross-platform | Programas de anúncios sociais, seleção de plataformas, estratégia de audiência |

### 💼 Divisão de Sales

Transformando pipeline em receita por técnica, não por busywork de CRM.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Outbound Strategist](sales/sales-outbound-strategist.md) | Prospecção baseada em sinais, sequências multicanal, targeting de ICP | Construir pipeline com outreach guiado por pesquisa, não por volume |
| 🔍 [Discovery Coach](sales/sales-discovery-coach.md) | SPIN, Gap Selling, Sandler — design de perguntas e estrutura de call | Preparar discovery calls, qualificar oportunidades, treinar reps |
| ♟️ [Deal Strategist](sales/sales-deal-strategist.md) | Qualificação MEDDPICC, posicionamento competitivo, win planning | Pontuar deals, expor risco de pipeline, criar estratégias de vitória |
| 🛠️ [Sales Engineer](sales/sales-engineer.md) | Demos técnicas, escopo de POC, battlecards competitivos | Vitórias técnicas de pré-vendas, preparação de demo, posicionamento competitivo |
| 🏹 [Proposal Strategist](sales/sales-proposal-strategist.md) | Resposta a RFP, win themes, estrutura narrativa | Escrever propostas que persuadem, não apenas cumprem requisitos |
| 📊 [Pipeline Analyst](sales/sales-pipeline-analyst.md) | Forecasting, saúde de pipeline, velocidade de deals, RevOps | Revisões de pipeline, acurácia de forecast, operações de receita |
| 🗺️ [Account Strategist](sales/sales-account-strategist.md) | Land-and-expand, QBRs, mapeamento de stakeholders | Expansão pós-venda, planejamento de contas, crescimento de NRR |
| 🏋️ [Sales Coach](sales/sales-coach.md) | Desenvolvimento de reps, coaching de calls, facilitação de pipeline review | Melhorar cada rep e cada deal por coaching estruturado |
| 🎯 [Sales Outreach](specialized/sales-outreach.md) | Prospecção fria, cadências multi-touch, tratamento de objeções, propostas | Outreach B2B top-of-funnel - de cold email a discovery call marcada |

### 📢 Divisão de Marketing

Crescendo sua audiência, uma interação autêntica por vez.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🚀 [Growth Hacker](marketing/marketing-growth-hacker.md) | Aquisição rápida de usuários, viral loops, experimentos | Crescimento explosivo, aquisição de usuários, otimização de conversão |
| 📝 [Content Creator](marketing/marketing-content-creator.md) | Conteúdo multiplataforma, calendários editoriais | Estratégia de conteúdo, copywriting, storytelling de marca |
| 🐦 [Twitter Engager](marketing/marketing-twitter-engager.md) | Engajamento em tempo real, thought leadership | Estratégia de Twitter, campanhas no LinkedIn, social profissional |
| 📱 [TikTok Strategist](marketing/marketing-tiktok-strategist.md) | Conteúdo viral, otimização de algoritmo | Crescimento no TikTok, conteúdo viral, audiência Gen Z/Millennial |
| 📸 [Instagram Curator](marketing/marketing-instagram-curator.md) | Storytelling visual, construção de comunidade | Estratégia de Instagram, desenvolvimento estético, conteúdo visual |
| 🤝 [Reddit Community Builder](marketing/marketing-reddit-community-builder.md) | Engajamento autêntico, conteúdo orientado a valor | Estratégia Reddit, confiança da comunidade, marketing autêntico |
| 📱 [App Store Optimizer](marketing/marketing-app-store-optimizer.md) | ASO, otimização de conversão, discoverability | Marketing de app, otimização de loja, crescimento de app |
| 🌐 [Social Media Strategist](marketing/marketing-social-media-strategist.md) | Estratégia cross-platform, campanhas | Estratégia social geral, campanhas multiplataforma |
| 📕 [Xiaohongshu Specialist](marketing/marketing-xiaohongshu-specialist.md) | Conteúdo lifestyle, estratégia orientada por tendências | Crescimento no Xiaohongshu, storytelling estético, audiência Gen Z |
| 💬 [WeChat Official Account Manager](marketing/marketing-wechat-official-account.md) | Engajamento de subscribers, content marketing | Estratégia de WeChat OA, construção de comunidade, otimização de conversão |
| 🧠 [Zhihu Strategist](marketing/marketing-zhihu-strategist.md) | Thought leadership, engajamento guiado por conhecimento | Construção de autoridade no Zhihu, estratégia de Q&A, geração de leads |
| 🇨🇳 [Baidu SEO Specialist](marketing/marketing-baidu-seo-specialist.md) | Otimização Baidu, China SEO, conformidade ICP | Rankear no Baidu e alcançar o mercado de busca chinês |
| 🎬 [Bilibili Content Strategist](marketing/marketing-bilibili-content-strategist.md) | Algoritmo B站, cultura danmaku, crescimento de UP主 | Construir audiências no Bilibili com conteúdo community-first |
| 🎠 [Carousel Growth Engine](marketing/marketing-carousel-growth-engine.md) | Carrosséis TikTok/Instagram, publicação autônoma | Gerar e publicar conteúdo de carrossel viral |
| 💼 [LinkedIn Content Creator](marketing/marketing-linkedin-content-creator.md) | Personal branding, thought leadership, conteúdo profissional | Crescimento no LinkedIn, construção de audiência profissional, conteúdo B2B |
| 🛒 [China E-Commerce Operator](marketing/marketing-china-ecommerce-operator.md) | Taobao, Tmall, Pinduoduo, live commerce | Operar e-commerce multiplataforma na China |
| 🎥 [Kuaishou Strategist](marketing/marketing-kuaishou-strategist.md) | Kuaishou, comunidade 老铁, crescimento grassroots | Construir audiências autênticas em mercados lower-tier |
| 🔍 [SEO Specialist](marketing/marketing-seo-specialist.md) | SEO técnico, estratégia de conteúdo, link building | Impulsionar crescimento orgânico sustentável |
| 📘 [Book Co-Author](marketing/marketing-book-co-author.md) | Livros de thought leadership, ghostwriting, publishing | Colaboração estratégica em livros para founders e experts |
| 🌏 [Cross-Border E-Commerce Specialist](marketing/marketing-cross-border-ecommerce.md) | Amazon, Shopee, Lazada, fulfillment cross-border | Estratégia full-funnel de e-commerce cross-border |
| 🎵 [Douyin Strategist](marketing/marketing-douyin-strategist.md) | Plataforma Douyin, marketing de short-video, algoritmo | Crescer audiências na principal plataforma chinesa de short-video |
| 🎙️ [Livestream Commerce Coach](marketing/marketing-livestream-commerce-coach.md) | Treinamento de hosts, otimização de live room, conversão | Construir operações de livestream e-commerce de alta performance |
| 🎧 [Podcast Strategist](marketing/marketing-podcast-strategist.md) | Estratégia de conteúdo para podcast, otimização de plataforma | Estratégia e operações para o mercado chinês de podcasts |
| 🔒 [Private Domain Operator](marketing/marketing-private-domain-operator.md) | WeCom, private traffic, operações de comunidade | Construir ecossistemas de private domain no WeChat corporativo |
| 🎬 [Short-Video Editing Coach](marketing/marketing-short-video-editing-coach.md) | Pós-produção, workflows de edição, specs de plataforma | Treinamento prático e otimização de edição de short-video |
| 🔥 [Weibo Strategist](marketing/marketing-weibo-strategist.md) | Sina Weibo, trending topics, engajamento de fãs | Operação e crescimento full-spectrum no Weibo |
| 🔮 [AI Citation Strategist](marketing/marketing-ai-citation-strategist.md) | AEO/GEO, visibilidade em recomendações de IA, auditoria de citações | Melhorar visibilidade de marca em ChatGPT, Claude, Gemini, Perplexity |
| 🇨🇳 [China Market Localization Strategist](marketing/marketing-china-market-localization-strategist.md) | Localização full-stack para mercado chinês, Douyin/Xiaohongshu/WeChat GTM | Transformar sinais de tendência em estratégias go-to-market executáveis na China |
| 🎬 [Video Optimization Specialist](marketing/marketing-video-optimization-specialist.md) | Estratégia de algoritmo do YouTube, chaptering, conceitos de thumbnail | Crescimento de canal no YouTube, video SEO, otimização de retenção de audiência |

### 📊 Divisão de Produto

Construindo a coisa certa na hora certa.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Sprint Prioritizer](product/product-sprint-prioritizer.md) | Planejamento Agile, priorização de features | Sprint planning, alocação de recursos, gestão de backlog |
| 🔍 [Trend Researcher](product/product-trend-researcher.md) | Inteligência de mercado, análise competitiva | Pesquisa de mercado, avaliação de oportunidades, identificação de tendências |
| 💬 [Feedback Synthesizer](product/product-feedback-synthesizer.md) | Análise de feedback de usuários, extração de insights | Análise de feedback, insights de usuários, prioridades de produto |
| 🧠 [Behavioral Nudge Engine](product/product-behavioral-nudge-engine.md) | Psicologia comportamental, design de nudges, engajamento | Maximizar motivação do usuário com ciência comportamental |
| 🧭 [Product Manager](product/product-manager.md) | Ownership completo do ciclo de vida do produto | Discovery, PRDs, planejamento de roadmap, GTM, medição de resultados |

### 🎬 Divisão de Project Management

Mantendo os trens no horário (e dentro do orçamento).

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎬 [Studio Producer](project-management/project-management-studio-producer.md) | Orquestração de alto nível, gestão de portfólio | Supervisão multiprojeto, alinhamento estratégico, alocação de recursos |
| 🐑 [Project Shepherd](project-management/project-management-project-shepherd.md) | Coordenação cross-functional, gestão de timeline | Coordenação end-to-end de projetos, gestão de stakeholders |
| ⚙️ [Studio Operations](project-management/project-management-studio-operations.md) | Eficiência do dia a dia, otimização de processos | Excelência operacional, suporte ao time, produtividade |
| 🧪 [Experiment Tracker](project-management/project-management-experiment-tracker.md) | Testes A/B, validação de hipóteses | Gestão de experimentos, decisões data-driven, testes |
| 👔 [Senior Project Manager](project-management/project-manager-senior.md) | Scoping realista, conversão em tarefas | Converter specs em tarefas, gestão de escopo |
| 📋 [Jira Workflow Steward](project-management/project-management-jira-workflow-steward.md) | Workflow Git, estratégia de branch, rastreabilidade | Reforçar disciplina de Git vinculada ao Jira e entrega |

### 🧪 Divisão de Testing

Quebrando coisas para que os usuários não precisem quebrar.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📸 [Evidence Collector](testing/testing-evidence-collector.md) | QA baseado em screenshots, prova visual | Testes de UI, verificação visual, documentação de bugs |
| 🔍 [Reality Checker](testing/testing-reality-checker.md) | Certificação baseada em evidências, quality gates | Prontidão de produção, aprovação de qualidade, certificação de release |
| 📊 [Test Results Analyzer](testing/testing-test-results-analyzer.md) | Avaliação de testes, análise de métricas | Análise de output de testes, insights de qualidade, relatório de cobertura |
| ⚡ [Performance Benchmarker](testing/testing-performance-benchmarker.md) | Testes de performance, otimização | Testes de velocidade, load testing, tuning de performance |
| 🔌 [API Tester](testing/testing-api-tester.md) | Validação de API, testes de integração | Testes de API, verificação de endpoints, QA de integração |
| 🛠️ [Tool Evaluator](testing/testing-tool-evaluator.md) | Avaliação de tecnologia, seleção de ferramentas | Avaliar tools, recomendações de software, decisões técnicas |
| 🔄 [Workflow Optimizer](testing/testing-workflow-optimizer.md) | Análise de processos, melhoria de workflow | Otimização de processos, ganhos de eficiência, oportunidades de automação |
| ♿ [Accessibility Auditor](testing/testing-accessibility-auditor.md) | Auditoria WCAG, testes com tecnologia assistiva | Conformidade de acessibilidade, testes com screen reader, verificação de design inclusivo |

### 🛟 Divisão de Support

A espinha dorsal da operação.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 💬 [Support Responder](support/support-support-responder.md) | Atendimento ao cliente, resolução de issues | Suporte ao cliente, experiência do usuário, operações de suporte |
| 📊 [Analytics Reporter](support/support-analytics-reporter.md) | Análise de dados, dashboards, insights | Business intelligence, acompanhamento de KPIs, visualização de dados |
| 💰 [Finance Tracker](support/support-finance-tracker.md) | Planejamento financeiro, gestão de orçamento | Análise financeira, cash flow, performance de negócio |
| 🏗️ [Infrastructure Maintainer](support/support-infrastructure-maintainer.md) | Confiabilidade de sistemas, otimização de performance | Gestão de infraestrutura, operações de sistemas, monitoramento |
| ⚖️ [Legal Compliance Checker](support/support-legal-compliance-checker.md) | Compliance, regulamentações, revisão legal | Conformidade legal, requisitos regulatórios, gestão de risco |
| 📑 [Executive Summary Generator](support/support-executive-summary-generator.md) | Comunicação com C-suite, resumos estratégicos | Relatórios executivos, comunicação estratégica, suporte à decisão |

### 🥽 Divisão de Spatial Computing

Construindo o futuro imersivo.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🏗️ [XR Interface Architect](spatial-computing/xr-interface-architect.md) | Design de interação espacial, UX imersiva | Design de interfaces AR/VR/XR, UX de spatial computing |
| 💻 [macOS Spatial/Metal Engineer](spatial-computing/macos-spatial-metal-engineer.md) | Swift, Metal, 3D de alta performance | Spatial computing em macOS, apps nativos para Vision Pro |
| 🌐 [XR Immersive Developer](spatial-computing/xr-immersive-developer.md) | WebXR, AR/VR baseada em navegador | Experiências imersivas baseadas em browser, apps WebXR |
| 🎮 [XR Cockpit Interaction Specialist](spatial-computing/xr-cockpit-interaction-specialist.md) | Controles baseados em cockpit, sistemas imersivos | Sistemas de controle em cockpit, interfaces de controle imersivas |
| 🍎 [visionOS Spatial Engineer](spatial-computing/visionos-spatial-engineer.md) | Desenvolvimento Apple Vision Pro | Apps para Vision Pro, experiências de spatial computing |
| 🔌 [Terminal Integration Specialist](spatial-computing/terminal-integration-specialist.md) | Integração com terminal, ferramentas command-line | CLI tools, workflows de terminal, developer tools |

### 🎯 Divisão Specialized

Os especialistas únicos que não cabem em uma caixa.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎭 [Agents Orchestrator](specialized/agents-orchestrator.md) | Coordenação multiagente, gestão de workflow | Projetos complexos que exigem coordenação de múltiplos agentes |
| 🔍 [LSP/Index Engineer](specialized/lsp-index-engineer.md) | Language Server Protocol, inteligência de código | Sistemas de inteligência de código, implementação de LSP, indexação semântica |
| 📥 [Sales Data Extraction Agent](specialized/sales-data-extraction-agent.md) | Monitoramento de Excel, extração de métricas de sales | Ingestão de dados de sales, métricas MTD/YTD/Year End |
| 📈 [Data Consolidation Agent](specialized/data-consolidation-agent.md) | Agregação de dados de sales, relatórios de dashboard | Resumos por território, performance de reps, snapshots de pipeline |
| 📬 [Report Distribution Agent](specialized/report-distribution-agent.md) | Entrega automatizada de relatórios | Distribuição de relatórios por território, envios agendados |
| 🔐 [Agentic Identity & Trust Architect](specialized/agentic-identity-trust.md) | Identidade de agentes, autenticação, verificação de confiança | Sistemas de identidade multiagente, autorização de agentes, trilhas de auditoria |
| 🔗 [Identity Graph Operator](specialized/identity-graph-operator.md) | Resolução de identidade compartilhada para sistemas multiagente | Deduplicação de entidades, propostas de merge, consistência de identidade cross-agent |
| 💸 [Accounts Payable Agent](specialized/accounts-payable-agent.md) | Processamento de pagamentos, gestão de vendors, auditoria | Execução autônoma de pagamentos em crypto, fiat, stablecoins |
| 🛡️ [Blockchain Security Auditor](specialized/blockchain-security-auditor.md) | Auditorias de smart contracts, análise de exploits | Encontrar vulnerabilidades em contratos antes do deployment |
| 📋 [Compliance Auditor](specialized/compliance-auditor.md) | SOC 2, ISO 27001, HIPAA, PCI-DSS | Guiar organizações por certificações de compliance |
| 🌍 [Cultural Intelligence Strategist](specialized/specialized-cultural-intelligence-strategist.md) | UX global, representação, exclusão cultural | Garantir que software ressoe entre culturas |
| 🗣️ [Developer Advocate](specialized/specialized-developer-advocate.md) | Construção de comunidade, DX, conteúdo developer | Conectar produto e comunidade developer |
| 🔬 [Model QA Specialist](specialized/specialized-model-qa.md) | Auditorias de ML, análise de features, interpretabilidade | QA end-to-end para modelos de machine learning |
| 🗃️ [ZK Steward](specialized/zk-steward.md) | Gestão de conhecimento, Zettelkasten, notas | Construir bases de conhecimento conectadas e validadas |
| 🔌 [MCP Builder](specialized/specialized-mcp-builder.md) | Servidores Model Context Protocol, tooling para agentes de IA | Construir servidores MCP que ampliam capacidades de agentes de IA |
| 📄 [Document Generator](specialized/specialized-document-generator.md) | Geração de PDF, PPTX, DOCX, XLSX a partir de código | Criação profissional de documentos, relatórios, visualização de dados |
| ⚙️ [Automation Governance Architect](specialized/automation-governance-architect.md) | Governança de automação, n8n, auditoria de workflows | Avaliar e governar automações de negócio em escala |
| 📚 [Corporate Training Designer](specialized/corporate-training-designer.md) | Treinamento enterprise, desenvolvimento de currículo | Desenhar sistemas de treinamento e programas de aprendizagem |
| 🏛️ [Government Digital Presales Consultant](specialized/government-digital-presales-consultant.md) | Pré-vendas ToG na China, transformação digital | Propostas e bids de transformação digital governamental |
| ⚕️ [Healthcare Marketing Compliance](specialized/healthcare-marketing-compliance.md) | Compliance de publicidade healthcare na China | Conformidade regulatória de marketing healthcare |
| 🎯 [Recruitment Specialist](specialized/recruitment-specialist.md) | Aquisição de talentos, operações de recruiting | Estratégia de recrutamento, sourcing e processos de contratação |
| 🎓 [Study Abroad Advisor](specialized/study-abroad-advisor.md) | Educação internacional, planejamento de application | Planejamento de estudo no exterior nos EUA, Reino Unido, Canadá, Austrália |
| 🔗 [Supply Chain Strategist](specialized/supply-chain-strategist.md) | Gestão de supply chain, estratégia de procurement | Otimização de supply chain e planejamento de procurement |
| 🗺️ [Workflow Architect](specialized/specialized-workflow-architect.md) | Descoberta, mapeamento e especificação de workflows | Mapear todos os caminhos por um sistema antes de escrever código |
| ☁️ [Salesforce Architect](specialized/specialized-salesforce-architect.md) | Design Salesforce multi-cloud, governor limits, integrações | Arquitetura Salesforce enterprise, estratégia de org, deployment pipelines |
| 🇫🇷 [French Consulting Market Navigator](specialized/specialized-french-consulting-market.md) | Ecossistema ESN/SI, portage salarial, posicionamento de rate | Consultoria freelance no mercado francês de TI |
| 🇰🇷 [Korean Business Navigator](specialized/specialized-korean-business-navigator.md) | Cultura de negócios coreana, processo 품의, mecânica de relacionamentos | Profissionais estrangeiros navegando relações de negócios na Coreia |
| 🏗️ [Civil Engineer](specialized/specialized-civil-engineer.md) | Análise estrutural, design geotécnico, códigos globais de construção | Engenharia estrutural multi-standard em Eurocode, ACI, AISC e mais |
| 🎧 [Customer Service](specialized/customer-service.md) | Suporte omnichannel, tratamento de reclamações, retenção, escalonamento | Suporte ao cliente em qualquer setor - varejo, SaaS, hotelaria, finanças, logística |
| 🏥 [Healthcare Customer Service](specialized/healthcare-customer-service.md) | Suporte a pacientes com consciência de HIPAA, billing, seguro, roteamento de emergências | Organizações healthcare que precisam de suporte ao paciente compliant e empático |
| 🏨 [Hospitality Guest Services](specialized/hospitality-guest-services.md) | Reservas, concierge, recuperação de reclamações, loyalty, eventos | Hotéis, resorts, restaurantes e venues de eventos |
| 🤝 [HR Onboarding](specialized/hr-onboarding.md) | Pre-boarding, compliance, enrollment de benefícios, planos 30-60-90 dias | Qualquer empresa fazendo onboarding de novos hires - de startups a enterprise |
| 🌐 [Language Translator](specialized/language-translator.md) | Tradução espanhol ↔ inglês, consciência de dialetos, contexto cultural | Necessidades de tradução em viagens, negócios, medicina e jurídico |
| ⏱️ [Legal Billing & Time Tracking](specialized/legal-billing-time-tracking.md) | Captura de tempo, narrativas de billing, compliance IOLTA, cobranças | Escritórios de advocacia maximizando recuperação de receita e precisão de billing |
| 📋 [Legal Client Intake](specialized/legal-client-intake.md) | Qualificação de prospects, triagem de conflito, agendamento de consulta | Escritórios convertendo consultas em clientes retidos |
| ⚖️ [Legal Document Review](specialized/legal-document-review.md) | Revisão de contratos, sinalização de riscos, comparação de versões, compliance | Primeira revisão pronta para advogado em qualquer área de prática |
| 🏦 [Loan Officer Assistant](specialized/loan-officer-assistant.md) | Intake de borrower, compliance TRID, tracking de pipeline, coordenação de closing | Times de mortgage e consumer lending |
| 🏠 [Real Estate Buyer & Seller](specialized/real-estate-buyer-seller.md) | Representação de comprador/vendedor, ofertas, coordenação de transação | Transações imobiliárias residenciais e de investimento |
| 🛒 [Retail Customer Returns](specialized/retail-customer-returns.md) | Processamento de devoluções, prevenção de fraude, trocas, devoluções para vendors | Varejo físico, e-commerce e omnichannel |

### 💵 Divisão de Finance

Especialistas em contabilidade, análise financeira, estratégia tributária e pesquisa de investimentos.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📒 [Bookkeeper & Controller](finance/finance-bookkeeper-controller.md) | Fechamento mensal, reconciliação, conformidade GAAP, controles internos | Operações contábeis do dia a dia, prontidão para auditoria, manutenção de registros financeiros |
| 📊 [Financial Analyst](finance/finance-financial-analyst.md) | Modelagem financeira, forecasting, análise de cenários, suporte à decisão | Modelos three-statement, análise de variance, business intelligence data-driven |
| 📈 [FP&A Analyst](finance/finance-fpa-analyst.md) | Budgeting, rolling forecasts, análise de variance, business reviews | Planos operacionais anuais, business reviews mensais, alocação estratégica de recursos |
| 🔍 [Investment Researcher](finance/finance-investment-researcher.md) | Due diligence, análise de portfólio, valuation de ativos, equity research | Desenvolvimento de tese de investimento, avaliação de risco, pesquisa de mercado |
| 🏛️ [Tax Strategist](finance/finance-tax-strategist.md) | Otimização tributária, compliance multijurisdicional, transfer pricing | Estruturação de entidades, análise de ETR, defesa em auditoria, planejamento tributário estratégico |

### 🎮 Divisão de Game Development

Construindo mundos, sistemas e experiências em todos os grandes engines.

#### Agentes Cross-Engine (Engine-Agnostic)

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🎯 [Game Designer](game-development/game-designer.md) | Design de sistemas, autoria de GDD, balanceamento de economia, gameplay loops | Desenhar mecânicas de game, sistemas de progressão, escrever documentos de design |
| 🗺️ [Level Designer](game-development/level-designer.md) | Teoria de layout, pacing, design de encontros, environmental storytelling | Construir levels, desenhar fluxo de encontros, narrativa espacial |
| 🎨 [Technical Artist](game-development/technical-artist.md) | Shaders, VFX, pipeline de LOD, otimização art-to-engine | Ponte entre arte e engenharia, autoria de shaders, asset pipelines seguros para performance |
| 🔊 [Game Audio Engineer](game-development/game-audio-engineer.md) | FMOD/Wwise, música adaptativa, áudio espacial, budgets de áudio | Sistemas de áudio interativo, música dinâmica, performance de áudio |
| 📖 [Narrative Designer](game-development/narrative-designer.md) | Sistemas de história, diálogos ramificados, arquitetura de lore | Escrever narrativas ramificadas, implementar sistemas de diálogo, lore de mundo |

#### Unity

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🏗️ [Unity Architect](game-development/unity/unity-architect.md) | ScriptableObjects, modularidade data-driven, DOTS/ECS | Projetos Unity de grande escala, design de sistemas data-driven, trabalho de performance com ECS |
| ✨ [Unity Shader Graph Artist](game-development/unity/unity-shader-graph-artist.md) | Shader Graph, HLSL, URP/HDRP, Renderer Features | Materiais Unity customizados, shaders VFX, passes de pós-processamento |
| 🌐 [Unity Multiplayer Engineer](game-development/unity/unity-multiplayer-engineer.md) | Netcode for GameObjects, Unity Relay/Lobby, server authority, prediction | Games online em Unity, client prediction, integração com Unity Gaming Services |
| 🛠️ [Unity Editor Tool Developer](game-development/unity/unity-editor-tool-developer.md) | EditorWindows, AssetPostprocessors, PropertyDrawers, validação de build | Tooling customizado de Unity Editor, automação de pipeline, validação de conteúdo |

#### Unreal Engine

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| ⚙️ [Unreal Systems Engineer](game-development/unreal-engine/unreal-systems-engineer.md) | Híbrido C++/Blueprint, GAS, restrições Nanite, gestão de memória | Sistemas complexos de gameplay em Unreal, Gameplay Ability System, C++ em nível de engine |
| 🎨 [Unreal Technical Artist](game-development/unreal-engine/unreal-technical-artist.md) | Material Editor, Niagara, PCG, Substrate | Materiais Unreal, Niagara VFX, geração procedural de conteúdo |
| 🌐 [Unreal Multiplayer Architect](game-development/unreal-engine/unreal-multiplayer-architect.md) | Replicação de Actors, hierarquia GameMode/GameState, dedicated server | Games online em Unreal, replication graphs, Unreal server authoritative |
| 🗺️ [Unreal World Builder](game-development/unreal-engine/unreal-world-builder.md) | World Partition, Landscape, HLOD, LWC | Grandes levels open-world em Unreal, sistemas de streaming, terreno em escala |

#### Godot

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 📜 [Godot Gameplay Scripter](game-development/godot/godot-gameplay-scripter.md) | GDScript 2.0, signals, composição, static typing | Sistemas de gameplay Godot, composição de scenes, GDScript atento à performance |
| 🌐 [Godot Multiplayer Engineer](game-development/godot/godot-multiplayer-engineer.md) | MultiplayerAPI, ENet/WebRTC, RPCs, modelo de autoridade | Games online em Godot, replicação de scenes, Godot server-authoritative |
| ✨ [Godot Shader Developer](game-development/godot/godot-shader-developer.md) | Godot shading language, VisualShader, RenderingDevice | Materiais Godot customizados, efeitos 2D/3D, pós-processamento, compute shaders |

#### Blender

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🧩 [Blender Addon Engineer](game-development/blender/blender-addon-engineer.md) | Blender Python (`bpy`), custom operators/panels, validadores de assets, exporters, automação de pipeline | Construir add-ons Blender, tools de preparo de assets, workflows de export e automação de pipeline DCC |

#### Roblox Studio

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| ⚙️ [Roblox Systems Scripter](game-development/roblox-studio/roblox-systems-scripter.md) | Luau, RemoteEvents/Functions, DataStore, arquitetura de módulos server-authoritative | Construir sistemas seguros de games Roblox, comunicação client-server, persistência de dados |
| 🎯 [Roblox Experience Designer](game-development/roblox-studio/roblox-experience-designer.md) | Loops de engajamento, monetização, retenção D1/D7, fluxo de onboarding | Desenhar loops de games Roblox, Game Passes, recompensas diárias, retenção de jogadores |
| 👗 [Roblox Avatar Creator](game-development/roblox-studio/roblox-avatar-creator.md) | Pipeline UGC, rigging de acessórios, submissão ao Creator Marketplace | Itens Roblox UGC, customização HumanoidDescription, lojas de avatar in-experience |

### 📚 Divisão Acadêmica

Rigor acadêmico para construção de mundos, storytelling e design narrativo.

| Agente | Especialidade | Quando Usar |
|-------|-----------|-------------|
| 🌍 [Anthropologist](academic/academic-anthropologist.md) | Sistemas culturais, parentesco, rituais, sistemas de crença | Desenhar sociedades culturalmente coerentes com lógica interna |
| 🌐 [Geographer](academic/academic-geographer.md) | Geografia física/humana, clima, cartografia | Construir mundos geograficamente coerentes com terreno e assentamentos realistas |
| 📚 [Historian](academic/academic-historian.md) | Análise histórica, periodização, cultura material | Validar coerência histórica, enriquecer cenários com detalhe de época autêntico |
| 📜 [Narratologist](academic/academic-narratologist.md) | Teoria narrativa, estrutura de história, arcos de personagem | Analisar e melhorar estrutura de história com frameworks teóricos estabelecidos |
| 🧠 [Psychologist](academic/academic-psychologist.md) | Teoria da personalidade, motivação, padrões cognitivos | Construir personagens psicologicamente críveis baseados em pesquisa |

---

## 🎯 Casos de Uso do Mundo Real

### Cenário 1: Construindo um MVP de Startup

**Seu Time**:
1. 🎨 **Frontend Developer** - Construir o app React
2. 🏗️ **Backend Architect** - Desenhar a API e o banco de dados
3. 🚀 **Growth Hacker** - Planejar aquisição de usuários
4. ⚡ **Rapid Prototyper** - Ciclos rápidos de iteração
5. 🔍 **Reality Checker** - Garantir qualidade antes do launch

**Resultado**: Ship mais rápido com expertise especializada em cada etapa.

---

### Cenário 2: Launch de Campanha de Marketing

**Seu Time**:
1. 📝 **Content Creator** - Desenvolver conteúdo de campanha
2. 🐦 **Twitter Engager** - Estratégia e execução no Twitter
3. 📸 **Instagram Curator** - Conteúdo visual e stories
4. 🤝 **Reddit Community Builder** - Engajamento autêntico com comunidade
5. 📊 **Analytics Reporter** - Acompanhar e otimizar performance

**Resultado**: Campanha multicanal coordenada com expertise específica de cada plataforma.

---

### Cenário 3: Desenvolvimento de Feature Enterprise

**Seu Time**:
1. 👔 **Senior Project Manager** - Planejamento de escopo e tarefas
2. 💎 **Senior Developer** - Implementação complexa
3. 🎨 **UI Designer** - Design system e componentes
4. 🧪 **Experiment Tracker** - Planejamento de testes A/B
5. 📸 **Evidence Collector** - Verificação de qualidade
6. 🔍 **Reality Checker** - Prontidão de produção

**Resultado**: Entrega enterprise-grade com quality gates e documentação.

---

### Cenário 4: Assumindo uma Conta de Paid Media

**Seu Time**:

1. 📋 **Paid Media Auditor** - Avaliação abrangente da conta
2. 📡 **Tracking & Measurement Specialist** - Verificar precisão do conversion tracking
3. 💰 **PPC Campaign Strategist** - Redesenhar arquitetura da conta
4. 🔍 **Search Query Analyst** - Limpar gasto desperdiçado em termos de busca
5. ✍️ **Ad Creative Strategist** - Atualizar todas as copies de anúncios e extensões
6. 📊 **Analytics Reporter** (Divisão de Support) - Construir dashboards de reporting

**Resultado**: Assunção sistemática da conta com tracking verificado, desperdício eliminado, estrutura otimizada e criativos renovados - tudo nos primeiros 30 dias.

---

### Cenário 5: Product Discovery com a Agência Completa

**Seu Time**: Todas as 8 divisões trabalhando em paralelo em uma única missão.

Veja o **[Exercício Nexus Spatial Discovery](examples/nexus-spatial-discovery.md)** -- um exemplo completo em que 8 agentes (Product Trend Researcher, Backend Architect, Brand Guardian, Growth Hacker, Support Responder, UX Researcher, Project Shepherd e XR Interface Architect) foram acionados simultaneamente para avaliar uma oportunidade de software e produzir um plano de produto unificado cobrindo validação de mercado, arquitetura técnica, estratégia de marca, go-to-market, sistemas de suporte, pesquisa de UX, execução de projeto e design de UI espacial.

**Resultado**: Blueprint de produto abrangente e cross-functional produzido em uma única sessão. [Mais exemplos](examples/).

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Veja como você pode ajudar:

### Adicione um Novo Agente

1. Faça fork do repositório
2. Crie um novo arquivo de agente na categoria apropriada
3. Siga a estrutura de template de agente:
   - Frontmatter com name, description, color
   - Seção Identidade & Memória
   - Missão Principal
   - Regras Críticas (específicas do domínio)
   - Entregáveis Técnicos com exemplos
   - Processo de Workflow
   - Métricas de Sucesso
4. Envie um PR com seu agente

### Melhore Agentes Existentes

- Adicione exemplos do mundo real
- Aprimore exemplos de código
- Atualize métricas de sucesso
- Melhore workflows

### Compartilhe Suas Histórias de Sucesso

Você usou estes agentes com sucesso? Compartilhe sua história nas [Discussions](https://github.com/msitarzewski/agency-agents/discussions)!

---

## 📖 Filosofia de Design dos Agentes

Cada agente é desenhado com:

1. **🎭 Personalidade Forte**: Não são templates genéricos - têm caráter e voz reais
2. **📋 Entregáveis Claros**: Outputs concretos, não orientação vaga
3. **✅ Métricas de Sucesso**: Resultados mensuráveis e padrões de qualidade
4. **🔄 Workflows Comprovados**: Processos passo a passo que funcionam
5. **💡 Memória de Aprendizado**: Reconhecimento de padrões e melhoria contínua

---

## 🎁 O que Torna Isso Especial?

### Diferente de Prompts Genéricos de IA:
- ❌ Prompts genéricos como "Act as a developer"
- ✅ Especialização profunda com personalidade e processo

### Diferente de Bibliotecas de Prompts:
- ❌ Coleções de prompts one-off
- ✅ Sistemas abrangentes de agentes com workflows e entregáveis

### Diferente de Ferramentas de IA:
- ❌ Ferramentas caixa-preta que você não consegue customizar
- ✅ Personalidades de agentes transparentes, forkáveis e adaptáveis

---

## 🎨 Destaques de Personalidade dos Agentes

> "Eu não apenas testo seu código - por padrão encontro 3-5 problemas e exijo prova visual para tudo."
>
> -- **Evidence Collector** (Divisão de Testing)

> "Você não está fazendo marketing no Reddit - você está se tornando um membro valioso da comunidade que por acaso representa uma marca."
>
> -- **Reddit Community Builder** (Divisão de Marketing)

> "Todo elemento lúdico deve servir a um propósito funcional ou emocional. Desenhe encantamento que amplifica em vez de distrair."
>
> -- **Whimsy Injector** (Divisão de Design)

> "Deixe-me adicionar uma animação de celebração que reduz a ansiedade de conclusão de tarefa em 40%"
>
> -- **Whimsy Injector** (durante um review de UX)

---

## 📊 Estatísticas

- 🎭 **144 Agentes Especializados** em 12 divisões
- 📝 **10.000+ linhas** de personalidade, processo e exemplos de código
- ⏱️ **Meses de iteração** a partir de uso no mundo real
- 🌟 **Battle-tested** em ambientes de produção
- 💬 **50+ requests** nas primeiras 12 horas no Reddit

---

## 🔌 Integrações Multi-Tool

The Agency funciona nativamente com Claude Code e traz scripts de conversão + instalação para que você use os mesmos agentes em todas as principais ferramentas de coding agentic.

### Ferramentas Suportadas

- **[Claude Code](https://claude.ai/code)** — agentes `.md` nativos, sem necessidade de conversão → `~/.claude/agents/`
- **[GitHub Copilot](https://github.com/copilot)** — agentes `.md` nativos, sem necessidade de conversão → `~/.github/agents/` + `~/.copilot/agents/`
- **[Antigravity](https://github.com/google-gemini/antigravity)** — `SKILL.md` por agente → `~/.gemini/antigravity/skills/`
- **[Gemini CLI](https://github.com/google-gemini/gemini-cli)** — extensão + arquivos `SKILL.md` → `~/.gemini/extensions/agency-agents/`
- **[OpenCode](https://opencode.ai)** — arquivos de agente `.md` → `.opencode/agents/`
- **[Cursor](https://cursor.sh)** — arquivos de regras `.mdc` → `.cursor/rules/`
- **[Aider](https://aider.chat)** — um único `CONVENTIONS.md` → `./CONVENTIONS.md`
- **[Windsurf](https://codeium.com/windsurf)** — um único `.windsurfrules` → `./.windsurfrules`
- **[OpenClaw](https://github.com/openclaw/openclaw)** — `SOUL.md` + `AGENTS.md` + `IDENTITY.md` por agente
- **[Qwen Code](https://github.com/QwenLM/qwen-code)** — arquivos SubAgent `.md` → `~/.qwen/agents/`
- **[Kimi Code](https://github.com/MoonshotAI/kimi-cli)** — specs YAML de agentes → `~/.config/kimi/agents/`

---

### ⚡ Instalação Rápida

**Passo 1 -- Gere os arquivos de integração:**
```bash
./scripts/convert.sh
# Mais rápido (paralelo, ordem de output pode variar): ./scripts/convert.sh --parallel
```

**Passo 2 -- Instale (interativo, detecta suas ferramentas automaticamente):**
```bash
./scripts/install.sh
# Mais rápido (paralelo, ordem de output pode variar): ./scripts/install.sh --no-interactive --parallel
```

O instalador escaneia seu sistema em busca de ferramentas instaladas, mostra uma UI com checkboxes e permite escolher exatamente o que instalar:

```
  +------------------------------------------------+
  |   The Agency -- Tool Installer                 |
  +------------------------------------------------+

  System scan: [*] = detected on this machine

  [x]  1)  [*]  Claude Code     (claude.ai/code)
  [x]  2)  [*]  Copilot         (~/.github + ~/.copilot)
  [x]  3)  [*]  Antigravity     (~/.gemini/antigravity)
  [ ]  4)  [ ]  Gemini CLI      (gemini extension)
  [ ]  5)  [ ]  OpenCode        (opencode.ai)
  [ ]  6)  [ ]  OpenClaw        (~/.openclaw/agency-agents)
  [x]  7)  [*]  Cursor          (.cursor/rules)
  [ ]  8)  [ ]  Aider           (CONVENTIONS.md)
  [ ]  9)  [ ]  Windsurf        (.windsurfrules)
  [ ] 10)  [ ]  Qwen Code       (~/.qwen/agents)
  [ ] 11)  [ ]  Kimi Code       (~/.config/kimi/agents)

  [1-11] toggle   [a] all   [n] none   [d] detected
  [Enter] install   [q] quit
```

**Ou instale diretamente uma ferramenta específica:**
```bash
./scripts/install.sh --tool cursor
./scripts/install.sh --tool opencode
./scripts/install.sh --tool openclaw
./scripts/install.sh --tool antigravity
```

**Não interativo (CI/scripts):**
```bash
./scripts/install.sh --no-interactive --tool all
```

**Execuções mais rápidas (parallel)** — Em máquinas multi-core, use `--parallel` para que cada tool seja processada em paralelo. A ordem de output entre ferramentas é não determinística. Funciona tanto com instalação interativa quanto não interativa: por exemplo, `./scripts/install.sh --interactive --parallel` (escolha as ferramentas, depois instale em paralelo) ou `./scripts/install.sh --no-interactive --parallel`. A contagem de jobs usa `nproc` (Linux), `sysctl -n hw.ncpu` (macOS) ou 4 por padrão; sobrescreva com `--jobs N`.

```bash
./scripts/convert.sh --parallel                    # converte todas as tools em paralelo
./scripts/convert.sh --parallel --jobs 8           # limita jobs paralelos
./scripts/install.sh --no-interactive --parallel   # instala todas as tools detectadas em paralelo
./scripts/install.sh --interactive --parallel      # escolhe tools, depois instala em paralelo
./scripts/install.sh --no-interactive --parallel --jobs 4
```

---

### Instruções Específicas por Ferramenta

<details>
<summary><strong>Claude Code</strong></summary>

Agentes são copiados diretamente do repo para `~/.claude/agents/` -- sem necessidade de conversão.

```bash
./scripts/install.sh --tool claude-code
```

Então ative no Claude Code:
```
Use the Frontend Developer agent to review this component.
```

Veja [integrations/claude-code/README.md](integrations/claude-code/README.md) para detalhes.
</details>

<details>
<summary><strong>GitHub Copilot</strong></summary>

Agentes são copiados diretamente do repo para `~/.github/agents/` e `~/.copilot/agents/` -- sem necessidade de conversão.

```bash
./scripts/install.sh --tool copilot
```

Então ative no GitHub Copilot:
```
Use the Frontend Developer agent to review this component.
```

Veja [integrations/github-copilot/README.md](integrations/github-copilot/README.md) para detalhes.
</details>

<details>
<summary><strong>Antigravity (Gemini)</strong></summary>

Cada agente vira uma skill em `~/.gemini/antigravity/skills/agency-<slug>/`.

```bash
./scripts/install.sh --tool antigravity
```

Ative no Gemini com Antigravity:
```
@agency-frontend-developer review this React component
```

Veja [integrations/antigravity/README.md](integrations/antigravity/README.md) para detalhes.
</details>

<details>
<summary><strong>Gemini CLI</strong></summary>

Instala como uma extensão do Gemini CLI com uma skill por agente mais um manifest.
Em um clone novo, gere os arquivos da extensão Gemini antes de executar o instalador.

```bash
./scripts/convert.sh --tool gemini-cli
./scripts/install.sh --tool gemini-cli
```

Veja [integrations/gemini-cli/README.md](integrations/gemini-cli/README.md) para detalhes.
</details>

<details>
<summary><strong>OpenCode</strong></summary>

Agentes são colocados em `.opencode/agents/` na raiz do seu projeto (escopo de projeto).

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool opencode
```

Ou instale globalmente:
```bash
mkdir -p ~/.config/opencode/agents
cp integrations/opencode/agents/*.md ~/.config/opencode/agents/
```

Ative no OpenCode:
```
@backend-architect design this API.
```

Veja [integrations/opencode/README.md](integrations/opencode/README.md) para detalhes.
</details>

<details>
<summary><strong>Cursor</strong></summary>

Cada agente vira um arquivo de regra `.mdc` em `.cursor/rules/` do seu projeto.

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool cursor
```

As rules são aplicadas automaticamente quando o Cursor as detecta no projeto. Referencie explicitamente:
```
Use the @security-engineer rules to review this code.
```

Veja [integrations/cursor/README.md](integrations/cursor/README.md) para detalhes.
</details>

<details>
<summary><strong>Aider</strong></summary>

Todos os agentes são compilados em um único arquivo `CONVENTIONS.md` que o Aider lê automaticamente.

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool aider
```

Depois referencie agentes na sua sessão do Aider:
```
Use the Frontend Developer agent to refactor this component.
```

Veja [integrations/aider/README.md](integrations/aider/README.md) para detalhes.
</details>

<details>
<summary><strong>Windsurf</strong></summary>

Todos os agentes são compilados em `.windsurfrules` na raiz do seu projeto.

```bash
cd /your/project
/path/to/agency-agents/scripts/install.sh --tool windsurf
```

Referencie agentes no Cascade do Windsurf:
```
Use the Reality Checker agent to verify this is production ready.
```

Veja [integrations/windsurf/README.md](integrations/windsurf/README.md) para detalhes.
</details>

<details>
<summary><strong>OpenClaw</strong></summary>

Cada agente vira um workspace com `SOUL.md`, `AGENTS.md` e `IDENTITY.md` em `~/.openclaw/agency-agents/`.

```bash
./scripts/convert.sh --tool openclaw
./scripts/install.sh --tool openclaw
```

Se o CLI `openclaw` estiver disponível, o instalador registra cada workspace automaticamente.
Execute `openclaw gateway restart` após a instalação para que os novos agentes sejam ativados.

Veja [integrations/openclaw/README.md](integrations/openclaw/README.md) para detalhes.

</details>

<details>
<summary><strong>Qwen Code</strong></summary>

SubAgents são instalados em `.qwen/agents/` na raiz do seu projeto (escopo de projeto).

```bash
# Converta e instale (execute a partir da raiz do seu projeto)
cd /your/project
./scripts/convert.sh --tool qwen
./scripts/install.sh --tool qwen
```

**Uso no Qwen Code:**
- Referencie por nome: `Use the frontend-developer agent to review this component`
- Ou deixe o Qwen auto-delegar com base no contexto da tarefa
- Gerencie via comando `/agents` no modo interativo

> 📚 [Qwen SubAgents Docs](https://qwenlm.github.io/qwen-code-docs/en/users/features/sub-agents/)

</details>

<details>
<summary><strong>Kimi Code</strong></summary>

Agentes são convertidos para o formato Kimi Code CLI (YAML + system prompt) e instalados em `~/.config/kimi/agents/`.

```bash
# Converta e instale
./scripts/convert.sh --tool kimi
./scripts/install.sh --tool kimi
```

**Uso com Kimi Code:**
```bash
# Use um agente
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml

# Em um projeto
kimi --agent-file ~/.config/kimi/agents/frontend-developer/agent.yaml \
     --work-dir /your/project \
     "Review this React component"
```

Veja [integrations/kimi/README.md](integrations/kimi/README.md) para detalhes.

</details>

---

### Regenerando Depois de Mudanças

Quando você adicionar novos agentes ou editar agentes existentes, regenere todos os arquivos de integração:

```bash
./scripts/convert.sh                    # regenera todos (serial)
./scripts/convert.sh --parallel         # regenera todos em paralelo (mais rápido)
./scripts/convert.sh --tool cursor      # regenera apenas uma tool
```

---

## 🗺️ Roadmap

- [ ] Ferramenta web interativa de seleção de agentes
- [x] Exemplos de workflow multiagente -- veja [examples/](examples/)
- [x] Scripts de integração multi-tool (Claude Code, GitHub Copilot, Antigravity, Gemini CLI, OpenCode, OpenClaw, Cursor, Aider, Windsurf, Qwen Code, Kimi Code)
- [ ] Tutoriais em vídeo sobre design de agentes
- [ ] Marketplace de agentes da comunidade
- [ ] "Quiz de personalidade" de agentes para matching com projetos
- [ ] Série de showcases "Agent of the Week"

---

## 🌐 Traduções & Localizações da Comunidade

Traduções e adaptações regionais mantidas pela comunidade. Elas são mantidas de forma independente -- veja cada repo para cobertura e compatibilidade de versão.

| Idioma | Mantenedor | Link | Observações |
|----------|-----------|------|-------|
| 🇨🇳 简体中文 (zh-CN) | [@jnMetaCode](https://github.com/jnMetaCode) | [agency-agents-zh](https://github.com/jnMetaCode/agency-agents-zh) | 141 agentes traduzidos + 46 originais para o mercado chinês |
| 🇨🇳 简体中文 (zh-CN) | [@dsclca12](https://github.com/dsclca12) | [agent-teams](https://github.com/dsclca12/agent-teams) | Tradução independente com localização para Bilibili, WeChat, Xiaohongshu |

Quer adicionar uma tradução? Abra uma issue e vamos linkar aqui.

---

## 🔗 Recursos Relacionados

- [awesome-openclaw-agents](https://github.com/mergisi/awesome-openclaw-agents) — Coleção de agentes OpenClaw mantida pela comunidade (derivada deste repo)

---

## 📜 Licença

Licença MIT - Use livremente, comercial ou pessoalmente. Atribuição é apreciada, mas não obrigatória.

---

## 🙏 Agradecimentos

O que começou como uma thread no Reddit sobre especialização de agentes de IA se tornou algo notável — **147 agentes em 12 divisões**, apoiados por uma comunidade de contribuidores do mundo todo. Cada agente neste repo existe porque alguém se importou o suficiente para escrevê-lo, testá-lo e compartilhá-lo.

A todas as pessoas que abriram um PR, registraram uma issue, começaram uma Discussion ou simplesmente testaram um agente e contaram o que funcionou — obrigado. Vocês são o motivo de The Agency continuar melhorando.

---

## 💬 Comunidade

- **GitHub Discussions**: [Compartilhe suas histórias de sucesso](https://github.com/msitarzewski/agency-agents/discussions)
- **Issues**: [Reporte bugs ou solicite features](https://github.com/msitarzewski/agency-agents/issues)
- **Reddit**: Participe da conversa em r/ClaudeAI
- **Twitter/X**: Compartilhe com #TheAgency

---

## 🚀 Comece Agora

1. **Explore** os agentes acima e encontre especialistas para suas necessidades
2. **Copie** os agentes para `~/.claude/agents/` para integração com Claude Code
3. **Ative** agentes referenciando-os nas suas conversas com Claude
4. **Customize** personalidades e workflows de agentes para suas necessidades específicas
5. **Compartilhe** seus resultados e contribua de volta para a comunidade

---

<div align="center">

**🎭 The Agency: Seu Dream Team de IA Espera por Você 🎭**

[⭐ Dê uma Star neste repo](https://github.com/msitarzewski/agency-agents) • [🍴 Faça um Fork](https://github.com/msitarzewski/agency-agents/fork) • [🐛 Reporte uma issue](https://github.com/msitarzewski/agency-agents/issues) • [❤️ Sponsor](https://github.com/sponsors/msitarzewski)

Feito com ❤️ pela comunidade, para a comunidade

</div>
