# Awesome AI Agent Discoveries

> Auto-curated by [@agentxagi](https://twitter.com/agentxagi) — real projects, real stars, updated daily.

## Agent Infrastructure

- **[ECC](https://github.com/affaan-m/ECC)** (★188,000) — Agent harness performance optimization system. Skills, instincts, memory, security, and research-first development for Claude Code, Codex, Opencode, Cursor and beyond.
- **[OpenViking](https://github.com/volcengine/OpenViking)** (★24,380) — Open-source context database for AI Agents. File system paradigm with hierarchical context delivery and self-evolving.
- **[Agent Orchestrator](https://github.com/ComposioHQ/agent-orchestrator)** (★7,179) — Parallel coding agent orchestrator. Plans tasks, spawns agents via tmux+git worktrees, handles CI fixes, merge conflicts, and code reviews autonomously.
- **[ByteRover CLI](https://github.com/campfirein/byterover-cli)** (★4,769) — Portable memory layer for autonomous coding agents. MCP server providing persistent context across sessions. Works with Claude Code, Codex, any agent.
- **[zerolang](https://github.com/vercel-labs/zerolang)** (★4,120) — Agent-first programming language by Vercel Labs. Small regular syntax designed for agents to learn on the fly. Structured diagnostics, deterministic tooling, deep stdlib. Written in C.
- **[Motus (lithos-ai)](https://github.com/lithos-ai/motus)** (★455) — Open-source agent-serving project. From the team behind Motus Tracing (356 likes, 27K views on Twitter). Agent observability infrastructure.
- **[engram](https://github.com/Gentleman-Programming/engram)** (★0) — Persistent memory system for AI coding agents. Agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI.
- **[osaurus](https://github.com/osaurus-ai/osaurus)** (★0) — Native macOS harness for AI agents. Any model, persistent memory, autonomous execution, cryptographic identity. Fully offline. Swift.
- **[code-review-graph](https://github.com/tirth8205/code-review-graph)** (★0) — Local knowledge graph for Claude Code. Builds a persistent map of your codebase so Claude reads only what matters — 6.8x fewer tokens on reviews and up to 49x on daily coding tasks. 19+ languages. Runs fully local. No API keys.
- **[Mirage](https://github.com/strukto-ai/mirage)** (★0) — A unified virtual filesystem for AI agents. Gives every agent a consistent file interface regardless of backend. Works with Claude Code, LangChain, OpenAI agents. TypeScript + Python.
- **[mcp2cli](https://github.com/knowsuchagency/mcp2cli)** (★0) — Turn any MCP, OpenAPI, or GraphQL server into a CLI — at runtime, with zero codegen. Every MCP server loads ALL tool definitions on EVERY turn. mcp2cli converts them to simple commands the agent calls only when needed. Saves thousands of tokens per turn.
- **[EverOS](https://github.com/EverMind-AI/EverOS)** (★0) — Build, evaluate, and integrate long-term memory for self-evolving agents. Python, Apache-2.0.
- **[SimpleMem](https://github.com/aiming-lab/SimpleMem)** (★0) — Efficient lifelong memory for LLM agents — text and multimodal. Python, MIT.
- **[zeroclaw](https://github.com/zeroclaw-labs/zeroclaw)** (★0) — Fast, small, fully autonomous AI personal assistant infrastructure. Rust-based. Deploy anywhere, any OS, any platform. Modular swap-anything architecture.
- **[holaOS](https://github.com/holaboss-ai/holaOS)** (★0) — Agent OS that turns repeat work into running AI work-streams. Electron-based, MCP-compatible, with persistent memory and proactive AI runtime. TypeScript.
- **[boxlite](https://github.com/boxlite-ai/boxlite)** (★0) — Compute substrate for AI agents: lightweight on laptop, elastic to cloud. Rust + TypeScript, Apache 2.0. Embedded, self-hosted, serverless.

- **[Firefox DevTools MCP](https://github.com/mozilla/firefox-devtools-mcp)** (★170) — Official Mozilla MCP server for Firefox DevTools. AI agents inspect and control Firefox through Remote Debugging Protocol. TypeScript, MIT.
## Agent Memory

- **[memvid](https://github.com/memvid/memvid)** (★15,542) — Memory layer for AI Agents. Replaces complex RAG pipelines with a serverless, single-file memory layer. Rust-based, offline-first.
- **[agentmemory](https://github.com/rohitg00/agentmemory)** (★0) — Persistent memory for AI coding agents. Records session activity, compresses with AI, injects context back on next session. 4-layer memory architecture: working, episodic, semantic, procedural. 95.2% retrieval accuracy on LongMemEval-S.
- **[MemOS](https://github.com/MemTensor/MemOS)** (★0) — Self-evolving memory OS for LLM and AI agents. Hybrid retrieval (keyword + vector + graph), cross-task skill reuse, 35.24% token savings.

## Agent Security
- **[Anthropic Cybersecurity Skills](https://github.com/mukul975/Anthropic-Cybersecurity-Skills)** (★6,543) — 754 structured cybersecurity skills for AI agents. Mapped to 5 frameworks: MITRE ATT&CK, NIST CSF 2.0, MITRE ATLAS, D3FEND, NIST AI RMF. Works with Claude Code, Copilot, Codex CLI, Cursor, Gemini CLI and 20+ platforms. 26 security domains. Python, Apache 2.0.
- **[AI Security Arsenal](https://github.com/hardw00t/ai-security-arsenal)** (★73) — Curated security skills for AI agents. Appsec, cloud, containers, LLM attacks, and threat modeling. Compatible with Claude Code, OpenClaw, and other agent tools. Python, MIT.

- **[audit (evilsocket)](https://github.com/evilsocket/audit)** (★397) — An 8-stage vulnerability-discovery agent. Reimplements Cloudflare's Project Glasswing pipeline with many narrow agents, adversarial validation, and reachability tracing. By the bettercap creator. MIT, Python.

- **[AiSOC](https://github.com/beenuar/AiSOC)** (★0) — Open-source AI-powered Security Operations Center. Alert fusion, purple-team drills, agent-assisted triage, MITRE ATT&CK investigation. MIT-licensed, self-hostable. Python + Next.js.
- **[agent-governance-toolkit](https://github.com/microsoft/agent-governance-toolkit)** (★0) — Microsoft AI Agent Governance Toolkit. Policy enforcement, zero-trust identity, execution sandboxing, reliability engineering for autonomous agents. Covers 10/10 OWASP Agentic Top 10. Python, MIT.
- **[agent-safehouse](https://github.com/eugene1g/agent-safehouse)** (★0) — Sandbox your local AI agents so they can read/write only what they need. Shell-based, minimal.

- **[NSA MCP Security Design Considerations](https://www.nsa.gov/Portals/75/documents/Cybersecurity/CSI_MCP_SECURITY.pdf)** — NSA Cybersecurity official security guidance for AI-driven automation using MCP. Implicit trust boundaries, dynamic tool execution risks, hardening steps for MCP deployments. Trending on Twitter with 2.4K+ views.
- **[HexStrike AI](https://github.com/0x4m4/hexstrike-ai)** (★8,867) — MCP server exposing 150+ cybersecurity tools to AI agents. Automated pentesting, vulnerability discovery, bug bounty automation. Python, MIT.
- **[Claude Code System Prompts](https://github.com/Piebald-AI/claude-code-system-prompts)** (★10,386) — Full Claude Code system prompt transparency. 27 builtin tool descriptions, sub-agent prompts (Plan/Explore/Task), security review process. Updated per version.

- **[AI Kill Chain](https://github.com/gouravnagar-infosec/ai-kill-chain)** (★37) — Defender-side extension of the Lockheed Martin Cyber Kill Chain for LLM and agentic AI threats. Adds a model supply chain stage and splits actions-on-objectives into exfiltration, model extraction, and agentic pivot.

## Agent Tools

- **[html-anything](https://github.com/nexu-io/html-anything)** (★0) — Agentic HTML editor — your local AI agent writes the HTML, you ship it. 75 skills × 9 surfaces (magazine, deck, poster, XHS/tweet, prototype, data report, Hyperframes). Sandboxed preview, 1-click publish to WeChat/X/Zhihu. Zero API key required.

## Agents

- **[OctoTools](https://github.com/octotools/octotools)** (★1,462) — Agentic framework with extensible tool cards for complex reasoning. Planner+executor loop, standardized tool metadata. Broad LLM support.
- **[OpenSquilla](https://github.com/opensquilla/opensquilla)** (★1,278) — Token-efficient microkernel AI agent. Local model router sends each turn to cheapest capable model. Persistent memory, layered sandbox, web search, on-device embeddings. 20+ LLM providers.
- **[Photo-agents](https://github.com/jmerelnyc/Photo-agents)** (★1,022) — Autonomous self-evolving agents with vision-grounded layered memory. Perceive/reason/act loop. Agents write own skills from real success. Multi-provider LLM router.
- **[skillgrade](https://github.com/mgechev/skillgrade)** (★0) — Unit tests for agent skills — run assertions against agent skill outputs the same way you'd test code
- **[agent-skills-eval](https://github.com/darkrishabh/agent-skills-eval)** (★0) — Test runner for agentskills.io-style skills with YAML-based scenarios and LLM judges
- **[eval-view](https://github.com/hidai25/eval-view)** (★0) — Regression testing for AI agents — snapshot behavior, diff tool calls, catch regressions in CI
- **[agent-belt](https://github.com/jfrog/agent-belt)** (★0) — Reproducible evaluation for AI coding agents — multi-turn scenarios, rich assertions, multi-judge consensus
- **[Raindrop Workshop](https://github.com/raindrop-ai/workshop)** (★0) — Local debugger for AI agents — live streamed traces of every token, tool call, and decision with self-healing eval loops
- **[12-Factor Agents](https://github.com/humanlayer/12-factor-agents)** (★0) — Engineering principles for building production-grade LLM-powered software — agents as software with LLM steps, not prompt loops
- **[Context Mode](https://github.com/mksglu/context-mode)** (★0) — Context window optimization for AI coding agents — sandboxes tool output, claims 98% reduction in context usage across 15 platforms
- **[DeerFlow](https://github.com/bytedance/deer-flow)** (★0) — Long-horizon SuperAgent by ByteDance — researches, codes, and creates with sandboxes, memories, tools, skills, subagents, and message gateway
- **[Memori](https://github.com/MemoriLabs/Memori)** (★0) — Agent-native memory infrastructure — LLM-agnostic layer that turns agent execution and conversation into structured, persistent state for production systems
- **[Engram](https://github.com/Gentleman-Programming/engram)** (★0) — Persistent memory system for AI coding agents — agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI
- **[CUA (Computer Use Agents)](https://github.com/trycua/cua)** (★0) — Open-source infrastructure for Computer-Use Agents — sandboxes, SDKs, and benchmarks for agents that control full desktops across macOS, Linux, and Windows
- **[memU](https://github.com/NevaMind-AI/memU)** (★0) — Memory system built for 24/7 proactive agents like OpenClaw — persistent, structured memory that survives across agent sessions and restarts
- **[ZeroLang](https://github.com/vercel-labs/zerolang)** (★0) — Agent-first programming language from Vercel Labs — designed for AI agents as primary users, with structured diagnostics, tiny static binaries, and learnable syntax
- **[agentmemory](https://github.com/rohitg00/agentmemory)** (★0) — Persistent memory for AI coding agents — extends Karpathy's LLM Wiki pattern with confidence scoring, lifecycle, knowledge graphs, and hybrid search
- **[Raindrop Workshop](https://github.com/raindrop-ai/workshop)** (★0) — Local debugger for AI agents that streams every token, tool call, and decision in realtime — then lets Claude Code read your traces, write evals, and fix what's broken
- **[SmallCode](https://github.com/Doorman11991/smallcode)** (★0) — Terminal-native coding agent built for small local models (7B-20B) — compensates for small model limitations with budget-managed context, forgiving tool-call parsing, TODO-file decomposed planning, and search-and-replace patches instead of full file rewrites
- **[NanoClaw](https://github.com/nanocoai/nanoclaw)** (★0) — Lightweight container-first alternative to OpenClaw — runs agents in isolated containers with built-in memory, scheduled jobs, and connects to WhatsApp, Telegram, Slack, Discord, Gmail
- **[IronClaw](https://github.com/nearai/ironclaw)** (★0) — Agent OS built in Rust focused on privacy, security, and extensibility — uses WebAssembly for sandboxed agent plugins
- **[DeepAgents](https://github.com/langchain-ai/deepagents)** (★0) — Batteries-included agent harness from LangChain — planning, sub-agents, filesystem, context management, persistent memory, skills, and MCP tool support built on LangGraph
- **[Obsidian Mind](https://github.com/breferrari/obsidian-mind)** (★0) — Obsidian vault that gives AI coding agents persistent memory — works with Claude Code, Codex CLI, Gemini CLI out of the box
- **[TencentDB Agent Memory](https://github.com/Tencent/TencentDB-Agent-Memory)** (★0) — 4-tier progressive memory pipeline for AI agents — symbolic short-term memory (Mermaid symbol offloading) + layered long-term memory (L0 raw → L1 facts → L2 summaries → L3 personas), fully local, zero external dependencies
- **[Beads](https://github.com/gastownhall/beads)** (★0) — Distributed graph issue tracker for AI coding agents — replaces markdown TODO lists with a Dolt-backed SQL database, dependency chains, memory compaction, and zero-conflict multi-agent coordination
- **[Forge (antoinezambelli)](https://github.com/antoinezambelli/forge)** (★0) — Reliability layer for self-hosted LLM tool-calling — lifts 8B local models to 86.5% on multi-step agentic evals through rescue parsing, retry nudges, step enforcement, and VRAM-aware context budgets
- **[Ruflo](https://github.com/ruvnet/ruflo)** (★0) — Agent orchestration platform for Claude — deploy multi-agent swarms with self-learning coordination, RAG, and native Claude Code/Codex integration
- **[ECC](https://github.com/affaan-m/ECC)** (★0) — Harness-native operator system for coding agents — skills, instincts, memory optimization, security scanning, and research-first development across Claude Code, Codex, Cursor, Gemini, and 7+ other agent harnesses
- **[ClawGUI](https://github.com/ZJU-REAL/ClawGUI)** (★0) — Full-stack framework for GUI agents — online RL training, standardized evaluation benchmarks, and real-device deployment in one package from Zhejiang University
- **[Emdash](https://github.com/generalaction/emdash)** (★0) — Agentic Development Environment (ADE) that runs multiple coding agents in parallel, each isolated in its own git worktree — supports 27 CLI agents including Claude Code, Codex, Gemini, Hermes Agent
- **[ContextForge (mcp-context-forge)](https://github.com/IBM/mcp-context-forge)** (★0) — IBM's open-source gateway, registry, and proxy that federates MCP, A2A, and REST/gRPC APIs into one unified endpoint with centralized governance, discovery, and guardrails
- **[Statewright](https://github.com/statewright/statewright)** (★0) — State machine guardrails that control which tools AI agents can use in each phase — planning gets read-only, implementation unlocks edit tools, testing only permits test commands
- **[CUGA](https://github.com/cuga-project/cuga-agent)** (★0) — Open-source generalist agent harness for enterprise — supports complex task execution on web and APIs, OpenAPI/MCP integrations, composable architecture, reasoning modes, and policy-aware features
- **[Archestra](https://github.com/archestra-ai/archestra)** (★0) — Enterprise AI platform with guardrails, MCP registry, gateway, and orchestrator — unifies agent tool access with centralized governance and cost controls
- **[Agent of Empires](https://github.com/njbrake/agent-of-empires)** (★0) — Session manager for parallel AI coding agents — runs Claude Code, Codex, Gemini, Cursor, and 10+ more agents in isolated tmux sessions with git worktrees, Docker sandboxing, TUI + web dashboard, and mobile access
- **[Pi Agent Harness](https://github.com/earendil-works/pi)** (★0) — Self-extensible coding agent CLI with unified multi-provider LLM API, agent runtime with tool calling and state management, and a terminal UI library with differential rendering
- **[OpenAI Agents SDK](https://github.com/openai/openai-agents-python)** (★0) — OpenAI's official lightweight multi-agent framework — provider-agnostic SDK with agents, sandbox agents, handoffs, guardrails, human-in-the-loop, sessions, tracing, and realtime voice agents
- **[CodeGraph](https://github.com/colbymchenry/codegraph)** (★0) — Pre-indexed code knowledge graph for coding agents — replaces expensive file-scanning with instant symbol relationship queries, cutting tokens by ~35% and tool calls by ~70%
- **[OpenCowork](https://github.com/OpenCoworkAI/open-cowork)** (★0) — Open-source AI agent desktop app that one-click installs Claude Code, MCP tools, and Skills with sandbox isolation and multi-model support
- **[OpenHuman](https://github.com/tinyhumansai/openhuman)** (★0) — Desktop-first personal AI agent with 118+ one-click OAuth integrations, Memory Tree knowledge base, and auto-fetch data sync — all local-first, Rust/Tauri
- **[Nexent](https://github.com/ModelEngine-Group/nexent)** (★0) — Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles — pure language input, unified tools, skills, memory, and orchestration with built-in constraints and feedback loops
- **[HiClaw](https://github.com/agentscope-ai/HiClaw)** (★0) — Collaborative multi-agent OS using Matrix protocol rooms for transparent human-in-the-loop coordination — Manager-Workers architecture with OpenClaw, QwenPaw, and Hermes runtimes coexisting

## Agents Frameworks

- **[Hive (aden-hive)](https://github.com/aden-hive/hive)** (★10,397) — Multi-Agent Harness for Production AI. Python framework with self-improving agents, human-in-the-loop, agent skills, supports OpenAI and Anthropic.
- **[cc-sdd (Spec-Driven Development)](https://github.com/gotalab/cc-sdd)** (★3,374) — Turns approved specs into long-running autonomous implementation. Minimal SDD harness with agent skills for Claude Code, Codex, Cursor, Copilot, Gemini CLI.
- **[smallcode](https://github.com/Doorman11991/smallcode)** (★0) — AI coding agent optimized for small LLMs. Hits 87% benchmark score with only a 4B-active parameter model. Proves you dont need massive models for real coding tasks.
- **[ARGO](https://github.com/xark-argo/argo)** (★0) — Open-source local AI agent platform. Manus-style autonomous task execution running 100% on your laptop. No cloud, no subscription. Multi-agent task engine with planning, reflection, tool chaining. Ollama + HuggingFace + OpenAI/Claude/DeepSeek. Full MCP support. Local RAG.
- **[Dulus](https://github.com/KevRojo/Dulus)** (★0) — Free CLI agent that harvests Gemini (guest, no login), Claude.ai, Kimi, Qwen, DeepSeek browser sessions and turns them into tool-calling agents. Reads and edits files, runs Bash, greps repos, browses the web, ships commits. All from terminal at $0.
- **[moltis](https://github.com/moltis-org/moltis)** (★0) — Secure persistent personal agent server in Rust. One binary, sandboxed execution, multi-provider LLMs, voice, memory, messaging integrations. Runs on your hardware.
- **[oh-my-claudecode](https://github.com/Yeachan-Heo/oh-my-claudecode)** (★0) — Teams-first multi-agent orchestration for Claude Code. Parallel execution, agent specialization.
- **[TradingAgents](https://github.com/TauricResearch/TradingAgents)** (★0) — Multi-agent LLM financial trading framework. Research Desk, Quant Team, Trading Floor, and Risk Management as separate agents orchestrated together. Python.
- **[omo (oh-my-openagent)](https://github.com/code-yeongyu/oh-my-openagent)** (★0) — The best agent harness. Previously oh-my-opencode. 58.8K stars. Supports Claude Code, Codex, Cursor, Gemini CLI, OpenCode. Modular skills, orchestration, agent loop — all in one harness.
- **[agent-lightning](https://github.com/microsoft/agent-lightning)** (★0) — Microsoft open-source RL trainer for AI agents. Works with LangChain, AutoGen, CrewAI, OpenAI SDK, or plain Python. Captures prompts, tool calls, rewards as structured events. Trains improved prompts or policy weights automatically.
- **[TEN Framework](https://github.com/TEN-framework/ten-framework)** (★0) — Open-source framework for conversational voice AI agents. Multi-modal, real-time voice + video. Python.
- **[nexent](https://github.com/ModelEngine-Group/nexent)** (★0) — Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles. Unified tools, skills, memory, orchestration with constraints, feedback loops, control planes. Python, MIT.

## Evaluation

- **[MCP-Universe](https://github.com/SalesforceAIResearch/MCP-Universe)** (★0) — RL training and benchmarking framework for MCP tool-use agents — lets you train agents to use tools via reinforcement learning and evaluate them on standardized benchmarks
- **[Eval Engineer](https://github.com/Galileo-Agent-Labs/eval-engineer)** (★0) — Open-source skill bundle that turns Claude Code and Codex into eval engineers backed by Galileo traces — inspect, diagnose, fix, and verify agent behavior through evidence
- **[ClawBench](https://github.com/reacher-z/ClawBench)** (★0) — Open-source benchmark for browser AI agents — 153 everyday tasks across 144 live websites with 5-layer recording, DOM-match, and LLM judge
- **[MCPMark](https://github.com/eval-sys/mcpmark)** (★0) — Stress-testing benchmark for MCP tool-use — evaluates agents across real MCP servers (Notion, GitHub, Filesystem, Postgres, Playwright) with isolated sandboxes and unified metrics
- **[Claw-Eval](https://github.com/claw-eval/claw-eval)** (★0) — Evaluation harness for autonomous agents — 300 human-verified tasks across 9 categories with Pass^3 methodology, 2159 rubrics, and public leaderboard
- **[PinchBench](https://github.com/pinchbench/skill)** (★0) — Real-world benchmark for OpenClaw coding agents — 53 tasks measuring tool usage, multi-step reasoning, and practical outcomes (did it actually schedule the meeting, create the file, triage the email?)

## Governance

- **[Agent Governance Toolkit](https://github.com/microsoft/agent-governance-toolkit)** (★0) — Runtime governance for AI agents — every tool call, resource access, and inter-agent message evaluated against policy before execution, deterministic, sub-millisecond, auditable

## Infrastructure

- **[Cloudflare + Claude Managed Agents isolated execution](https://x.com/Cloudflare/status/2056747823907942668)** (★0) — Cloudflare integrates with Anthropic's Claude Managed Agents to provide isolated sandboxed execution environments for autonomous code delivery at edge scale
- **[Anthropic acquires Stainless ($300M)](https://www.infoworld.com/article/4172947/anthropic-acquires-stainless-to-strengthen-claudes-developer-tooling.html)** (★0) — Anthropic acquires Stainless for $300M — the company behind every Anthropic SDK generator and MCP server tool since the early API days
- **[Plano](https://github.com/katanemo/plano)** (★0) — AI-native proxy and data plane for agentic apps — LLM routing, safety guardrails, orchestration, and observability in one Rust proxy
- **[Cozeloop](https://github.com/coze-dev/coze-loop)** (★0) — Full-lifecycle agent optimization platform — dev, debug, eval, and monitor agents from a single Go service
- **[CubeSandbox](https://github.com/TencentCloud/CubeSandbox)** (★0) — Hardware-isolated sandbox for AI agents built on RustVMM + KVM — boots in under 60ms, uses less than 5MB per instance
- **[OpenSandbox (Alibaba)](https://github.com/alibaba/OpenSandbox)** (★0) — Secure sandbox runtime for AI agents from Alibaba — extensible plugin architecture for isolation, resource limits, and policy enforcement
- **[microsandbox](https://github.com/superradcompany/microsandbox)** (★0) — Secure, local, programmable sandboxes for AI agents — runs entirely on your machine, no cloud dependency, Rust API
- **[τ³-bench (tau-three-bench)](https://github.com/sierra-research/tau2-bench)** (★0) — Multimodal benchmark for agent evaluation — now covers text, voice (full-duplex), and knowledge retrieval domains with a live leaderboard
- **[LiteLLM Agent Platform](https://github.com/BerriAI/litellm-agent-platform)** (★0) — Self-hosted platform for running coding agents in isolated sandboxes with a credential vault — agents get stub keys, vault swaps them for real ones on every outbound TLS call
- **[Laminar](https://github.com/lmnr-ai/lmnr)** (★0) — Open-source observability platform purpose-built for AI agents — traces, evals, monitoring, SQL access to all data, written in Rust
- **[OpenViking](https://github.com/volcengine/OpenViking)** (★0) — Context database for AI agents — unifies memory, resources, and skills under a filesystem paradigm with tiered loading (L0/L1/L2) and observable retrieval trajectories
- **[HolmesGPT](https://github.com/HolmesGPT/holmesgpt)** (★0) — CNCF Sandbox SRE agent — investigates production incidents and finds root causes by querying live observability data from Kubernetes, Prometheus, Datadog, Grafana, AWS, GCP, Azure, and 30+ more sources
- **[CozeLoop](https://github.com/coze-dev/coze-loop)** (★0) — Full-lifecycle agent optimization platform from ByteDance/Coze — prompt development with visual playground, automated multi-dimensional evaluation, and full execution observability from user input to AI output
- **[Kubeshark](https://github.com/kubeshark/kubeshark)** (★0) — eBPF-powered network observability for Kubernetes — indexes L4/L7 traffic with full K8s context, decrypts TLS without keys, queryable by AI agents via MCP
- **[OpenSRE](https://github.com/Tracer-Cloud/opensre)** (★0) — Open-source framework for building AI SRE agents with scored synthetic RCA suites, real-world end-to-end tests, and reinforcement learning training environment for production incident response
- **[RTK](https://github.com/rtk-ai/rtk)** (★0) — CLI proxy that intercepts LLM API calls and compresses token usage by 60-90% on common dev commands — single Rust binary, zero dependencies, works with any agent
- **[OpenLit](https://github.com/openlit/openlit)** (★0) — OpenTelemetry-native LLM observability platform — traces, GPU monitoring, guardrails, evaluations, prompt management, and vault in one stack with 50+ integrations

## Mcp

- **[MCP Gateway Registry](https://github.com/agentic-community/mcp-gateway-registry)** (★658) — Enterprise-ready MCP Gateway & Registry. Centralizes AI dev tools with secure OAuth authentication, dynamic tool discovery, Keycloak and Entra ID integration, fine-grained access control. TypeScript.

- **[Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp)** (★0) — Official Chrome DevTools exposed as MCP server — lets coding agents inspect, debug, and profile web apps directly
- **[MCP Toolbox for Databases](https://github.com/googleapis/mcp-toolbox)** (★0) — Open-source MCP server by Google for databases. Supports PostgreSQL, MySQL, BigQuery, Spanner, MongoDB, Redis, Elasticsearch, ClickHouse, CockroachDB, Oracle, TiDB, Firestore, and more. Go.
- **[mcpc](https://github.com/apify/mcpc)** (★0) — Universal CLI client for MCP by Apify. Persistent sessions, stdio/HTTP, OAuth 2.1, tasks, JSON output, proxy for AI sandboxes, x402 support.

## Memory

- **[claude-mem](https://github.com/thedotmack/claude-mem)** (★0) — Persistent context across sessions for coding agents — captures session activity, compresses with AI, injects into future sessions
- **[Acontext](https://github.com/memodb-io/Acontext)** (★0) — Agent skills as a memory layer — captures learnings from agent runs as plain markdown files, no embeddings, no API lock-in, git-friendly
- **[Memvid](https://github.com/memvid/memvid)** (★0) — Replaces complex RAG pipelines with a serverless, single-file memory layer built on video encoding for instant retrieval
- **[Pro Workflow](https://github.com/rohitg00/pro-workflow)** (★0) — Self-correcting memory for Claude Code — stores every correction as a searchable rule in SQLite, builds persistent FTS5-indexed wikis, and runs an auto-research loop so agent knowledge compounds across sessions
- **[Create Context Graph](https://github.com/neo4j-labs/create-context-graph)** (★0) — Neo4j Labs CLI that scaffolds full-stack agent apps with graph-based reasoning memory — pick your domain, pick your framework, get a complete app with graph visualization in under 5 minutes

## Monitoring

- **[Opik](https://github.com/comet-ml/opik)** (★0) — Open-source AI observability, evaluation, and optimization platform — tracing, automated evals, prompt optimization, and production dashboards for LLM apps and agentic workflows

## Multi Agent

- **[CCCC](https://github.com/ChesterRa/cccc)** (★0) — Local-first multi-agent collaboration kernel — append-only ledger for durable state, read receipts, delivery tracking, and remote ops from your phone via Telegram/Slack bridges

## Observability

- **[Lapdog (Datadog)](https://lapdog.datadoghq.com/)** (★0) — Local agent tracer — traces reasoning and tool calls from Codex, Claude Code, and Pi in real time, no account required

## Orchestration

- **[contrabass](https://github.com/junhoyeo/contrabass)** (★0) — Project-level orchestrator for AI coding agents — Go + Charm TUI implementation of OpenAI's Symphony SPEC.md
- **[OpenAI Symphony SPEC.md](https://www.infoq.com/news/2026/05/openai-symphony-agents/)** (★0) — OpenAI open-sourced Symphony, a SPEC.md for autonomous coding agent orchestration
- **[TraceFix](https://ortiz.rutgers.edu/projects/tracefix/)** (★0) — Uses TLA+ counterexamples to repair multi-agent LLM coordination protocols before deployment
- **[Google Antigravity 2.0](https://developers.google.com/antigravity)** (★0) — Google's multi-agent orchestration platform — standalone desktop app, CLI, SDK, voice. Gemini 3.5 Flash runs 12x faster within the framework
- **[Ruflo](https://github.com/ruvnet/ruflo)** (★0) — Agent orchestration platform for Claude — deploy multi-agent workflows with a visual builder and structured output routing
- **[MassGen](https://github.com/massgen/MassGen)** (★0) — Open-source multi-agent scaling system with TUI — agents work in parallel, vote on best solutions via consensus, with checklist-gated quality rounds
- **[Warp Oz Multi-Agent Orchestration](https://x.com/warpdotdev/status/2056772856835453395)** (★0) — Multi-agent orchestration in Warp's Oz — delegate complex tasks across Claude Code, Codex, and Warp Agent with worktree isolation and message passing
- **[Open Multi-Agent](https://github.com/open-multi-agent/open-multi-agent)** (★0) — TypeScript-native multi-agent orchestration — turns a goal into a task DAG automatically, with MCP and live tracing, three runtime dependencies
- **[Sandcastle](https://github.com/mattpocock/sandcastle)** (★0) — Orchestrate sandboxed coding agents in TypeScript with sandcastle.run() — single API call spins up an isolated agent on Docker, Podman, or Vercel Firecracker microVMs

## Retrieval

- **[Retrieval Routing: vector + GraphRAG + PageIndex](https://x.com/NullS0S/status/2056383310830735676)** (★0) — Production pattern: route queries across vector RAG, GraphRAG, and PageIndex based on query type using a lightweight classifier before retrieval

## Security

- **[claudit-sec](https://github.com/HarmonicSecurity/claudit-sec)** (★250) — Single-command security audit for Claude Desktop and Claude Code on macOS. Visibility into MCP servers, extensions, plugins, connectors, scheduled tasks, and permissions. Shell script, zero dependencies.

- **[pentest-ai](https://github.com/0xSteph/pentest-ai)** (★0) — Offensive security MCP server — wraps 205 pentesting tools and 17 specialist agents behind a single MCP interface
- **[audit (evilsocket)](https://github.com/evilsocket/audit)** (★0) — 8-stage vulnerability discovery agent — reimplements Cloudflare's Project Glasswing pipeline with narrow agents, deliberate disagreement, and reachability tracing
- **[OneCLI](https://github.com/onecli/onecli)** (★0) — Open-source credential vault for AI agents — agents access services without ever seeing real keys, MCP-compatible
- **[Varlock](https://github.com/dmno-dev/varlock)** (★0) — AI-safe .env files — separates schema definitions (safe for agents to read) from secret values (only humans access), preventing agents from ever seeing raw credentials in config files
- **[Infisical Agent Vault](https://github.com/Infisical/agent-vault)** (★0) — HTTP credential proxy and vault for AI agents — intercepts outbound requests and injects real credentials so agents never see raw secrets
- **[ExploitBench](https://github.com/exploitbench/exploitbench)** (★0) — Progressive difficulty benchmark that measures how far AI agents climb from finding vulnerable code to building working exploits — code analysis → trigger → primitive → RCE
- **[AI-Infra-Guard](https://github.com/Tencent/AI-Infra-Guard)** (★0) — Full-stack AI red teaming platform from Tencent — scans OpenClaw deployments, agent configurations, MCP servers, skills, and LLM endpoints for vulnerabilities and jailbreak attempts
- **[shellfirm](https://github.com/kaplanelad/shellfirm)** (★0) — Safety guardrails for AI coding agents and human terminal commands — intercepts risky shell commands before execution with challenge-response confirmation, blast radius detection, and safe alternative suggestions
- **[AgentDoG](https://github.com/AI45Lab/AgentDoG)** (★0) — Trajectory-level risk diagnosis framework for autonomous agents — analyzes full execution traces to detect safety risks that emerge mid-trajectory, not just at final output
- **[Pipelock](https://github.com/luckyPipewrench/pipelock)** (★0) — Open-source AI agent firewall and egress proxy that sits inline between coding agents and the network — scans MCP traffic bidirectionally, blocks credential leaks and prompt injection, generates mediator-signed cryptographic proof of agent actions
- **[RAMPART](https://github.com/microsoft/RAMPART)** (★0) — Pytest-native safety and security testing framework for AI agents from Microsoft — write adversarial attack tests, benign failure tests, and harm category assertions as regular pytest cases
- **[Greywall](https://github.com/GreyhavenHQ/greywall)** (★0) — Container-free deny-by-default sandbox for AI coding agents — kernel-enforced filesystem, network, and syscall isolation via landlock and seccomp
- **[RAPTOR](https://github.com/gadievron/raptor)** (★0) — Autonomous offensive/defensive security research framework built on Claude Code — chains static analysis (Semgrep, CodeQL), binary analysis (AFL++ fuzzing, rr debugger), LLM vulnerability validation, exploit generation, and patch writing into a single workflow
- **[nono](https://github.com/always-further/nono)** (★0) — Capability-based sandbox for AI agents built in Rust — zero setup, zero latency, fine-grained policy brokering directly in the agent's operating context
- **[code-on-incus](https://github.com/mensfeld/code-on-incus)** (★0) — Give each AI agent its own isolated machine with root, Docker, and systemd — active defense detects and stops reverse shells, credential scanning, and data exfiltration automatically
- **[IronCurtain](https://github.com/provos/ironcurtain)** (★0) — Secure runtime for autonomous AI agents where security policy is derived from a human-readable constitution — plain English in, deterministic enforcement out
- **[iFixAi](https://github.com/ifixai-ai/iFixAi)** (★0) — Open-source diagnostic for AI misalignment — 32 behavioral tests across fabrication, manipulation, deception, unpredictability, and opacity. Provider-agnostic, letter grade in under 5 minutes.

## Tools

- **[Context7](https://github.com/upstash/context7)** (★0) — Up-to-date code documentation delivered to LLMs and code editors via MCP — solves the stale-doc problem for coding agents
- **[Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp)** (★0) — Chrome DevTools as MCP server — lets coding agents control and inspect a live browser for debugging, performance, and automation
- **[Agent Device](https://github.com/callstackincubator/agent-device)** (★0) — CLI tool giving AI agents control over iOS, Android, TV, and desktop apps — token-efficient accessibility snapshots instead of screenshots, with MCP support
- **[Slopless](https://github.com/agent-quality-controls/slopless)** (★0) — Deterministic textlint rules and CLI for catching AI-generated prose patterns in Markdown — 50+ rules, zero LLM calls, installable as a Codex or Claude Code skill

- **[OpenTeam](https://github.com/afumu/openteam)** (★54) — Chrome extension for orchestrating local AI-agent team workflows across web AI services. Manage multiple agents from different providers in one browser interface. TypeScript.
- **[Forge](https://github.com/ForgeAILab/forge)** (★39) — Rust workflow engine for structured AI coding agent task lifecycles. MCP-native, self-hosted. Manages task lifecycles instead of ad-hoc agent loops.

---

146 discoveries indexed.

### CC-Switch
⭐ 77.2K | Cross-platform desktop All-in-One assistant for Claude Code, Codex, OpenCode, OpenClaw, Gemini CLI & Hermes Agent
→ [github.com/farion1231/cc-switch](https://github.com/farion1231/cc-switch)

### Antigravity Awesome Skills
⭐ 38.2K | 1,400+ installable agentic skills for Claude Code, Cursor, Codex CLI, Gemini CLI, and more
→ [github.com/sickn33/antigravity-awesome-skills](https://github.com/sickn33/antigravity-awesome-skills)

### Multica
⭐ 30.6K | Open-source managed agents platform. Turn coding agents into real teammates — assign tasks, track progress, compound skills
→ [github.com/multica-ai/multica](https://github.com/multica-ai/multica)
