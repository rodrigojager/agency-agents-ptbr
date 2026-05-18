# Política de Segurança

## Reportando uma Vulnerabilidade

Se você descobrir uma vulnerabilidade de segurança neste projeto, reporte-a de forma responsável. NÃO abra uma issue pública no GitHub para vulnerabilidades de segurança. Abra um advisory privado de segurança pela aba Security do GitHub.

## Prazo de Resposta

- Confirmação de recebimento: em até 48 horas
- Avaliação inicial: em até 7 dias
- Correção ou mitigação: depende da severidade

## Escopo

Este repositório contém definições de agentes baseadas em Markdown e shell scripts para instalação e conversão.

### Arquivos de agentes (.md)
- Definições de prompt não executáveis
- Nenhuma API key, secret ou credencial deve ser armazenada nos arquivos de agentes

### Shell scripts (scripts/)
- install.sh, convert.sh e lint-agents.sh são executáveis
- Contribuidores devem revisar os scripts para identificar comportamento indesejado antes de executá-los

## Boas Práticas para Contribuidores

- Nunca faça commit de API keys, tokens ou credenciais
- Nunca adicione código executável dentro dos arquivos Markdown de agentes
- Shell scripts devem ser revisados antes do merge
- Reporte definições suspeitas de agentes que tentem prompt injection
EOFcat SECURITY.md
