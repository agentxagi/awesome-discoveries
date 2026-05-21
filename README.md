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


### [Pi Agent Harness](https://github.com/earendil-works/pi) - Self-extensible coding agent with supply-chain hardening
Mono-repo architecture: unified multi-provider LLM API (OpenAI/Anthropic/Google), agent runtime with tool calling + state management, interactive coding agent CLI, terminal UI with differential rendering. 52K stars, 6235 forks, MIT, TypeScript. What sets pi apart is supply-chain hardening: direct deps pinned to exact versions, npm audit with signature verification, shrinkwrap for transitive deps, pre-commit hooks blocking accidental lockfile changes, and a 2-day minimum release age for new npm packages. OSS session sharing to HuggingFace for real-world agent benchmarking. The unified LLM API layer is provider-agnostic.

### [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) - Official lightweight multi-agent framework from OpenAI
Provider-agnostic SDK supporting 100+ LLMs. Sandbox Agents run work in containers over long horizons. Guardrails for input/output validation. Built-in tracing UI, human-in-the-loop, session management, and realtime voice agents with gpt-realtime-2. 26K stars, 4072 forks, MIT, Python. OpenAI SDK-level answer to CrewAI and LangGraph. Notably provider-agnostic, not locked to OpenAI models. The sandbox agent pattern pairs well with CubeSandbox and microsandbox.

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




### [ClawGUI](https://github.com/ZJU-REAL/ClawGUI) - RL training + eval + deploy for GUI agents
Full-stack framework from Zhejiang University. Online RL training for GUI agents, standardized benchmarks, and real-device deployment in one package. ArXiv paper (2604.11784), HuggingFace Daily Paper. Ships a trained 2B model (ClawGUI-2B). Controls real phones via natural language. Most GUI agent work is eval-only. ClawGUI is the only one doing RL training — training a small model through reinforcement learning to get good at GUI interaction, instead of just prompting a frontier model. 1257 stars, Apache 2.0, Python. Complements CUA (desktop agents) and ClawBench (browser agent eval).

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



### [ECC](https://github.com/affaan-m/ECC) - Harness-native operator system for coding agents
Anthropic hackathon winner. Skills, instincts, memory optimization, security scanning, and research-first development across Claude Code, Codex, Cursor, Gemini, Zed, and GitHub Copilot. 187K stars, MIT, 170+ contributors, 12+ language ecosystems. Not configs — a portable skill/memory layer that works across all major coding agent harnesses. v2.0 adds pub/sub for inter-agent communication. The key insight: treat the agent harness as a platform, build skills that travel across tools.


### [Beads](https://github.com/gastownhall/beads) - Graph issue tracker for coding agents
From Steve Yegge. Replaces markdown TODO lists with a Dolt-backed SQL database. Every issue is a queryable row, dependencies are graph edges, and old tasks get semantically compacted to save context window. Hash-based IDs prevent merge collisions when multiple agents work the same codebase. Integrations for Claude Code, Codex, Cursor, Windsurf, Factory. Stealth mode for personal use on shared repos. 23.9K stars, MIT, Go, 1582 forks. The compaction feature is essentially memory decay for the issue tracker - old closed tasks get summarized instead of deleted. bd prime gives agents workflow context and persistent memories without re-reading everything.
### [agentmemory](https://github.com/rohitg00/agentmemory) - Persistent memory for coding agents with confidence scoring

### [Acontext](https://github.com/memodb-io/Acontext) - Agent skills as a memory layer
Captures learnings from agent runs as plain markdown skill files. No embeddings, no vector DBs, no API lock-in. "Skill is Memory, Memory is Skill" — skills are files you can read, edit, version with git, share across agents and frameworks. 3.3K stars, Apache 2.0, JavaScript. Self-evolving skills that grow from agent mistakes and successes. Works with LangGraph, Claude, AI SDK, anything that reads files. The polar opposite of opaque vector memory: everything is inspectable.
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




### [PinchBench](https://github.com/pinchbench/skill) - Real-world OpenClaw coding agent benchmark
53 tasks measuring whether agents actually get things done — scheduling meetings, writing code, triaging email, researching topics, managing files. From Kilo.ai. Public leaderboard at pinchbench.com. 1186 stars, MIT, 132 forks. Most evals measure process quality (did the model use the right tool?). PinchBench measures outcomes (did the meeting actually get scheduled?). OpenRouter model routing for easy comparison. Complements Claw-Eval (human-verified Pass^3) and MCPMark (MCP tool-use stress test) by testing the end-to-end angle that matters in production.

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

### [HolmesGPT](https://github.com/HolmesGPT/holmesgpt) - CNCF Sandbox SRE Agent for production incidents
CNCF Sandbox project originally from Robusta.Dev, with major contributions from Microsoft. Investigates production incidents by querying live observability data from 30+ sources (Kubernetes, Prometheus, Grafana, Datadog, AWS, GCP, Azure, Jira, PagerDuty, Kafka, MongoDB, Elasticsearch). Operator Mode runs 24/7 in Kubernetes, catches problems before customers notice, sends Slack messages with root cause analysis, and can open GitHub PRs to fix what it finds. Petabyte-scale data with server-side filtering. Read-only by design, respects RBAC. 2460 stars, Apache 2.0, Python. v0.30.1 released today. While most agent infra focuses on coding or workflow, HolmesGPT fills the SRE gap: automated incident triage, root cause analysis, and remediation. The first CNCF sandbox project for AI-powered incident response.


### [Kubeshark](https://github.com/kubeshark/kubeshark) - eBPF network observability for K8s, queryable by AI agents via MCP
eBPF-powered network capture at kernel level with near-zero overhead. Indexes L4/L7 traffic with full Kubernetes context (pod, service, namespace). Decrypts TLS without private keys — agents see actual HTTP traffic inside encrypted connections. MCP server exposes network queries to any agent. The MCP angle is the differentiator: instead of humans reading pcap files, AI agents query live network traffic directly. 11.9K stars, Apache 2.0, Go, 541 forks, 143 open issues. Collapses network capture (tcpdump), TLS inspection (service mesh sidecars), and K8s context (kubectl) into one MCP-callable surface. The network evidence layer that agent-driven SRE workflows need.
### [OpenSRE](https://github.com/Tracer-Cloud/opensre) - RL training environment for AI SRE agents
The SWE-bench equivalent for production incident response. Open-source framework that builds scored synthetic RCA suites (root-cause accuracy, required evidence, adversarial red herrings) and real-world end-to-end tests across Kubernetes, EC2, CloudWatch, Lambda, ECS Fargate, and Flink. Agents train through reinforcement learning on realistic production failure scenarios with noise, time pressure, and distractors. 5.5K stars, Apache 2.0, Python, 696 forks, 166 open issues. The comparison to HolmesGPT is direct: HolmesGPT is a specific SRE agent. OpenSRE is the training ground and evaluation framework that any SRE agent can use to improve. The RL environment angle matters — most agent evals test single-turn accuracy. OpenSRE tests multi-step investigation under realistic conditions.

### [OpenViking](https://github.com/volcengine/OpenViking) - Context database for AI agents
From ByteDance/Volcengine. Unifies memory, resources, and skills under a filesystem paradigm instead of fragmented vector storage. Three-tier loading (L0 raw → L1 structured → L2 summaries) loads context on demand instead of dumping everything. Directory recursive retrieval combines directory positioning with semantic search. Retrieval trajectories are visible and debuggable — you can see why the agent fetched what it fetched. Auto session management compresses conversations and extracts long-term memory. Rust CLI + Python package. 24.2K stars, AGPL, 1815 forks, active since Jan 2026. The filesystem metaphor is genuinely different from TencentDB (progressive compression) and Memori (structured state): OpenViking treats all agent context as files in a hierarchy, making it queryable, observable, and tiered by default.

### [CozeLoop](https://github.com/coze-dev/coze-loop) - Full-lifecycle agent optimization platform
From ByteDance/Coze. Three pillars in one platform: prompt development (visual playground with multi-LLM comparison and version management), evaluation (automated multi-dimensional testing for accuracy, conciseness, compliance), and observability (full trace recording from user input to AI output including prompt parsing, model calls, tool execution, and exception capture). The shared data model across all three matters: your eval datasets reference the same prompt versions your playground tested, and your traces feed back into eval sets. Most teams cobble together separate tools for each piece. CozeLoop packages them with a unified data layer. Docker Compose or Kubernetes Helm Chart deployment. Supports OpenAI and Volcengine Ark. 5464 stars, Apache 2.0, Go, 761 forks. Created June 2025, pushed today with active daily development. Not well-known outside the Chinese developer community, but the engineering is real — the eval features (eval cron, agent eval, batch evaluation) are maturing fast.


### [ContextForge](https://github.com/IBM/mcp-context-forge) - IBM gateway, registry, and proxy for agent tool protocols
Federates MCP, A2A, REST, and gRPC APIs into one unified endpoint. Centralized governance, discovery, guardrails, TOON compression. JWT auth, Kubernetes-native. 3740 stars, 669 forks, Python. Where Plano handles the data plane, ContextForge handles the control plane: registry, discovery, policy. 1067 open issues.

### [Archestra](https://github.com/archestra-ai/archestra) - Enterprise AI platform with MCP registry, gateway, and orchestrator
Opinionated enterprise platform on top of the gateway pattern. MCP registry with access policies, rate limits, audit logging, cost management, multi-model routing. Supports A2A, ACP, MCP protocols. K8s-native, TypeScript. 3716 stars, 827 forks. Where ContextForge is protocol federation, Archestra adds the opinionated platform layer.

### [Statewright](https://github.com/statewright/statewright) - State machine guardrails for AI agents
Constrains which tools agents can use in each phase. Planning gets read-only, implementation unlocks edit tools, testing only allows test commands. 342 stars in 17 days, Rust. Instead of bigger models, make the problem smaller. Below 13GB VRAM, models can call tools but lack context for accurate edits. Statewright guardrails turn those failures into completions. Works with Claude Code, Codex, Cursor, Pi. Plugin install. Restricts the action space before the model decides, not after.

### [CUGA](https://github.com/cuga-project/cuga-agent) - Generalist agent harness for the enterprise
#1 on AppWorld benchmark, top-tier on WebArena. IBM Research. Wire your APIs and MCP servers, tune reasoning modes (fast/balanced/accurate), govern behavior with policies. MCP, OpenAPI, LangChain tool support. 738 stars, 131 forks, Python. The start-with-a-generalist-customize pattern. Live demo on HuggingFace.

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

### [ExploitBench](https://github.com/exploitbench/exploitbench) - Progressive exploit chain benchmark for AI agents
Most agent benchmarks measure if code works. ExploitBench measures if agents can break things. Progressive difficulty ladder: find vulnerable code → trigger the bug → build exploit primitives → arbitrary code execution. First target is V8 (16 capabilities in the Chromium exploitation ladder). Drives containers through an MCP server, works with any LLM via direct provider API or OpenAI-compatible gateway. Pre-built V8 eval images on GHCR. Leaderboard at exploitbench.ai. 157 stars, MIT, Python, 6 days old. Where tau3-bench tests reliability and MCPMark tests tool-use accuracy, ExploitBench tests the full security exploit chain — the capability nobody wants agents to have but everyone needs to measure.

### [AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) - Full-stack AI red teaming platform from Tencent
Scans the entire AI deployment stack: OpenClaw configurations, agent setups, MCP servers, skills, infrastructure, and LLM jailbreak endpoints. BlackHat Arsenal EU 2025 presentation. The scanning surface is what separates it from single-layer security tools that only test prompt injection or model jailbreaks. AI-Infra-Guard knows what an OpenClaw skill is, what an MCP server looks like, and how to audit agent permissions. 3.7K stars, Apache 2.0, Python. Published on ClawHub with EdgeOne ClawScan integration. Docker images and cloud deployment. Where ExploitBench measures whether agents can break things, AI-Infra-Guard scans whether your deployment is breakable.

### [Claw-Eval](https://github.com/claw-eval/claw-eval) - Human-verified agent evaluation with Pass^3 methodology
300 human-verified tasks across 9 categories with 2,159 rubrics. The Pass^3 methodology eliminates lucky runs: a model must pass each task in 3 independent trials. arXiv paper (2604.06132). Referenced publicly by Meta (Muse Spark), Kimi K2.6, Qwen 3.6, Tencent Hunyuan, Xiaomi MiMo, Z.AI GLM-5, and Ant Ling. 590 stars, MIT, Python, HuggingFace dataset. The human-verified angle matters: most agent benchmarks use synthetic tasks or LLM-generated evaluations. Claw-Eval tests what users actually need agents to do. Complements MCPMark (MCP tool-use) and ClawBench (browser agents).


### [SmallCode](https://github.com/Doorman11991/smallcode) - Coding agent for small local models (7B-20B)
Terminal-native agent that compensates for small model limitations instead of assuming frontier hardware. Budget-managed context, forgiving multi-format tool-call parser, TODO-file decomposed planning, search-and-replace patches instead of full file rewrites. 87% benchmark with 4B-active model. RTK (Rust Token Killer) rewrites bash commands for 60-90% token savings. Works with Ollama, LM Studio, any OpenAI-compatible endpoint. 746 stars in 2 days, MIT, JavaScript. Most coding agents target Claude/GPT-5. SmallCode targets the other end: a Mac Mini running a 7B model that can still ship real code.

### [Obsidian Mind](https://github.com/breferrari/obsidian-mind) - Obsidian vault as persistent agent memory
Uses Obsidian's graph view, backlinks, and search as the memory interface for coding agents. Agents write structured markdown notes; humans browse and curate in the same vault. The bidirectional flow matters: agents accumulate knowledge during sessions, humans correct it in Obsidian, agents read back the corrections on next run. Works with Claude Code, Codex CLI, Gemini CLI. 2592 stars, MIT, TypeScript, 327 forks. Part of the memory-as-filesystem pattern but with a polished UI layer. If you already use Obsidian, this turns your existing workflow into agent memory.

### [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) - Browser debugging for AI agents via MCP
From Google. Lets coding agents (Claude, Cursor, Codex, Gemini) control and inspect a live Chrome browser through MCP. Performance traces, network requests, screenshots, source-mapped console errors. Uses Puppeteer for reliable automation. 40K stars, npm package, MIT. The missing link between coding agents and real browser debugging. Your agent records a trace, reads the network waterfall, checks console errors with source-mapped stack traces. Also ships a CLI for non-MCP use.


### [shellfirm](https://github.com/kaplanelad/shellfirm) - Safety guardrails for AI coding agents and terminal commands
Intercepts dangerous shell commands before execution. Challenge-response confirmation, blast radius detection (shows what `rm -rf ./src` would actually delete), safe alternative suggestions. MCP server integration for Claude Code and Cursor. Context-aware: harder challenges when SSH'd in, running as root, on protected branches, or in production K8s clusters. 100+ patterns across 9 ecosystems. Project policies via `.shellfirm.yaml`. 910 stars, Apache 2.0, Rust. The gap filler between AI coding agents and `rm -rf`.

### [AgentDoG](https://github.com/AI45Lab/AgentDoG) - Trajectory-level risk diagnosis for autonomous agents
Analyzes full execution traces, not just final output. Catches safety risks that emerge across multiple steps in combination. Three-axis taxonomy: Risk Source, Failure Mode, Real-World Harm. Ships trained models (4B/7B/8B based on Qwen3, Qwen2.5, Llama3.1). ATBench dataset with 500 trajectories, 1575 unique tools. Outperforms R-Judge, ASSE-Safety baselines. 470 stars, Python, arXiv paper (2601.18491). From AI45Lab (Shanghai AI Laboratory). Most agent safety tools classify the output. AgentDoG classifies the journey.

### [Memvid](https://github.com/memvid/memvid) - Single-file agent memory via video encoding

Replaces RAG pipelines with a serverless memory layer. Stores embeddings in MP4 video frames with FAISS indexing. One file, zero server, instant retrieval. 15.5K stars, Rust+Python, Apache 2.0. A legitimate alternative to Pinecone/Weaviate for agent memory where you don't want infrastructure.

### [Pipelock](https://github.com/luckyPipewrench/pipelock) - AI agent firewall with mediator-signed action receipts
Sits inline between coding agents and the network as an egress proxy. Scans MCP traffic bidirectionally (48 credential patterns, 29 injection patterns with 6-pass normalization). Generates cryptographic receipts signed outside the agent trust boundary — evidence does not depend on the agent attesting to itself. CNCF Landscape listed, OpenSSF Silver, SLSA provenance. Process containment support. Works with Claude Code, Codex, Cursor, Cline, and agent SDKs (OpenAI, Google ADK, LangGraph). 618 stars, Apache 2.0, Go. The security model most agent stacks are missing: not what the model says, but what the agent does on the network.

### [Emdash](https://github.com/generalaction/emdash) - Multi-agent dev environment with worktree isolation
Agentic Development Environment (ADE) that runs multiple coding agents in parallel, each in its own git worktree. 27 CLI providers: Claude Code, Codex, Gemini, Hermes, Cursor, Devin, Droid, Jules, Junie, Kiro, Amp, and more. Pass Linear/GitHub/Jira tickets directly. Review diffs, run tests, create PRs, see CI/CD, merge — all from one desktop app. YC W26. Apache 2.0.


### [RAMPART](https://github.com/microsoft/RAMPART) - Pytest-native safety testing for AI agents
From Microsoft. Write adversarial attack tests, benign failure tests, and harm category assertions as regular pytest cases. Announced May 20 2026 via Microsoft Security blog. OpenSSF Scorecard, PyPI package. The pytest-native approach means safety tests live alongside functional tests in CI, not in a separate security audit phase. Complements runtime tools like Pipelock and shellfirm by catching issues before deployment. MIT, Python.

### [Agent of Empires](https://github.com/njbrake/agent-of-empires) - Multi-agent session manager with TUI + web dashboard
Run Claude Code, Codex, Gemini, Cursor, and 10+ more coding agents in parallel. Each agent gets its own tmux session and git worktree. Docker sandboxing optional. TUI for terminal, web dashboard with PWA install, mobile access via QR + Tailscale Funnel. Sessions persist across reboots. Multi-repo workspaces. Rust, MIT, 2321 stars, Homebrew installable. The practical answer to running 5+ coding agents without losing track.

### [Pro Workflow](https://github.com/rohitg00/pro-workflow) - Self-correcting memory for Claude Code
Every correction becomes a permanent rule in SQLite with FTS5 search. After 50 sessions, correction rate drops near zero. Auto-research loop grows knowledge wikis overnight. 34 skills, 37 hook scripts. Works with Claude Code, Cursor, and 32+ agents via SkillKit. MIT, JavaScript, 2189 stars. Different from Acontext (skills-as-markdown) and Memori (structured state): Pro Workflow focuses on what the agent got wrong, not what it learned.
### [CodeGraph](https://github.com/colbymchenry/codegraph) - Pre-indexed code knowledge graph for coding agents
Pre-indexes symbol relationships, call graphs, and code structure so coding agents query the graph instead of scanning files with grep/glob/read. Benchmarked across 7 real codebases in 7 languages: ~35% token cost reduction, ~70% fewer tool calls. Works with Claude Code, Cursor, Codex CLI, OpenCode. 100% local, zero cloud dependency. 10.2K stars, MIT, TypeScript, 631 forks, 76 open issues. The context compression layer coding agents need — same problem Acontext and Codebase Chat tackle from different angles, but CodeGraph uses a proper graph model instead of markdown files or conversation history.

### [RTK](https://github.com/rtk-ai/rtk) - CLI proxy for LLM token compression
Intercepts LLM API calls and compresses token usage by 60-90% on common dev commands. Single Rust binary, zero dependencies, works as a transparent proxy between agents and model providers. Works with Claude Code, Codex, Cursor, and any CLI agent. 51.9K stars, Apache 2.0, 3158 forks, 976 open issues. The mechanism: intercept at the transport layer, compress what can be compressed, pass through what cannot. Pairs with CodeGraph (smarter context) — together they attack token cost from both sides: less context needed, and less tokens per context.

