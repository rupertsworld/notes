# The agent layer
#ai #agents 

The agent runtime is a distinct layer from the LLM itself. See [[Karpathy on 'claws']].

## The stack

1. **LLM** - the model (inference, weights, context window)
2. **Agent** - tool use, reasoning loops, single-task execution
3. **Agent runtime** - orchestration, scheduling, persistence, multi-agent coordination

## See also

- [[Gopher agents]] - HN comment on how agent-mediated interaction might favor simpler protocols
- [[AgentMail]] - Email infrastructure API for agents
- [[OpenClaw Gateway Protocol]] - Unified control/transport protocol for agent systems
- [[Karpathy on building for agents]] - CLIs, MCP, Skills as the agent-accessible interface layer
