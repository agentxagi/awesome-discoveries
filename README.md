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

#
### [Forge](https://github.com/antoinezambelli/forge) - Reliability guardrails for local model agents
Lifts 8B local models to 86.5% on multi-step agentic evals. Rescue parsing catches bad tool calls, step enforcement prevents skipped steps, VRAM-aware budgets compact context before OOM. Three modes: full WorkflowRunner, guardrails middleware for your own loop, or drop-in proxy server. 952 stars, MIT, Python. Works with Ollama, llama-server, Llamafile, Anthropic. The ablation study (N=50) shows each guardrail contributes measurably. Most agent tooling assumes frontier models. Forge assumes you're running local and handles everything that breaks.

## Agent Infrastructure
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

### [Ruflo](https://github.com/ruvnet/ruflo) - Multi-agent swarm orchestration for Claude
Agent orchestration platform for deploying coordinated Claude Code and Codex instances. Self-learning swarm intelligence with memory persistence, RAG integration, and neural coordination. 53K stars, 22M+ npm downloads, TypeScript. Formerly claude-flow. Ships plugins for Claude Code and Codex. The swarm pattern: specialized agents coordinate through shared memory and message passing. Each agent gets isolated context but can access swarm state. Active development (commits daily). The key difference from single-agent tools: Ruflo manages the coordination layer between agents, not just individual agent execution.

### [memU](https://github.com/NevaMind-AI/memU) - Memory for 24/7 proactive agents
Purpose-built for always-on agents like OpenClaw. Most agent memory targets chatbots (session context persistence). memU targets the harder problem: agents running 24/7 that need to accumulate state, learn from past runs, and maintain consistency across restarts. 13.6k stars, 1028 forks, Python. Explicitly designed for OpenClaw-compatible proactive agents. While Memori and Engram focus on coding agent memory, memU focuses on background agents that never stop. The proactive-agent memory layer is underserved — this fills it.

### [TencentDB Agent Memory](https://github.com/Tencent/TencentDB-Agent-Memory) - 4-tier memory pipeline with real benchmarks
From Tencent. Symbolic short-term memory (Mermaid symbol offloading) + 4-layer long-term memory (L0 raw → L1 facts → L2 summaries → L3 personas). Fully local, zero external dependencies. Benchmarks: 61% token reduction, +51% pass rate on WideSearch, PersonaMem accuracy 48%→76%. OpenClaw plugin, Hermes compatible. 3618 stars, MIT, TypeScript. The progressive compression pipeline is the differentiator — instead of dumping raw context into a vector DB, it distills through 4 layers. Each layer serves a different recall need: L1 for facts, L2 for summaries, L3 for accumulated user understanding.



### [Beads](https://github.com/gastownhall/beads) - Graph issue tracker for coding agents
From Steve Yegge. Replaces markdown TODO lists with a Dolt-backed SQL database. Every issue is a queryable row, dependencies are graph edges, and old tasks get semantically compacted to save context window. Hash-based IDs prevent merge collisions when multiple agents work the same codebase. Integrations for Claude Code, Codex, Cursor, Windsurf, Factory. Stealth mode for personal use on shared repos. 23.9K stars, MIT, Go, 1582 forks. The compaction feature is essentially memory decay for the issue tracker - old closed tasks get summarized instead of deleted. bd prime gives agents workflow context and persistent memories without re-reading everything.
### [agentmemory](https://github.com/rohitg00/agentmemory) - Persistent memory for coding agents with confidence scoring
Extends Karpathy LLM Wiki pattern with confidence scoring, lifecycle management, knowledge graphs, and hybrid search. MCP-native, works with Claude Code, Cursor, Gemini CLI, Codex CLI, OpenClaw out of the box. 14.3k stars, TypeScript, Apache 2.0. The design doc got 1200 stars on its own. Uses iii engine under the hood. Confidence scoring on memories means agents weigh how much to trust recalled context, not just store-and-retrieve. No vector DB required. The memory layer coding agents actually need: persistent across sessions, queryable via MCP.


## Agent Infrastructure

### [eval-view](https://github.com/hidai25/eval-view) - Regression testing for AI agents
Snapshot agent behavior, diff tool calls between runs, catch regressions in CI. Works with LangGraph, CrewAI, OpenAI, Anthropic. Python/pytest-based.


### [MCP-Universe](https://github.com/SalesforceAIResearch/MCP-Universe) - RL training and benchmarking for MCP tool-use
From Salesforce AI Research. Treats tool-use as a reinforcement learning problem - agents learn which tools to call, when, and with what parameters through reward signals. Includes standardized benchmarking environments. Apache 2.0, Python, 587 stars. 82 forks, actively maintained.

### [tau3-bench](https://github.com/sierra-research/tau2-bench) - Multimodal agent benchmark (text, voice, knowledge)
From Sierra. The tau-bench series tests the full tool-agent-user interaction loop, not just code generation. tau3 adds full-duplex voice evaluation (OpenAI, Gemini, xAI providers) and a knowledge domain with configurable RAG pipelines. Live leaderboard at taubench.com. 1206 stars, MIT. 75+ task quality fixes based on SABER analysis (Cuadron et al., 2025). Most agent benchmarks test code. tau-bench tests airline, retail, and banking domains, the interaction patterns agents actually face in production. The voice evaluation layer is new, nobody else benchmarks full-duplex voice agents systematically.
### [MCPMark](https://github.com/eval-sys/mcpmark) - Stress-testing benchmark for MCP tool-use
Evaluates agents across real MCP servers (Notion, GitHub, Filesystem, Postgres, Playwright) with isolated sandboxes and unified metrics. 419 stars, Apache 2.0, Python. Has arXiv paper (2509.24002) and HuggingFace trajectory dataset. DeepSeek v3.2 used MCPMark in their evaluation. Pinned MCP server versions for reproducibility. Leaderboard: gpt-5-high 51.6%, gemini-3-pro 50.6%, deepseek-v3.2-thinking 36.8%. Most agents fail on half the tasks — which means the benchmark measures real capability. Auto-compaction support for long evaluations. 50 easy tasks for smaller open-source models plus harder tasks for frontier. Complements MCP-Universe (RL training) in the evaluation stack.



### [ClawBench](https://github.com/reacher-z/ClawBench) - Browser agent benchmark on 153 real-world tasks
Open-source benchmark for browser AI agents across 144 live websites. Top score is 33.3% — the best agents fail on 2 out of 3 everyday web tasks. 5-layer recording (screenshot, DOM, network, console, a11y tree), DOM-match + LLM judge for scoring. Published as arXiv paper, HuggingFace Daily Paper. Dataset on HuggingFace. Most agent benchmarks test code generation; ClawBench tests the thing users actually want: navigate real websites and complete multi-step tasks. 310 stars, Apache 2.0, Python.

### [agent-belt](https://github.com/jfrog/agent-belt) - Eval framework for coding agents (JFrog)
CLI-based, runs multi-turn scenarios with rich assertions and multi-judge consensus. Works against Claude Code, Codex, Copilot, or any agent you plug in. From JFrog engineering.



### [Eval Engineer](https://github.com/Galileo-Agent-Labs/eval-engineer) - Eval skill bundle for Claude Code and Codex
Open-source skill bundle from Galileo that turns coding agents into eval engineers. Install into a project and Claude Code gets /eval-diagnose, /eval-cost, /eval-audit as slash commands. Codex gets the same as dollar-mentions. The flow: fetch Galileo traces, build a debug packet, run RCA on spans and metrics, make one bounded change, verify the next run improved. MIT, Python. Not a dashboard - an agent skill that knows which artifact to inspect, which metric matters, and whether the fix belongs in the prompt, tool schema, retriever, or config.

### [Plano](https://github.com/katanemo/plano) - AI-native proxy for agentic apps
Rust proxy built on Envoy that handles LLM routing, safety guardrails, rate limiting, and cost tracking between your agents and model providers. 6.4k stars. Most teams build this ad-hoc as middleware; Plano gives you a drop-in data plane. The "Envoy for agents" pattern.

### [Cozeloop](https://github.com/coze-dev/coze-loop) - Full-lifecycle agent optimization
Dev, debug, eval, and monitor agents from a single Go platform. 5.4k stars from ByteDance's Coze team. Most tools do eval or observability. Cozeloop does both plus prompt management and a playground for rapid iteration. Closes the feedback loop between monitoring and improvement.


### [Laminar](https://github.com/lmnr-ai/lmnr) - Open-source agent observability (YC S24)
OpenTelemetry-native observability platform built in Rust. 1 line of code to trace Vercel AI SDK, LangChain, OpenAI, Anthropic, Gemini, Browser Use. Traces + evals + monitoring + SQL access to all data. Self-hostable via Docker compose. The Rust core handles high-throughput agent traces. The monitoring layer uses natural language event definitions — not metric thresholds. 2917 stars, Apache 2.0. Compared to Langfuse (Python-based), Laminar is Rust-native and OpenTelemetry-first. If you're running agents in production and need to know what they're doing, this is the stack.

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

### [Infisical Agent Vault](https://github.com/Infisical/agent-vault) - HTTP credential proxy for AI agents
From Infisical (established secrets management platform). Go-based HTTP proxy that intercepts outbound requests and injects credentials so agents never touch raw secrets. 1232 stars, works with Claude Code, OpenClaw, Hermes, and custom agents. The proxy pattern complements OneCLI (CLI token vending) and LiteLLM (TLS proxy) — three approaches to the same problem. Agent Vault sits at the HTTP layer: any agent making outbound API calls gets creds injected transparently. 11 open issues, active development. If you run agents that call external APIs, you need one of these three tools.



### [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit) - Runtime policy enforcement for AI agents
From Microsoft. Every tool call, resource access, and inter-agent message evaluated against policy before execution — deterministic, sub-millisecond, auditable. Covers 10/10 OWASP Agentic Top 10. Multi-language SDKs (Python, TypeScript, .NET, Rust, Go). The benchmark says it all: prompt-based safety has 26.67% policy violation rate in red-team testing; application-layer enforcement: 0.00%. Policy as code — define rules declaratively, evaluate before every action. Works with LangChain, CrewAI, AutoGen, OpenAI Agents, Google ADK, Semantic Kernel, AWS Bedrock, 20+ more. 1596 stars, 308 forks, MIT, pushed today. OpenSSF certified. The governance layer production agents need before they touch real systems.

### [OpenViking](https://github.com/volcengine/OpenViking) - Context database for AI agents
From ByteDance/Volcengine. Unifies memory, resources, and skills under a filesystem paradigm instead of fragmented vector storage. Three-tier loading (L0 raw → L1 structured → L2 summaries) loads context on demand instead of dumping everything. Directory recursive retrieval combines directory positioning with semantic search. Retrieval trajectories are visible and debuggable — you can see why the agent fetched what it fetched. Auto session management compresses conversations and extracts long-term memory. Rust CLI + Python package. 24.2K stars, AGPL, 1815 forks, active since Jan 2026. The filesystem metaphor is genuinely different from TencentDB (progressive compression) and Memori (structured state): OpenViking treats all agent context as files in a hierarchy, making it queryable, observable, and tiered by default.
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

### [Obsidian Mind](https://github.com/breferrari/obsidian-mind) - Obsidian vault as persistent agent memory
Uses Obsidian's graph view, backlinks, and search as the memory interface for coding agents. Agents write structured markdown notes; humans browse and curate in the same vault. The bidirectional flow matters: agents accumulate knowledge during sessions, humans correct it in Obsidian, agents read back the corrections on next run. Works with Claude Code, Codex CLI, Gemini CLI. 2592 stars, MIT, TypeScript, 327 forks. Part of the memory-as-filesystem pattern but with a polished UI layer. If you already use Obsidian, this turns your existing workflow into agent memory.

### [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) - Browser debugging for AI agents via MCP
From Google. Lets coding agents (Claude, Cursor, Codex, Gemini) control and inspect a live Chrome browser through MCP. Performance traces, network requests, screenshots, source-mapped console errors. Uses Puppeteer for reliable automation. 40K stars, npm package, MIT. The missing link between coding agents and real browser debugging. Your agent records a trace, reads the network waterfall, checks console errors with source-mapped stack traces. Also ships a CLI for non-MCP use.

