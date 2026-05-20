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

### [Memori](https://github.com/MemoriLabs/Memori) - Agent-native memory infrastructure
LLM-agnostic layer that turns agent execution and conversation into structured, persistent state. 14.6k stars, Python, 2200 forks. Different from session-context tools (claude-mem): Memori captures execution traces, decisions, and conversation turns, then compresses them into retrievable memory any LLM can query. The agent-memory problem has two layers - short-term context (solved by bigger windows) and long-term structured recall (still unsolved). Memori targets the second. Production agents need to remember what happened across sessions without re-reading full transcripts.

### [CUA](https://github.com/trycua/cua) - Cross-platform Computer Use Agent infrastructure
Open-source stack for agents that control full desktops across macOS, Linux, and Windows. Ships sandboxes, SDKs, and eval benchmarks together. 16.9k stars, MIT, 1069 forks. Most agent frameworks stop at the browser. CUA goes to the OS level: window management, file operations, app control across all three platforms. Active commits (last push today). While browser-use (94k stars) owns the web layer, CUA owns the desktop layer. 307 open issues = real community, not a trophy repo.



### [NanoClaw](https://github.com/nanocoai/nanoclaw) - Container-first OpenClaw alternative
Lightweight alternative that runs agents in isolated containers by default. Connects to WhatsApp, Telegram, Slack, Discord, Gmail. Built on Anthropic Agents SDK directly. 29K stars, MIT, TypeScript, 12.8K forks. Container isolation is not optional - every agent gets its own sandbox without config.



### [IronClaw](https://github.com/nearai/ironclaw) - Privacy-first Agent OS in Rust
Agents run in WASM sandboxes with explicit permission boundaries. Memory-safe runtime handling credentials and tool execution. CodeAct + RLM patterns built in. 12.3K stars, Apache 2.0, Rust. The WASM plugin model means third-party extensions cannot escape their sandbox.




### [DeepAgents](https://github.com/langchain-ai/deepagents) - Batteries-included agent harness from LangChain
Opinionated agent harness built on LangGraph with planning, sub-agents, filesystem operations, context management, persistent memory, skills, shell access, and MCP tool support out of the box. Model-agnostic, works with any LLM that supports tool calling. 23K stars, MIT, Python + TypeScript. The key difference from raw LangGraph: everything a production agent needs is bundled and tunable. Sub-agents get isolated context windows. Filesystem backend is pluggable (local, sandboxed, remote). The Deep Agents Code CLI is their terminal coding agent, powered by any model. 160 open issues, active community. The layers compose: LangGraph for custom graphs, LangChain create_agent for lightweight harness, DeepAgents for the full package.

### [memU](https://github.com/NevaMind-AI/memU) - Memory for 24/7 proactive agents
Purpose-built for always-on agents like OpenClaw. Most agent memory targets chatbots (session context persistence). memU targets the harder problem: agents running 24/7 that need to accumulate state, learn from past runs, and maintain consistency across restarts. 13.6k stars, 1028 forks, Python. Explicitly designed for OpenClaw-compatible proactive agents. While Memori and Engram focus on coding agent memory, memU focuses on background agents that never stop. The proactive-agent memory layer is underserved — this fills it.

### [agentmemory](https://github.com/rohitg00/agentmemory) - Persistent memory for coding agents with confidence scoring
Extends Karpathy LLM Wiki pattern with confidence scoring, lifecycle management, knowledge graphs, and hybrid search. MCP-native, works with Claude Code, Cursor, Gemini CLI, Codex CLI, OpenClaw out of the box. 14.3k stars, TypeScript, Apache 2.0. The design doc got 1200 stars on its own. Uses iii engine under the hood. Confidence scoring on memories means agents weigh how much to trust recalled context, not just store-and-retrieve. No vector DB required. The memory layer coding agents actually need: persistent across sessions, queryable via MCP.


## Agent Infrastructure

### [eval-view](https://github.com/hidai25/eval-view) - Regression testing for AI agents
Snapshot agent behavior, diff tool calls between runs, catch regressions in CI. Works with LangGraph, CrewAI, OpenAI, Anthropic. Python/pytest-based.


### [MCP-Universe](https://github.com/SalesforceAIResearch/MCP-Universe) - RL training and benchmarking for MCP tool-use
From Salesforce AI Research. Treats tool-use as a reinforcement learning problem - agents learn which tools to call, when, and with what parameters through reward signals. Includes standardized benchmarking environments. Apache 2.0, Python, 587 stars. 82 forks, actively maintained.

### [tau3-bench](https://github.com/sierra-research/tau2-bench) - Multimodal agent benchmark (text, voice, knowledge)
From Sierra. The tau-bench series tests the full tool-agent-user interaction loop, not just code generation. tau3 adds full-duplex voice evaluation (OpenAI, Gemini, xAI providers) and a knowledge domain with configurable RAG pipelines. Live leaderboard at taubench.com. 1206 stars, MIT. 75+ task quality fixes based on SABER analysis (Cuadron et al., 2025). Most agent benchmarks test code. tau-bench tests airline, retail, and banking domains, the interaction patterns agents actually face in production. The voice evaluation layer is new, nobody else benchmarks full-duplex voice agents systematically.

### [agent-belt](https://github.com/jfrog/agent-belt) - Eval framework for coding agents (JFrog)
CLI-based, runs multi-turn scenarios with rich assertions and multi-judge consensus. Works against Claude Code, Codex, Copilot, or any agent you plug in. From JFrog engineering.



### [Eval Engineer](https://github.com/Galileo-Agent-Labs/eval-engineer) - Eval skill bundle for Claude Code and Codex
Open-source skill bundle from Galileo that turns coding agents into eval engineers. Install into a project and Claude Code gets /eval-diagnose, /eval-cost, /eval-audit as slash commands. Codex gets the same as dollar-mentions. The flow: fetch Galileo traces, build a debug packet, run RCA on spans and metrics, make one bounded change, verify the next run improved. MIT, Python. Not a dashboard - an agent skill that knows which artifact to inspect, which metric matters, and whether the fix belongs in the prompt, tool schema, retriever, or config.

### [Plano](https://github.com/katanemo/plano) - AI-native proxy for agentic apps
Rust proxy built on Envoy that handles LLM routing, safety guardrails, rate limiting, and cost tracking between your agents and model providers. 6.4k stars. Most teams build this ad-hoc as middleware; Plano gives you a drop-in data plane. The "Envoy for agents" pattern.

### [Cozeloop](https://github.com/coze-dev/coze-loop) - Full-lifecycle agent optimization
Dev, debug, eval, and monitor agents from a single Go platform. 5.4k stars from ByteDance's Coze team. Most tools do eval or observability. Cozeloop does both plus prompt management and a playground for rapid iteration. Closes the feedback loop between monitoring and improvement.

### [CubeSandbox](https://github.com/TencentCloud/CubeSandbox) - Hardware-isolated sandbox for AI agents
From Tencent Cloud. Not containers — KVM micro-VMs via RustVMM for hardware-level isolation. Boots in <60ms, uses <5MB per instance, 2000+ concurrent sandboxes on a single node. E2B SDK compatible. Rust, Apache 2.0, 5.8k stars in 6 weeks. Most agent sandboxes use Docker + seccomp. CubeSandbox uses virtualization, which is fundamentally harder to escape. The security layer production agents need.

### [OpenSandbox](https://github.com/alibaba/OpenSandbox) - Extensible sandbox runtime for AI agents (Alibaba)
10.7k stars, Apache 2.0, Python. Plugin-based isolation architecture — custom policies for resource limits, network restrictions, and execution boundaries. The agent sandbox space is consolidating: CubeSandbox (Tencent, KVM micro-VMs), OpenSandbox (Alibaba, plugins), microsandbox (Rust, local-first), Sandcastle (TypeScript, multi-provider). OpenSandbox's angle is extensibility over raw isolation. Active commits.

### [microsandbox](https://github.com/superradcompany/microsandbox) - Local-first programmable sandboxes for AI agents
6.1k stars, Rust, Apache 2.0. Runs entirely on your machine, no cloud dependency. Most agent sandboxes assume cloud infra (E2B, CubeSandbox, Modal). microsandbox targets dev teams with data sovereignty constraints or offline requirements. Rust core = small footprint, fast spin-up. The "run agents locally but safely" pattern fills a gap the cloud-first sandboxes leave open.



### [Varlock](https://github.com/dmno-dev/varlock) - AI-safe .env files
Splits config into schema definitions (agents can read) and secret values (humans only). Agents understand the configuration surface without ever touching credentials. 3.4K stars, MIT, TypeScript.

### [LiteLLM Agent Platform](https://github.com/BerriAI/litellm-agent-platform) - Self-hosted agent sandboxing with credential vault
From the LiteLLM team (20k+ stars on their LLM proxy). Agents run in isolated Kubernetes pods with a vault proxy that swaps stub credentials for real ones on every outbound TLS call. The vault is the key insight: agents get bypass-permissions without ever seeing actual keys. Supports Claude Code, Codex, Hermes. Uses kubernetes-sigs/agent-sandbox CRDs. Most sandboxing solutions handle isolation; this one handles the harder problem of credential management inside the sandbox. MIT, TypeScript, 438 stars.

### [OneCLI](https://github.com/onecli/onecli) - Open-source credential vault for AI agents
Agents access services without ever seeing real keys. CLI vault model that vends short-lived session tokens instead of raw secrets. MCP-compatible, works with OpenClaw and Hermes. TypeScript + Rust, Apache 2.0, 2.2k stars. The credential management problem is agent infra's biggest unsolved gap — most teams put API keys in env vars and hope. OneCLI intercepts at the tool layer. Complements LiteLLM's vault proxy (TLS interception) with a CLI-level token vending model. Together they represent a new infra layer: credential management purpose-built for agents.


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


### [Open Multi-Agent](https://github.com/open-multi-agent/open-multi-agent) - Goal-to-DAG orchestration with 3 runtime dependencies
TypeScript-native. You describe a goal, it generates a task DAG automatically. Three runtime dependencies total in a space where most frameworks pull in hundreds. Model-agnostic (Claude, Gemini, OpenAI, DeepSeek, Ollama). Built-in MCP support and live tracing. 6.2k stars, MIT, created March 2026. The minimal-dependency approach matters: less surface area, faster audits, fewer supply chain risks.

### Memory architecture pattern: 3-layer isolation for multi-agent workspaces
From [@Distroux](https://x.com/Distroux): split shared state into (1) append-only run log, (2) human-owned frozen spec, (3) disposable scratchpad per agent. Agents file PRs to change the spec, never edit directly. Prevents state corruption when multiple agents share a workspace. Practical rule: if Claude Code and Codex rewrite the same context file, you have state corruption, not coordination.

### [Sandcastle](https://github.com/mattpocock/sandcastle) - Sandboxed coding agent orchestration
From Matt Pocock. `sandcastle.run()` spins up an isolated agent in Docker, Podman, or Vercel Firecracker microVMs. Provider-agnostic, handles branch isolation and merge-back automatically. 4.6k stars, MIT, 483 forks. Agent orchestration needs sandboxing as a first-class concern. You invoke the agent, Sandcastle handles the blast radius.


### [DeerFlow](https://github.com/bytedance/deer-flow) - Long-horizon SuperAgent by ByteDance
Researches, codes, and creates across tasks that take minutes to hours. Architecture: sandboxes, persistent memories, tools, skills, subagents, and a message gateway. 68K+ stars, Python, actively maintained by ByteDance. Most agent frameworks handle single-turn or short chains. DeerFlow is built for multi-hour autonomous workflows with checkpoint/resume. The SuperAgent pattern — one orchestrator delegating to specialized subagents with shared memory and sandboxed execution.



## Ferramentas & CLIs

### [Raindrop Workshop](https://github.com/raindrop-ai/workshop) - Local debugger for AI agents
Live-streamed traces of every token, tool call, and decision your agent makes. Claude Code reads the traces, writes evals, and fixes bugs in a self-healing loop. MIT license, 674 stars in 19 days. Works with Vercel AI SDK, OpenAI Agents SDK, Anthropic SDK, LangChain, CrewAI, Mastra, and more. Run `/instrument-agent` and traces start flowing.

### [Context Mode](https://github.com/mksglu/context-mode) - Context window optimization for coding agents
Intercepts and compresses tool output before it hits the model. Claims 98% reduction in context usage across 15 platforms (Claude Code, Cursor, Windsurf, Codex, etc). 15k stars. #1 on Hacker News with 570+ points. Used at Microsoft, Google, Meta. The context budget problem is one of the main costs in production agents — every wasted token on npm install logs and test output is money. TypeScript, ELv2 license.

### [Engram](https://github.com/Gentleman-Programming/engram) - Persistent memory for coding agents via MCP
Agent-agnostic Go binary with SQLite + FTS5. Exposes persistent memory through MCP - coding agents get recall of past decisions without a vector DB or Redis. 3.6k stars, MIT, single binary deploy. The MCP-native approach means adding memory is one config line, not infrastructure. SQLite is the right tradeoff for coding agents: you need exact recall of past decisions, not semantic similarity. Includes HTTP API, CLI, and TUI for manual inspection.

### [ZeroLang](https://github.com/vercel-labs/zerolang) - Agent-first programming language
From Vercel Labs. What if the primary consumer of a programming language isn't a human but an AI agent? Zero explores this: structured JSON diagnostics that agents can parse, error repair codes, sub-16KB static binaries, explicit capabilities, and a syntax designed to be learned on the fly from examples and compiler feedback. Written in C, Apache 2.0. 3.4k stars in 5 days. Pre-1.0 and intentionally unstable — but the concept shifts how we think about the agent-tooling interface. If agents write code, shouldn't the language be designed for them?

### [audit](https://github.com/evilsocket/audit) - 8-stage vulnerability discovery agent
From evilsocket (bettercap creator). Reimplements Cloudflare's Project Glasswing pipeline: 8 narrow stages (recon, hunt, validate, gapfill, dedupe, trace, feedback, report) instead of one big "find bugs" prompt. The key insight: a second agent on a different model tries to disprove every finding, and a reachability trace gates whether attacker input can actually reach the sink. Built on Claude Code Agent SDK, uses subscription billing (not metered API). 308 stars, MIT, 2 days old. Real security tooling from a known security researcher.

### [SmallCode](https://github.com/Doorman11991/smallcode) - Coding agent for small local models (7B-20B)
Terminal-native agent that compensates for small model limitations instead of assuming frontier hardware. Budget-managed context, forgiving multi-format tool-call parser, TODO-file decomposed planning, search-and-replace patches instead of full file rewrites. 87% benchmark with 4B-active model. RTK (Rust Token Killer) rewrites bash commands for 60-90% token savings. Works with Ollama, LM Studio, any OpenAI-compatible endpoint. 746 stars in 2 days, MIT, JavaScript. Most coding agents target Claude/GPT-5. SmallCode targets the other end: a Mac Mini running a 7B model that can still ship real code.
