# Integração MCP Memory

> Dê a qualquer agente memória persistente entre sessões usando o Model Context Protocol (MCP).

## O que Ela Faz

Por padrão, agentes em The Agency começam cada sessão do zero. O contexto é passado manualmente via copy-paste entre agentes e sessões. Um servidor MCP de memória muda isso:

- **Memória entre sessões**: Um agente lembra decisões, entregáveis e contexto de sessões anteriores
- **Continuidade de handoff**: Quando um agente faz handoff para outro, o agente recebedor consegue lembrar exatamente o que foi feito — sem copy-paste
- **Rollback em falhas**: Quando uma checagem de QA falha ou uma decisão de arquitetura se mostra errada, volte para um estado conhecido como bom em vez de recomeçar

## Setup

Você precisa de um servidor MCP que forneça tools de memória: `remember`, `recall`, `rollback` e `search`. Adicione-o à configuração do seu cliente MCP (Claude Code, Cursor etc.):

```json
{
  "mcpServers": {
    "memory": {
      "command": "your-mcp-memory-server",
      "args": []
    }
  }
}
```

Qualquer servidor MCP que exponha as tools `remember`, `recall`, `rollback` e `search` funcionará. Consulte o [ecossistema MCP](https://modelcontextprotocol.io) para implementações disponíveis.

## Como Adicionar Memória a Qualquer Agente

Para aprimorar um agente existente com memória persistente, adicione uma seção **Memory Integration** ao prompt do agente. Essa seção instrui o agente a usar tools de memória MCP em momentos-chave.

### O Padrão

```markdown
## Memory Integration

When you start a session:
- Recall relevant context from previous sessions using your role and the current project as search terms
- Review any memories tagged with your agent name to pick up where you left off

When you make key decisions or complete deliverables:
- Remember the decision or deliverable with descriptive tags (your agent name, the project, the topic)
- Include enough context that a future session — or a different agent — can understand what was done and why

When handing off to another agent:
- Remember your deliverables tagged for the receiving agent
- Include the handoff metadata: what you completed, what's pending, and what the next agent needs to know

When something fails and you need to recover:
- Search for the last known-good state
- Use rollback to restore to that point rather than rebuilding from scratch
```

### O que o Agente Faz com Isso

O LLM usará as tools MCP de memória automaticamente quando receber estas instruções:

- `remember` — armazenar uma decisão, entregável ou snapshot de contexto com tags
- `recall` — buscar memórias relevantes por keyword, tag ou similaridade semântica
- `rollback` — reverter para um estado anterior quando algo dá errado
- `search` — encontrar memórias específicas entre sessões e agentes

Sem mudanças de código nos arquivos de agentes. Sem chamadas de API para escrever. As tools MCP cuidam de tudo.

## Exemplo: Aprimorando o Backend Architect

Veja [backend-architect-with-memory.md](backend-architect-with-memory.md) para um exemplo completo — o agente Backend Architect padrão com uma seção Memory Integration adicionada.

## Exemplo: Workflow com Memória

Veja [../../examples/workflow-with-memory.md](../../examples/workflow-with-memory.md) para o workflow Startup MVP aprimorado com memória persistente, mostrando como agentes passam contexto pela memória em vez de copy-paste.

## Dicas

- **Use tags de forma consistente**: Use o nome do agente e o nome do projeto como tags em toda memória. Isso torna o recall confiável.
- **Deixe o LLM decidir o que é importante**: As instruções de memória são orientação, não regras rígidas. O LLM descobrirá quando lembrar e o que recuperar.
- **Rollback é a killer feature**: Quando um Reality Checker reprova um entregável, o agente original pode voltar ao último checkpoint em vez de tentar desfazer manualmente as mudanças.
