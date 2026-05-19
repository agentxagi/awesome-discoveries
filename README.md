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


## Ferramentas & CLIs

*Nenhum item ainda.*
