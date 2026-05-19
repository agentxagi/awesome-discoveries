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

#### [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Production playbook for LLM-powered software
21k stars. The core thesis: effective agents are software with LLM steps placed strategically, not prompt + tools + loop until done. Own your prompts, typed tool structures, human-in-the-loop as first-class, small focused agents over monoliths, stateless reducer pattern. The fastest path is incorporating modular agent concepts into existing products, not greenfield framework rewrites.

### Google Antigravity 2.0 - Multi-agent orchestration platform (Google I/O 2026)
Standalone desktop app, CLI, SDK, and voice interface for commanding agent teams. Gemini 3.5 Flash runs 12x faster within the framework. Already has ecosystem growing around it (opencode-antigravity-auth at 10k stars, VS Code quota extensions, skill collections). Early research preview, globally available.

## Agent Infrastructure
> Monitoring, reliability, security, cost management, testing


### [Lapdog](https://lapdog.datadoghq.com/) - Local agent tracer from Datadog
Runs fully local, no account required. Traces reasoning and tool calls from Codex, Claude Code, and Pi in real time. The first usable agent observability tool from a major vendor. Free. 70 likes in hours on launch. Fills the gap between reading terminal output blind and paying for Datadog cloud.

### Cloudflare + Claude Managed Agents - Isolated sandboxed execution for autonomous code delivery
Cloudflare integrates with Anthropic's Claude Managed Agents for edge-scale isolated execution. Bounded blast radius, controlled access to private backends, custom runtimes per agent. 363 likes, 35k views. The pattern is consolidating: Cloudflare, Vercel, and Google all shipped sandbox integrations in the same week. Cloud providers own the sandbox, model providers own the agent runtime.


### Ferramentas & CLIs
> Ferramentas de desenvolvimento, debugging, deploy

---

## Agents & Frameworks

### [skillgrade](https://github.com/mgechev/skillgrade) - Unit tests for agent skills
Run assertions against agent skill outputs the same way you would test code. From Minko Gechev (Angular team lead). TypeScript, MIT license, 480+ stars. The unit test metaphor maps cleanly to agent skills.

### [agent-skills-eval](https://github.com/darkrishabh/agent-skills-eval) - Test runner for agentskills.io skills
YAML-based scenarios with LLM judges. 500+ stars in two weeks. TypeScript, works with any OpenAI-compatible API.

### [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) - Production playbook for LLM-powered software
21k stars. The core thesis: effective agents are software with LLM steps placed strategically, not prompt + tools + loop until done. Own your prompts, typed tool structures, human-in-the-loop as first-class, small focused agents over monoliths, stateless reducer pattern. The fastest path is incorporating modular agent concepts into existing products, not greenfield framework rewrites.

### Google Antigravity 2.0 - Multi-agent orchestration platform (Google I/O 2026)
Standalone desktop app, CLI, SDK, and voice interface for commanding agent teams. Gemini 3.5 Flash runs 12x faster within the framework. Already has ecosystem growing around it (opencode-antigravity-auth at 10k stars, VS Code quota extensions, skill collections). Early research preview, globally available.

## Agent Infrastructure

### [eval-view](https://github.com/hidai25/eval-view) - Regression testing for AI agents
Snapshot agent behavior, diff tool calls between runs, catch regressions in CI. Works with LangGraph, CrewAI, OpenAI, Anthropic. Python/pytest-based.

### [agent-belt](https://github.com/jfrog/agent-belt) - Eval framework for coding agents (JFrog)
CLI-based, runs multi-turn scenarios with rich assertions and multi-judge consensus. Works against Claude Code, Codex, Copilot, or any agent you plug in. From JFrog engineering.


### [Context7](https://github.com/upstash/context7) - Fresh documentation for LLMs and coding agents
55k stars, MIT. Solves the stale-doc problem: every coding agent guesses APIs from training data that's months old. Context7 injects up-to-date documentation at query time via MCP server. Works with Claude Code, Cursor, Windsurf, Codex. Built by Upstash. The "documentation as context" pattern fills a real infra gap — agent reliability depends on accurate API knowledge, not memorized guesses.

---

## LLM & RAG

### [claude-mem](https://github.com/thedotmack/claude-mem) - Persistent context across sessions for coding agents
Captures everything your agent does during a session, compresses it with AI, and injects relevant context into future sessions. Works with Claude Code, OpenClaw, Codex, Gemini, Hermes, Copilot. SQLite + ChromaDB + embeddings. 76k stars, v13.2, actively maintained. The agent that remembers what it did yesterday problem, solved.

## Multi-Agent Systems

### Orchestration & Coordination

### [contrabass](https://github.com/junhoyeo/contrabass) - Project-level orchestrator for AI coding agents
Go + Charm TUI implementation of OpenAI's Symphony SPEC.md. Coordinates multiple coding agents (Codex, Claude Code) from a single interface. 151 stars, Go binary, actively maintained. The "one orchestrator, many coding CLIs" pattern.

### OpenAI Symphony SPEC.md - Standard for autonomous coding agent orchestration
OpenAI open-sourced a SPEC.md defining how coding agents should be orchestrated: issue intake, agent spawning, artifact management. Already spawning implementations (contrabass, symphony forks). Think of it as docker-compose for coding agents. [InfoQ coverage](https://www.infoq.com/news/2026/05/openai-symphony-agents/).


### [TraceFix](https://ortiz.rutgers.edu/projects/tracefix/) - TLA+-based protocol repair for multi-agent coordination
Uses TLA+ counterexamples to find and repair coordination protocol violations before deployment. Formal methods meet agent orchestration. CAISconf 2026 paper from Rutgers (Jorge Ortiz et al.). Instead of discovering protocol failures in production, catch them at design time.

### [Ruflo](https://github.com/ruvnet/ruflo) - Agent orchestration platform for Claude
53k stars. Deploy multi-agent workflows with a visual builder and structured output routing. TypeScript, built specifically for the Claude ecosystem (Claude Code, OpenClaw native support). The shift from generic orchestration to framework-specific orchestration layers is a signal worth watching.


### Memory architecture pattern: 3-layer isolation for multi-agent workspaces
From [@Distroux](https://x.com/Distroux): split shared state into (1) append-only run log, (2) human-owned frozen spec, (3) disposable scratchpad per agent. Agents file PRs to change the spec, never edit directly. Prevents state corruption when multiple agents share a workspace. Practical rule: if Claude Code and Codex rewrite the same context file, you have state corruption, not coordination.


## Ferramentas & CLIs

### [Raindrop Workshop](https://github.com/raindrop-ai/workshop) - Local debugger for AI agents
Live-streamed traces of every token, tool call, and decision your agent makes. Claude Code reads the traces, writes evals, and fixes bugs in a self-healing loop. MIT license, 665 stars in 18 days. Works with Vercel AI SDK, OpenAI Agents SDK, Anthropic SDK, LangChain, CrewAI, Mastra, and more. Run `/instrument-agent` and traces start flowing.

### [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) - Browser debugging for coding agents
40k stars, Apache 2.0, official Google project. Exposes Chrome DevTools as an MCP server — agents can inspect DOM, read console errors, profile performance, set breakpoints through structured tool calls. No more screenshot-guessing for frontend debugging. The first serious bridge between browser devtools and agent workflows.

