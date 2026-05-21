# awesome-discoveries

Curated index of AI agent tools, frameworks, and infrastructure. Updated continuously by [@agentxagi](https://x.com/agentxagi).

## Agent Infrastructure

- [osaurus](https://github.com/osaurus-ai/osaurus) (5,477★) [Swift] (MIT) — Native macOS harness for AI agents. Any model, persistent memory, autonomous execution, cryptographic identity. Fully offline. Swift.
- [engram](https://github.com/Gentleman-Programming/engram) (3,681★) [Go] (MIT) — Persistent memory system for AI coding agents. Agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI.
- [Agent Orchestrator](https://github.com/ComposioHQ/agent-orchestrator) [TypeScript] (MIT) — Parallel coding agent orchestrator. Plans tasks, spawns agents via tmux+git worktrees, handles CI fixes, merge conflicts, and code reviews autonomously.
- [ByteRover CLI](https://github.com/campfirein/byterover-cli) [TypeScript] (NOASSERTION) — Portable memory layer for autonomous coding agents. MCP server providing persistent context across sessions. Works with Claude Code, Codex, any agent.

## Agent Memory

- [agentmemory](https://github.com/rohitg00/agentmemory) (15,516★) [TypeScript] (Apache-2.0) — Persistent memory for AI coding agents. Records session activity, compresses with AI, injects context back on next session. 4-layer memory architecture: working, episodic, semantic, procedural. 95.2% retrieval accuracy on LongMemEval-S.
- [MemOS](https://github.com/MemTensor/MemOS) (9,260★) [TypeScript] (Apache-2.0) — Self-evolving memory OS for LLM and AI agents. Hybrid retrieval (keyword + vector + graph), cross-task skill reuse, 35.24% token savings.

## Agents

- [skillgrade](https://github.com/mgechev/skillgrade) — Unit tests for agent skills — run assertions against agent skill outputs the same way you'd test code
- [agent-skills-eval](https://github.com/darkrishabh/agent-skills-eval) — Test runner for agentskills.io-style skills with YAML-based scenarios and LLM judges
- [eval-view](https://github.com/hidai25/eval-view) — Regression testing for AI agents — snapshot behavior, diff tool calls, catch regressions in CI
- [agent-belt](https://github.com/jfrog/agent-belt) — Reproducible evaluation for AI coding agents — multi-turn scenarios, rich assertions, multi-judge consensus
- [Raindrop Workshop](https://github.com/raindrop-ai/workshop) — Local debugger for AI agents — live streamed traces of every token, tool call, and decision with self-healing eval loops
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) — Engineering principles for building production-grade LLM-powered software — agents as software with LLM steps, not prompt loops
- [Context Mode](https://github.com/mksglu/context-mode) — Context window optimization for AI coding agents — sandboxes tool output, claims 98% reduction in context usage across 15 platforms
- [DeerFlow](https://github.com/bytedance/deer-flow) — Long-horizon SuperAgent by ByteDance — researches, codes, and creates with sandboxes, memories, tools, skills, subagents, and message gateway
- [Memori](https://github.com/MemoriLabs/Memori) — Agent-native memory infrastructure — LLM-agnostic layer that turns agent execution and conversation into structured, persistent state for production systems
- [Engram](https://github.com/Gentleman-Programming/engram) — Persistent memory system for AI coding agents — agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI
- [CUA (Computer Use Agents)](https://github.com/trycua/cua) — Open-source infrastructure for Computer-Use Agents — sandboxes, SDKs, and benchmarks for agents that control full desktops across macOS, Linux, and Windows
- [memU](https://github.com/NevaMind-AI/memU) — Memory system built for 24/7 proactive agents like OpenClaw — persistent, structured memory that survives across agent sessions and restarts
- [ZeroLang](https://github.com/vercel-labs/zerolang) — Agent-first programming language from Vercel Labs — designed for AI agents as primary users, with structured diagnostics, tiny static binaries, and learnable syntax
- [agentmemory](https://github.com/rohitg00/agentmemory) — Persistent memory for AI coding agents — extends Karpathy's LLM Wiki pattern with confidence scoring, lifecycle, knowledge graphs, and hybrid search
- [Raindrop Workshop](https://github.com/raindrop-ai/workshop) — Local debugger for AI agents that streams every token, tool call, and decision in realtime — then lets Claude Code read your traces, write evals, and fix what's broken
- [SmallCode](https://github.com/Doorman11991/smallcode) — Terminal-native coding agent built for small local models (7B-20B) — compensates for small model limitations with budget-managed context, forgiving tool-call parsing, TODO-file decomposed planning, and search-and-replace patches instead of full file rewrites
- [NanoClaw](https://github.com/nanocoai/nanoclaw) — Lightweight container-first alternative to OpenClaw — runs agents in isolated containers with built-in memory, scheduled jobs, and connects to WhatsApp, Telegram, Slack, Discord, Gmail
- [IronClaw](https://github.com/nearai/ironclaw) — Agent OS built in Rust focused on privacy, security, and extensibility — uses WebAssembly for sandboxed agent plugins
- [DeepAgents](https://github.com/langchain-ai/deepagents) — Batteries-included agent harness from LangChain — planning, sub-agents, filesystem, context management, persistent memory, skills, and MCP tool support built on LangGraph
- [Obsidian Mind](https://github.com/breferrari/obsidian-mind) — Obsidian vault that gives AI coding agents persistent memory — works with Claude Code, Codex CLI, Gemini CLI out of the box
- [TencentDB Agent Memory](https://github.com/Tencent/TencentDB-Agent-Memory) — 4-tier progressive memory pipeline for AI agents — symbolic short-term memory (Mermaid symbol offloading) + layered long-term memory (L0 raw → L1 facts → L2 summaries → L3 personas), fully local, zero external dependencies
- [Beads](https://github.com/gastownhall/beads) — Distributed graph issue tracker for AI coding agents — replaces markdown TODO lists with a Dolt-backed SQL database, dependency chains, memory compaction, and zero-conflict multi-agent coordination
- [Forge (antoinezambelli)](https://github.com/antoinezambelli/forge) — Reliability layer for self-hosted LLM tool-calling — lifts 8B local models to 86.5% on multi-step agentic evals through rescue parsing, retry nudges, step enforcement, and VRAM-aware context budgets
- [Ruflo](https://github.com/ruvnet/ruflo) — Agent orchestration platform for Claude — deploy multi-agent swarms with self-learning coordination, RAG, and native Claude Code/Codex integration
- [ECC](https://github.com/affaan-m/ECC) — Harness-native operator system for coding agents — skills, instincts, memory optimization, security scanning, and research-first development across Claude Code, Codex, Cursor, Gemini, and 7+ other agent harnesses
- [ClawGUI](https://github.com/ZJU-REAL/ClawGUI) — Full-stack framework for GUI agents — online RL training, standardized evaluation benchmarks, and real-device deployment in one package from Zhejiang University
- [Emdash](https://github.com/generalaction/emdash) — Agentic Development Environment (ADE) that runs multiple coding agents in parallel, each isolated in its own git worktree — supports 27 CLI agents including Claude Code, Codex, Gemini, Hermes Agent
- [ContextForge (mcp-context-forge)](https://github.com/IBM/mcp-context-forge) — IBM's open-source gateway, registry, and proxy that federates MCP, A2A, and REST/gRPC APIs into one unified endpoint with centralized governance, discovery, and guardrails
- [Statewright](https://github.com/statewright/statewright) — State machine guardrails that control which tools AI agents can use in each phase — planning gets read-only, implementation unlocks edit tools, testing only permits test commands
- [CUGA](https://github.com/cuga-project/cuga-agent) — Open-source generalist agent harness for enterprise — supports complex task execution on web and APIs, OpenAPI/MCP integrations, composable architecture, reasoning modes, and policy-aware features
- [Archestra](https://github.com/archestra-ai/archestra) — Enterprise AI platform with guardrails, MCP registry, gateway, and orchestrator — unifies agent tool access with centralized governance and cost controls
- [Agent of Empires](https://github.com/njbrake/agent-of-empires) — Session manager for parallel AI coding agents — runs Claude Code, Codex, Gemini, Cursor, and 10+ more agents in isolated tmux sessions with git worktrees, Docker sandboxing, TUI + web dashboard, and mobile access
- [Pi Agent Harness](https://github.com/earendil-works/pi) — Self-extensible coding agent CLI with unified multi-provider LLM API, agent runtime with tool calling and state management, and a terminal UI library with differential rendering
- [OpenAI Agents SDK](https://github.com/openai/openai-agents-python) — OpenAI's official lightweight multi-agent framework — provider-agnostic SDK with agents, sandbox agents, handoffs, guardrails, human-in-the-loop, sessions, tracing, and realtime voice agents
- [CodeGraph](https://github.com/colbymchenry/codegraph) — Pre-indexed code knowledge graph for coding agents — replaces expensive file-scanning with instant symbol relationship queries, cutting tokens by ~35% and tool calls by ~70%
- [OpenCowork](https://github.com/OpenCoworkAI/open-cowork) — Open-source AI agent desktop app that one-click installs Claude Code, MCP tools, and Skills with sandbox isolation and multi-model support
- [OpenHuman](https://github.com/tinyhumansai/openhuman) — Desktop-first personal AI agent with 118+ one-click OAuth integrations, Memory Tree knowledge base, and auto-fetch data sync — all local-first, Rust/Tauri
- [Nexent](https://github.com/ModelEngine-Group/nexent) — Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles — pure language input, unified tools, skills, memory, and orchestration with built-in constraints and feedback loops
- [HiClaw](https://github.com/agentscope-ai/HiClaw) — Collaborative multi-agent OS using Matrix protocol rooms for transparent human-in-the-loop coordination — Manager-Workers architecture with OpenClaw, QwenPaw, and Hermes runtimes coexisting

## Agents Frameworks

- [cc-sdd (Spec-Driven Development)](https://github.com/gotalab/cc-sdd) [TypeScript] (MIT) — Turns approved specs into long-running autonomous implementation. Minimal SDD harness with agent skills for Claude Code, Codex, Cursor, Copilot, Gemini CLI.

## Evaluation

- [MCP-Universe](https://github.com/SalesforceAIResearch/MCP-Universe) — RL training and benchmarking framework for MCP tool-use agents — lets you train agents to use tools via reinforcement learning and evaluate them on standardized benchmarks
- [Eval Engineer](https://github.com/Galileo-Agent-Labs/eval-engineer) — Open-source skill bundle that turns Claude Code and Codex into eval engineers backed by Galileo traces — inspect, diagnose, fix, and verify agent behavior through evidence
- [ClawBench](https://github.com/reacher-z/ClawBench) — Open-source benchmark for browser AI agents — 153 everyday tasks across 144 live websites with 5-layer recording, DOM-match, and LLM judge
- [MCPMark](https://github.com/eval-sys/mcpmark) — Stress-testing benchmark for MCP tool-use — evaluates agents across real MCP servers (Notion, GitHub, Filesystem, Postgres, Playwright) with isolated sandboxes and unified metrics
- [Claw-Eval](https://github.com/claw-eval/claw-eval) — Evaluation harness for autonomous agents — 300 human-verified tasks across 9 categories with Pass^3 methodology, 2159 rubrics, and public leaderboard
- [PinchBench](https://github.com/pinchbench/skill) — Real-world benchmark for OpenClaw coding agents — 53 tasks measuring tool usage, multi-step reasoning, and practical outcomes (did it actually schedule the meeting, create the file, triage the email?)

## Governance

- [Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit) — Runtime governance for AI agents — every tool call, resource access, and inter-agent message evaluated against policy before execution, deterministic, sub-millisecond, auditable

## Infrastructure

- [Cloudflare + Claude Managed Agents isolated execution](https://x.com/Cloudflare/status/2056747823907942668) — Cloudflare integrates with Anthropic's Claude Managed Agents to provide isolated sandboxed execution environments for autonomous code delivery at edge scale
- [Anthropic acquires Stainless ($300M)](https://www.infoworld.com/article/4172947/anthropic-acquires-stainless-to-strengthen-claudes-developer-tooling.html) — Anthropic acquires Stainless for $300M — the company behind every Anthropic SDK generator and MCP server tool since the early API days
- [Plano](https://github.com/katanemo/plano) — AI-native proxy and data plane for agentic apps — LLM routing, safety guardrails, orchestration, and observability in one Rust proxy
- [Cozeloop](https://github.com/coze-dev/coze-loop) — Full-lifecycle agent optimization platform — dev, debug, eval, and monitor agents from a single Go service
- [CubeSandbox](https://github.com/TencentCloud/CubeSandbox) — Hardware-isolated sandbox for AI agents built on RustVMM + KVM — boots in under 60ms, uses less than 5MB per instance
- [OpenSandbox (Alibaba)](https://github.com/alibaba/OpenSandbox) — Secure sandbox runtime for AI agents from Alibaba — extensible plugin architecture for isolation, resource limits, and policy enforcement
- [microsandbox](https://github.com/superradcompany/microsandbox) — Secure, local, programmable sandboxes for AI agents — runs entirely on your machine, no cloud dependency, Rust API
- [τ³-bench (tau-three-bench)](https://github.com/sierra-research/tau2-bench) — Multimodal benchmark for agent evaluation — now covers text, voice (full-duplex), and knowledge retrieval domains with a live leaderboard
- [LiteLLM Agent Platform](https://github.com/BerriAI/litellm-agent-platform) — Self-hosted platform for running coding agents in isolated sandboxes with a credential vault — agents get stub keys, vault swaps them for real ones on every outbound TLS call
- [Laminar](https://github.com/lmnr-ai/lmnr) — Open-source observability platform purpose-built for AI agents — traces, evals, monitoring, SQL access to all data, written in Rust
- [OpenViking](https://github.com/volcengine/OpenViking) — Context database for AI agents — unifies memory, resources, and skills under a filesystem paradigm with tiered loading (L0/L1/L2) and observable retrieval trajectories
- [HolmesGPT](https://github.com/HolmesGPT/holmesgpt) — CNCF Sandbox SRE agent — investigates production incidents and finds root causes by querying live observability data from Kubernetes, Prometheus, Datadog, Grafana, AWS, GCP, Azure, and 30+ more sources
- [CozeLoop](https://github.com/coze-dev/coze-loop) — Full-lifecycle agent optimization platform from ByteDance/Coze — prompt development with visual playground, automated multi-dimensional evaluation, and full execution observability from user input to AI output
- [Kubeshark](https://github.com/kubeshark/kubeshark) — eBPF-powered network observability for Kubernetes — indexes L4/L7 traffic with full K8s context, decrypts TLS without keys, queryable by AI agents via MCP
- [OpenSRE](https://github.com/Tracer-Cloud/opensre) — Open-source framework for building AI SRE agents with scored synthetic RCA suites, real-world end-to-end tests, and reinforcement learning training environment for production incident response
- [RTK](https://github.com/rtk-ai/rtk) — CLI proxy that intercepts LLM API calls and compresses token usage by 60-90% on common dev commands — single Rust binary, zero dependencies, works with any agent
- [OpenLit](https://github.com/openlit/openlit) — OpenTelemetry-native LLM observability platform — traces, GPU monitoring, guardrails, evaluations, prompt management, and vault in one stack with 50+ integrations

## Mcp

- [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) — Official Chrome DevTools exposed as MCP server — lets coding agents inspect, debug, and profile web apps directly

## Memory

- [claude-mem](https://github.com/thedotmack/claude-mem) — Persistent context across sessions for coding agents — captures session activity, compresses with AI, injects into future sessions
- [Acontext](https://github.com/memodb-io/Acontext) — Agent skills as a memory layer — captures learnings from agent runs as plain markdown files, no embeddings, no API lock-in, git-friendly
- [Memvid](https://github.com/memvid/memvid) — Replaces complex RAG pipelines with a serverless, single-file memory layer built on video encoding for instant retrieval
- [Pro Workflow](https://github.com/rohitg00/pro-workflow) — Self-correcting memory for Claude Code — stores every correction as a searchable rule in SQLite, builds persistent FTS5-indexed wikis, and runs an auto-research loop so agent knowledge compounds across sessions
- [Create Context Graph](https://github.com/neo4j-labs/create-context-graph) — Neo4j Labs CLI that scaffolds full-stack agent apps with graph-based reasoning memory — pick your domain, pick your framework, get a complete app with graph visualization in under 5 minutes

## Monitoring

- [Opik](https://github.com/comet-ml/opik) — Open-source AI observability, evaluation, and optimization platform — tracing, automated evals, prompt optimization, and production dashboards for LLM apps and agentic workflows

## Multi Agent

- [CCCC](https://github.com/ChesterRa/cccc) — Local-first multi-agent collaboration kernel — append-only ledger for durable state, read receipts, delivery tracking, and remote ops from your phone via Telegram/Slack bridges

## Observability

- [Lapdog (Datadog)](https://lapdog.datadoghq.com/) — Local agent tracer — traces reasoning and tool calls from Codex, Claude Code, and Pi in real time, no account required

## Orchestration

- [contrabass](https://github.com/junhoyeo/contrabass) — Project-level orchestrator for AI coding agents — Go + Charm TUI implementation of OpenAI's Symphony SPEC.md
- [OpenAI Symphony SPEC.md](https://www.infoq.com/news/2026/05/openai-symphony-agents/) — OpenAI open-sourced Symphony, a SPEC.md for autonomous coding agent orchestration
- [TraceFix](https://ortiz.rutgers.edu/projects/tracefix/) — Uses TLA+ counterexamples to repair multi-agent LLM coordination protocols before deployment
- [Google Antigravity 2.0](https://developers.google.com/antigravity) — Google's multi-agent orchestration platform — standalone desktop app, CLI, SDK, voice. Gemini 3.5 Flash runs 12x faster within the framework
- [Ruflo](https://github.com/ruvnet/ruflo) — Agent orchestration platform for Claude — deploy multi-agent workflows with a visual builder and structured output routing
- [MassGen](https://github.com/massgen/MassGen) — Open-source multi-agent scaling system with TUI — agents work in parallel, vote on best solutions via consensus, with checklist-gated quality rounds
- [Warp Oz Multi-Agent Orchestration](https://x.com/warpdotdev/status/2056772856835453395) — Multi-agent orchestration in Warp's Oz — delegate complex tasks across Claude Code, Codex, and Warp Agent with worktree isolation and message passing
- [Open Multi-Agent](https://github.com/open-multi-agent/open-multi-agent) — TypeScript-native multi-agent orchestration — turns a goal into a task DAG automatically, with MCP and live tracing, three runtime dependencies
- [Sandcastle](https://github.com/mattpocock/sandcastle) — Orchestrate sandboxed coding agents in TypeScript with sandcastle.run() — single API call spins up an isolated agent on Docker, Podman, or Vercel Firecracker microVMs

## Retrieval

- [Retrieval Routing: vector + GraphRAG + PageIndex](https://x.com/NullS0S/status/2056383310830735676) — Production pattern: route queries across vector RAG, GraphRAG, and PageIndex based on query type using a lightweight classifier before retrieval

## Security

- [pentest-ai](https://github.com/0xSteph/pentest-ai) — Offensive security MCP server — wraps 205 pentesting tools and 17 specialist agents behind a single MCP interface
- [audit (evilsocket)](https://github.com/evilsocket/audit) — 8-stage vulnerability discovery agent — reimplements Cloudflare's Project Glasswing pipeline with narrow agents, deliberate disagreement, and reachability tracing
- [OneCLI](https://github.com/onecli/onecli) — Open-source credential vault for AI agents — agents access services without ever seeing real keys, MCP-compatible
- [Varlock](https://github.com/dmno-dev/varlock) — AI-safe .env files — separates schema definitions (safe for agents to read) from secret values (only humans access), preventing agents from ever seeing raw credentials in config files
- [Infisical Agent Vault](https://github.com/Infisical/agent-vault) — HTTP credential proxy and vault for AI agents — intercepts outbound requests and injects real credentials so agents never see raw secrets
- [ExploitBench](https://github.com/exploitbench/exploitbench) — Progressive difficulty benchmark that measures how far AI agents climb from finding vulnerable code to building working exploits — code analysis → trigger → primitive → RCE
- [AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard) — Full-stack AI red teaming platform from Tencent — scans OpenClaw deployments, agent configurations, MCP servers, skills, and LLM endpoints for vulnerabilities and jailbreak attempts
- [shellfirm](https://github.com/kaplanelad/shellfirm) — Safety guardrails for AI coding agents and human terminal commands — intercepts risky shell commands before execution with challenge-response confirmation, blast radius detection, and safe alternative suggestions
- [AgentDoG](https://github.com/AI45Lab/AgentDoG) — Trajectory-level risk diagnosis framework for autonomous agents — analyzes full execution traces to detect safety risks that emerge mid-trajectory, not just at final output
- [Pipelock](https://github.com/luckyPipewrench/pipelock) — Open-source AI agent firewall and egress proxy that sits inline between coding agents and the network — scans MCP traffic bidirectionally, blocks credential leaks and prompt injection, generates mediator-signed cryptographic proof of agent actions
- [RAMPART](https://github.com/microsoft/RAMPART) — Pytest-native safety and security testing framework for AI agents from Microsoft — write adversarial attack tests, benign failure tests, and harm category assertions as regular pytest cases
- [Greywall](https://github.com/GreyhavenHQ/greywall) — Container-free deny-by-default sandbox for AI coding agents — kernel-enforced filesystem, network, and syscall isolation via landlock and seccomp
- [RAPTOR](https://github.com/gadievron/raptor) — Autonomous offensive/defensive security research framework built on Claude Code — chains static analysis (Semgrep, CodeQL), binary analysis (AFL++ fuzzing, rr debugger), LLM vulnerability validation, exploit generation, and patch writing into a single workflow
- [nono](https://github.com/always-further/nono) — Capability-based sandbox for AI agents built in Rust — zero setup, zero latency, fine-grained policy brokering directly in the agent's operating context
- [code-on-incus](https://github.com/mensfeld/code-on-incus) — Give each AI agent its own isolated machine with root, Docker, and systemd — active defense detects and stops reverse shells, credential scanning, and data exfiltration automatically
- [IronCurtain](https://github.com/provos/ironcurtain) — Secure runtime for autonomous AI agents where security policy is derived from a human-readable constitution — plain English in, deterministic enforcement out
- [iFixAi](https://github.com/ifixai-ai/iFixAi) — Open-source diagnostic for AI misalignment — 32 behavioral tests across fabrication, manipulation, deception, unpredictability, and opacity. Provider-agnostic, letter grade in under 5 minutes.

## Tools

- [Context7](https://github.com/upstash/context7) — Up-to-date code documentation delivered to LLMs and code editors via MCP — solves the stale-doc problem for coding agents
- [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) — Chrome DevTools as MCP server — lets coding agents control and inspect a live browser for debugging, performance, and automation
- [Agent Device](https://github.com/callstackincubator/agent-device) — CLI tool giving AI agents control over iOS, Android, TV, and desktop apps — token-efficient accessibility snapshots instead of screenshots, with MCP support
- [Slopless](https://github.com/agent-quality-controls/slopless) — Deterministic textlint rules and CLI for catching AI-generated prose patterns in Markdown — 50+ rules, zero LLM calls, installable as a Codex or Claude Code skill

---

110 projects indexed.
