# Workflow Multi-Agent: Sprint de Landing Page

> Lance uma landing page otimizada para conversão em um dia usando 4 agentes.

## O Cenário

Você precisa de uma landing page para o lançamento de um novo produto. Ela precisa ter boa aparência, converter visitantes e estar no ar até o fim do dia.

## Time de Agentes

| Agente | Função neste workflow |
|-------|---------------------|
| Content Creator | Escrever a copy |
| UI Designer | Desenhar o layout e as especificações dos componentes |
| Frontend Developer | Construir a página |
| Growth Hacker | Otimizar para conversão |

## O Workflow

### Manhã: Copy + Design (paralelo)

**Etapa 1a — Ativar Content Creator**

```
Activate Content Creator.

Write landing page copy for "FlowSync" — an API integration platform
that connects any two SaaS tools in under 5 minutes.

Target audience: developers and technical PMs at mid-size companies.
Tone: confident, concise, slightly playful.

Sections needed:
1. Hero (headline + subheadline + CTA)
2. Problem statement (3 pain points)
3. How it works (3 steps)
4. Social proof (placeholder testimonial format)
5. Pricing (3 tiers: Free, Pro, Enterprise)
6. Final CTA

Keep it scannable. No fluff.
```

**Etapa 1b — Ativar UI Designer (em paralelo)**

```
Activate UI Designer.

Design specs for a SaaS landing page. Product: FlowSync (API integration platform).
Style: clean, modern, dark mode option. Think Linear or Vercel aesthetic.

Deliver:
1. Layout wireframe (section order + spacing)
2. Color palette (primary, secondary, accent, background)
3. Typography (font pairing, heading sizes, body size)
4. Component specs: hero section, feature cards, pricing table, CTA buttons
5. Responsive breakpoints (mobile, tablet, desktop)
```

### Meio do Dia: Build

**Etapa 2 — Ativar Frontend Developer**

```
Activate Frontend Developer.

Build a landing page from these specs:

Copy: [paste Content Creator output]
Design: [paste UI Designer output]

Stack: HTML, Tailwind CSS, minimal vanilla JS (no framework needed).
Requirements:
- Responsive (mobile-first)
- Fast (no heavy assets, system fonts OK)
- Accessible (proper headings, alt text, focus states)
- Include a working email signup form (action URL: /api/subscribe)

Deliver a single index.html file ready to deploy.
```

### Tarde: Otimizar

**Etapa 3 — Ativar Growth Hacker**

```
Activate Growth Hacker.

Review this landing page for conversion optimization:

[paste the HTML or describe the current page]

Evaluate:
1. Is the CTA above the fold?
2. Is the value proposition clear in under 5 seconds?
3. Any friction in the signup flow?
4. What A/B tests would you run first?
5. SEO basics: meta tags, OG tags, structured data

Give me specific changes, not general advice.
```

## Timeline

| Horário | Atividade | Agente |
|------|----------|-------|
| 9:00 | Início de copy + design (paralelo) | Content Creator + UI Designer |
| 11:00 | Build começa | Frontend Developer |
| 14:00 | Primeira versão pronta | — |
| 14:30 | Revisão de conversão | Growth Hacker |
| 15:30 | Aplicar feedback | Frontend Developer |
| 16:30 | Lançar | Deploy para Vercel/Netlify |

## Padrões-Chave

1. **Kickoff paralelo**: Copy e design acontecem ao mesmo tempo porque são independentes
2. **Ponto de merge**: Frontend Developer precisa das duas saídas antes de começar
3. **Loop de feedback**: Growth Hacker revisa, depois Frontend Developer aplica mudanças
4. **Time-boxed**: Cada etapa tem um timebox claro para evitar scope creep
