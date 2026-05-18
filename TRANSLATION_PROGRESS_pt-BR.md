# Progresso da Tradução pt-BR dos Agentes

Este documento registra o andamento da tradução **manual** dos agentes para português brasileiro, com foco em contexto e semântica.

## Objetivo
> **Importante:** este fluxo é 100% manual. Não usar scripts automáticos de tradução.

- Traduzir os arquivos de agentes (`*.md`) para pt-BR com qualidade editorial.
- Preservar termos em inglês quando forem realmente naturais no uso brasileiro (ex.: bug, commit, push, deploy, issue, branch, pull request, merge request, CEO, mouse).
- Manter consistência entre sessões futuras de trabalho.

## Diretrizes de Tradução (padrão do projeto)
1. **Tradução manual e contextual**
   - Não fazer substituição palavra-por-palavra.
   - Priorizar sentido do trecho no contexto do agente.

2. **Preservação de termos técnicos (quando natural no Brasil)**
   - Manter em inglês: bug, commit, push, deploy, issue, branch, pull request, merge request, CEO, mouse.
   - Avaliar caso a caso outros termos técnicos conforme contexto.

3. **Tom e estilo**
   - Preservar a personalidade do agente.
   - Manter tom profissional, direto e claro.

4. **Estrutura do arquivo**
   - Manter frontmatter YAML (`name`, `description`, `color`, `emoji`, `vibe`).
   - Manter seções, listas, blocos de código e templates técnicos.
   - Traduzir títulos e conteúdo, sem quebrar formatação Markdown.

5. **Nomenclatura de agentes**
   - Traduzir `name` quando houver equivalente natural em pt-BR.
   - Não forçar tradução estranha de nomes técnicos.

6. **Qualidade mínima antes de concluir um arquivo**
   - Revisar fluidez em pt-BR.
   - Verificar consistência terminológica.
   - Confirmar que não há trechos em “portunhol técnico”/mistura artificial.

## Status Atual

### Concluídos
- [x] `design/design-brand-guardian.md`
- [x] `design/design-ui-designer.md`
- [x] `design/design-ux-researcher.md`
- [x] `design/design-ux-architect.md`
- [x] `design/design-image-prompt-engineer.md`
- [x] `design/design-inclusive-visuals-specialist.md`
- [x] `design/design-whimsy-injector.md`
- [x] `design/design-visual-storyteller.md`
- [x] `academic/academic-anthropologist.md`
- [x] `academic/academic-geographer.md`
- [x] `academic/academic-historian.md`
- [x] `academic/academic-narratologist.md`
- [x] `academic/academic-psychologist.md`
- [x] `engineering/engineering-code-reviewer.md`
- [x] `engineering/engineering-backend-architect.md`
- [x] `engineering/engineering-ai-engineer.md`
- [x] `engineering/engineering-ai-data-remediation-engineer.md`
- [x] `engineering/engineering-cms-developer.md`
- [x] `engineering/engineering-codebase-onboarding-engineer.md`
- [x] `engineering/engineering-data-engineer.md`
- [x] `engineering/engineering-database-optimizer.md`
- [x] `engineering/engineering-devops-automator.md`
- [x] `engineering/engineering-email-intelligence-engineer.md`
- [x] `engineering/engineering-embedded-firmware-engineer.md`
- [x] `engineering/engineering-feishu-integration-developer.md`
- [x] `engineering/engineering-filament-optimization-specialist.md`
- [x] `engineering/engineering-frontend-developer.md`
- [x] `engineering/engineering-software-architect.md`
- [x] `engineering/engineering-git-workflow-master.md`
- [x] `engineering/engineering-incident-response-commander.md`
- [x] `engineering/engineering-minimal-change-engineer.md`
- [x] `engineering/engineering-mobile-app-builder.md`
- [x] `engineering/engineering-rapid-prototyper.md`
- [x] `engineering/engineering-security-engineer.md`
- [x] `engineering/engineering-senior-developer.md`
- [x] `engineering/engineering-sre.md`
- [x] `engineering/engineering-solidity-smart-contract-engineer.md`
- [x] `engineering/engineering-technical-writer.md`
- [x] `engineering/engineering-threat-detection-engineer.md`
- [x] `engineering/engineering-autonomous-optimization-architect.md`
- [x] `engineering/engineering-voice-ai-integration-engineer.md`
- [x] `engineering/engineering-wechat-mini-program-developer.md`
- [x] `finance/finance-financial-analyst.md`
- [x] `finance/finance-bookkeeper-controller.md`
- [x] `finance/finance-fpa-analyst.md`
- [x] `finance/finance-investment-researcher.md`
- [x] `finance/finance-tax-strategist.md`
- [x] `game-development/game-designer.md`
- [x] `game-development/level-designer.md`
- [x] `game-development/game-audio-engineer.md`
- [x] `game-development/technical-artist.md`
- [x] `game-development/narrative-designer.md`
- [x] `game-development/blender/blender-addon-engineer.md`
- [x] `game-development/godot/godot-gameplay-scripter.md`
- [x] `game-development/godot/godot-multiplayer-engineer.md`
- [x] `game-development/godot/godot-shader-developer.md`
- [x] `game-development/roblox-studio/roblox-avatar-creator.md`
- [x] `game-development/roblox-studio/roblox-experience-designer.md`
- [x] `game-development/roblox-studio/roblox-systems-scripter.md`
- [x] `game-development/unity/unity-architect.md`
- [x] `game-development/unity/unity-editor-tool-developer.md`
- [x] `game-development/unity/unity-multiplayer-engineer.md`
- [x] `game-development/unity/unity-shader-graph-artist.md`
- [x] `game-development/unreal-engine/unreal-multiplayer-architect.md`
- [x] `game-development/unreal-engine/unreal-systems-engineer.md`
- [x] `game-development/unreal-engine/unreal-technical-artist.md`
- [x] `game-development/unreal-engine/unreal-world-builder.md`
- [x] `paid-media/paid-media-auditor.md`
- [x] `paid-media/paid-media-creative-strategist.md`
- [x] `paid-media/paid-media-paid-social-strategist.md`
- [x] `paid-media/paid-media-ppc-strategist.md`
- [x] `paid-media/paid-media-programmatic-buyer.md`
- [x] `paid-media/paid-media-search-query-analyst.md`
- [x] `paid-media/paid-media-tracking-specialist.md`
- [x] `product/product-behavioral-nudge-engine.md`
- [x] `product/product-feedback-synthesizer.md`
- [x] `product/product-manager.md`
- [x] `product/product-sprint-prioritizer.md`
- [x] `product/product-trend-researcher.md`
- [x] `project-management/project-management-experiment-tracker.md`
- [x] `project-management/project-management-jira-workflow-steward.md`
- [x] `project-management/project-management-project-shepherd.md`
- [x] `project-management/project-management-studio-operations.md`
- [x] `project-management/project-management-studio-producer.md`
- [x] `project-management/project-manager-senior.md`
- [x] `sales/sales-account-strategist.md`
- [x] `sales/sales-coach.md`
- [x] `sales/sales-deal-strategist.md`
- [x] `sales/sales-discovery-coach.md`
- [x] `sales/sales-engineer.md`
- [x] `sales/sales-outbound-strategist.md`
- [x] `sales/sales-pipeline-analyst.md`
- [x] `sales/sales-proposal-strategist.md`
- [x] `support/support-analytics-reporter.md`
- [x] `support/support-executive-summary-generator.md`
- [x] `support/support-finance-tracker.md`
- [x] `support/support-infrastructure-maintainer.md`
- [x] `support/support-legal-compliance-checker.md`
- [x] `support/support-support-responder.md`
- [x] `spatial-computing/macos-spatial-metal-engineer.md`
- [x] `spatial-computing/terminal-integration-specialist.md`
- [x] `spatial-computing/visionos-spatial-engineer.md`
- [x] `spatial-computing/xr-cockpit-interaction-specialist.md`
- [x] `spatial-computing/xr-immersive-developer.md`
- [x] `spatial-computing/xr-interface-architect.md`
- [x] `testing/testing-api-tester.md`
- [x] `testing/testing-evidence-collector.md`
- [x] `testing/testing-reality-checker.md`
- [x] `testing/testing-accessibility-auditor.md`
- [x] `testing/testing-performance-benchmarker.md`
- [x] `testing/testing-test-results-analyzer.md`
- [x] `testing/testing-tool-evaluator.md`
- [x] `testing/testing-workflow-optimizer.md`
- [x] `examples/README.md`
- [x] `examples/workflow-book-chapter.md`
- [x] `examples/workflow-landing-page.md`
- [x] `examples/workflow-startup-mvp.md`
- [x] `examples/workflow-with-memory.md`
- [x] `examples/nexus-spatial-discovery.md`
- [x] `.github/PULL_REQUEST_TEMPLATE.md`
- [x] `CONTRIBUTING.md`
- [x] `CONTRIBUTING_zh-CN.md`
- [x] `README.md`
- [x] `SECURITY.md`
- [x] `scripts/i18n/README.md`
- [x] `integrations/aider/README.md`
- [x] `integrations/antigravity/README.md`
- [x] `integrations/claude-code/README.md`
- [x] `integrations/cursor/README.md`
- [x] `integrations/gemini-cli/README.md`
- [x] `integrations/github-copilot/README.md`
- [x] `integrations/kimi/README.md`
- [x] `integrations/mcp-memory/backend-architect-with-memory.md`
- [x] `integrations/mcp-memory/README.md`
- [x] `integrations/openclaw/README.md`
- [x] `integrations/opencode/README.md`
- [x] `integrations/qwen/README.md`
- [x] `integrations/README.md`
- [x] `integrations/windsurf/README.md`
- [x] `marketing/marketing-agentic-search-optimizer.md`
- [x] `marketing/marketing-ai-citation-strategist.md`
- [x] `marketing/marketing-app-store-optimizer.md`
- [x] `marketing/marketing-baidu-seo-specialist.md`
- [x] `marketing/marketing-bilibili-content-strategist.md`
- [x] `marketing/marketing-carousel-growth-engine.md`
- [x] `marketing/marketing-china-ecommerce-operator.md`
- [x] `marketing/marketing-china-market-localization-strategist.md`
- [x] `marketing/marketing-content-creator.md`
- [x] `marketing/marketing-cross-border-ecommerce.md`
- [x] `marketing/marketing-douyin-strategist.md`
- [x] `marketing/marketing-growth-hacker.md`
- [x] `marketing/marketing-book-co-author.md`
- [x] `marketing/marketing-instagram-curator.md`
- [x] `marketing/marketing-kuaishou-strategist.md`
- [x] `marketing/marketing-linkedin-content-creator.md`
- [x] `marketing/marketing-livestream-commerce-coach.md`
- [x] `marketing/marketing-podcast-strategist.md`
- [x] `marketing/marketing-private-domain-operator.md`
- [x] `marketing/marketing-video-optimization-specialist.md`
- [x] `marketing/marketing-reddit-community-builder.md`
- [x] `marketing/marketing-seo-specialist.md`
- [x] `marketing/marketing-short-video-editing-coach.md`
- [x] `marketing/marketing-social-media-strategist.md`
- [x] `marketing/marketing-tiktok-strategist.md`
- [x] `marketing/marketing-twitter-engager.md`
- [x] `marketing/marketing-weibo-strategist.md`
- [x] `marketing/marketing-wechat-official-account.md`
- [x] `marketing/marketing-xiaohongshu-specialist.md`
- [x] `marketing/marketing-zhihu-strategist.md`
- [x] `strategy/coordination/agent-activation-prompts.md`
- [x] `strategy/coordination/handoff-templates.md`
- [x] `strategy/EXECUTIVE-BRIEF.md`
- [x] `strategy/nexus-strategy.md`
- [x] `strategy/QUICKSTART.md`
- [x] `strategy/playbooks/phase-0-discovery.md`
- [x] `strategy/playbooks/phase-1-strategy.md`
- [x] `strategy/playbooks/phase-2-foundation.md`
- [x] `strategy/playbooks/phase-3-build.md`
- [x] `strategy/playbooks/phase-4-hardening.md`
- [x] `strategy/playbooks/phase-5-launch.md`
- [x] `strategy/playbooks/phase-6-operate.md`
- [x] `strategy/runbooks/scenario-enterprise-feature.md`
- [x] `strategy/runbooks/scenario-incident-response.md`
- [x] `strategy/runbooks/scenario-marketing-campaign.md`
- [x] `strategy/runbooks/scenario-startup-mvp.md`
- [x] `specialized/agents-orchestrator.md`
- [x] `specialized/agentic-identity-trust.md`
- [x] `specialized/accounts-payable-agent.md`
- [x] `specialized/automation-governance-architect.md`
- [x] `specialized/blockchain-security-auditor.md`
- [x] `specialized/compliance-auditor.md`
- [x] `specialized/corporate-training-designer.md`
- [x] `specialized/customer-service.md`
- [x] `specialized/data-consolidation-agent.md`
- [x] `specialized/government-digital-presales-consultant.md`
- [x] `specialized/healthcare-customer-service.md`
- [x] `specialized/healthcare-marketing-compliance.md`
- [x] `specialized/hr-onboarding.md`
- [x] `specialized/identity-graph-operator.md`
- [x] `specialized/language-translator.md`
- [x] `specialized/legal-client-intake.md`
- [x] `specialized/legal-billing-time-tracking.md`
- [x] `specialized/legal-document-review.md`
- [x] `specialized/loan-officer-assistant.md`
- [x] `specialized/lsp-index-engineer.md`
- [x] `specialized/report-distribution-agent.md`
- [x] `specialized/recruitment-specialist.md`
- [x] `specialized/retail-customer-returns.md`
- [x] `specialized/sales-data-extraction-agent.md`
- [x] `specialized/sales-outreach.md`
- [x] `specialized/specialized-chief-of-staff.md`
- [x] `specialized/specialized-civil-engineer.md`
- [x] `specialized/specialized-cultural-intelligence-strategist.md`
- [x] `specialized/specialized-developer-advocate.md`
- [x] `specialized/specialized-document-generator.md`
- [x] `specialized/specialized-french-consulting-market.md`
- [x] `specialized/specialized-korean-business-navigator.md`
- [x] `specialized/specialized-mcp-builder.md`
- [x] `specialized/specialized-model-qa.md`
- [x] `specialized/specialized-salesforce-architect.md`
- [x] `specialized/zk-steward.md`
- [x] `specialized/study-abroad-advisor.md`
- [x] `specialized/supply-chain-strategist.md`
- [x] `specialized/real-estate-buyer-seller.md`
- [x] `specialized/specialized-workflow-architect.md`
- [x] `specialized/hospitality-guest-services.md`

### Em andamento
- [ ] _(nenhum no momento)_

### Pendentes
- [ ] _(nenhum no momento — 226/226 arquivos Markdown de agentes traduzidos e marcados como concluídos)_

## Revisão de Qualidade

### Corrigidos após comparação com upstream
- [x] `design/design-brand-guardian.md` — conteúdo ausente restaurado no template de identidade de marca.
- [x] `design/design-ui-designer.md` — conteúdo ausente restaurado no design system e template de entregável.
- [x] `design/design-ux-researcher.md` — conteúdo ausente restaurado em critérios de participantes, protocolo, persona, findings, memória e capacidades avançadas.
- [x] `design/design-image-prompt-engineer.md` — camadas do framework, workflow e template de retrato ambiental restaurados.
- [x] `design/design-whimsy-injector.md` — taxonomia, microcopy, gamificação e capacidades avançadas restauradas.
- [x] `engineering/engineering-cms-developer.md` — trechos remanescentes em inglês traduzidos e estrutura preservada.

## Como retomar a tradução em uma próxima sessão
1. Abrir este arquivo: `TRANSLATION_PROGRESS_pt-BR.md`.
2. Se novos agentes forem adicionados ao repositório, continuar a partir da seção **Em andamento** ou incluir os novos arquivos em **Pendentes**.
3. Ao concluir um agente:
   - mover para **Concluídos**;
   - remover de **Em andamento/Pendentes**;
   - manter as diretrizes acima sem exceções.
4. Fazer commit com mensagem explícita, por exemplo:
   - `Manually translate academic-historian agent to pt-BR`

## Regra de ouro
Se houver dúvida entre “tradução literal” e “naturalidade em pt-BR”, escolher sempre a redação mais natural **sem perder precisão técnica**.
