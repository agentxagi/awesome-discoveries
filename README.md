# Awesome Discoveries

Curadoria viva de projetos, ferramentas e insights sobre AI agents, multi-agent systems, e infra de producao.

**Atualizado automaticamente** - alimentado por descobertas reais no X/Twitter e GitHub.

Maintained by [@agentxagi](https://x.com/agentxagi).

Contribuicoes bem-vindas - abre uma issue ou PR.

## Como funciona

O Growth Agent roda ciclos a cada 30min, buscando conversas relevantes no X e projetos interessantes no GitHub. Tudo que e genuinamente interessante entra aqui - com contexto real, nao so links.

## Criterio de inclusao

- **Resolve um problema real** - nao e demo/hype
- **Tem comunidade ativa** - stars, commits recentes, issues respondidas
- **Ou e um insight original** - algo que vale a pena compartilhar

## Categorias

### Agents & Frameworks
> Agentes autonomos, frameworks de coordenacao, tool-use

### LLM & RAG
> Embeddings, retrieval, fine-tuning, serving, evals

### Multi-Agent Systems
> Orquestracao, handoffs, memoria compartilhada, circuit breakers

### Agent Infrastructure
> Monitoring, reliability, security, cost management, testing

### Ferramentas & CLIs
> Ferramentas de desenvolvimento, debugging, deploy

---

## Agents & Frameworks

### [skillgrade](https://github.com/mgechev/skillgrade) - Unit tests for agent skills
Run assertions against agent skill outputs the same way you would test code. From Minko Gechev (Angular team lead). TypeScript, MIT license, 480+ stars. The unit test metaphor maps cleanly to agent skills.

### [agent-skills-eval](https://github.com/darkrishabh/agent-skills-eval) - Test runner for agentskills.io skills
YAML-based scenarios with LLM judges. 500+ stars in two weeks. TypeScript, works with any OpenAI-compatible API.

## Agent Infrastructure

### [eval-view](https://github.com/hidai25/eval-view) - Regression testing for AI agents
Snapshot agent behavior, diff tool calls between runs, catch regressions in CI. Works with LangGraph, CrewAI, OpenAI, Anthropic. Python/pytest-based.

### [agent-belt](https://github.com/jfrog/agent-belt) - Eval framework for coding agents (JFrog)
CLI-based, runs multi-turn scenarios with rich assertions and multi-judge consensus. Works against Claude Code, Codex, Copilot, or any agent you plug in. From JFrog engineering.

---

## LLM & RAG

*Nenhum item ainda.*

## Multi-Agent Systems

### Orchestration & Coordination

### [contrabass](https://github.com/junhoyeo/contrabass) - Project-level orchestrator for AI coding agents
Go + Charm TUI implementation of OpenAI's Symphony SPEC.md. Coordinates multiple coding agents (Codex, Claude Code) from a single interface. 151 stars, Go binary, actively maintained. The "one orchestrator, many coding CLIs" pattern.

### OpenAI Symphony SPEC.md - Standard for autonomous coding agent orchestration
OpenAI open-sourced a SPEC.md defining how coding agents should be orchestrated: issue intake, agent spawning, artifact management. Already spawning implementations (contrabass, symphony forks). Think of it as docker-compose for coding agents. [InfoQ coverage](https://www.infoq.com/news/2026/05/openai-symphony-agents/).


### [TraceFix](https://ortiz.rutgers.edu/projects/tracefix/) - TLA+-based protocol repair for multi-agent coordination
Uses TLA+ counterexamples to find and repair coordination protocol violations before deployment. Formal methods meet agent orchestration. CAISconf 2026 paper from Rutgers (Jorge Ortiz et al.). Instead of discovering protocol failures in production, catch them at design time.

### [Warp Oz](https://x.com/warpdotdev/status/2056772856835453395) - Multi-agent orchestration across coding agents
Delegate complex tasks across Claude Code, Codex, and Warp Agent from a single terminal. Each subagent gets its own worktree (local) or Docker container (cloud). The /orchestrate command generates a delegation plan and agents coordinate via structured message passing. 177 likes, 81k views on launch. First terminal orchestrator that crosses framework boundaries.

### Memory architecture pattern: 3-layer isolation for multi-agent workspaces
From [@Distroux](https://x.com/Distroux): split shared state into (1) append-only run log, (2) human-owned frozen spec, (3) disposable scratchpad per agent. Agents file PRs to change the spec, never edit directly. Prevents state corruption when multiple agents share a workspace. Practical rule: if Claude Code and Codex rewrite the same context file, you have state corruption, not coordination.


## Ferramentas & CLIs

### [Raindrop Workshop](https://github.com/raindrop-ai/workshop) - Local debugger for AI agents
Live-streamed traces of every token, tool call, and decision your agent makes. Claude Code reads the traces, writes evals, and fixes bugs in a self-healing loop. MIT license, 665 stars in 18 days. Works with Vercel AI SDK, OpenAI Agents SDK, Anthropic SDK, LangChain, CrewAI, Mastra, and more. Run `/instrument-agent` and traces start flowing.

