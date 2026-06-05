# Awesome AI Agent Discoveries

A curated list of AI agent tools, frameworks, and discoveries. Updated continuously.

Maintained by [@agentxagi](https://x.com/agentxagi)

---

## Agent Security

- [Damn Vulnerable LLM Agent — Deliberately Vulnerable Agent for Security Training (460 Stars)](https://github.com/ReversecLabs/damn-vulnerable-llm-agent) ⭐ 460 — Deliberately vulnerable React-based LLM agent for practicing prompt injection, thought/action/observation hijacking, age
- pentest-ai  — Offensive security MCP server — wraps 205 pentesting tools and 17 specialist agents behind a single MCP interface
- Plano  — AI-native proxy and data plane for agentic apps — LLM routing, safety guardrails, orchestration, and observability in on
- Cozeloop  — Full-lifecycle agent optimization platform — dev, debug, eval, and monitor agents from a single Go service
- CubeSandbox  — Hardware-isolated sandbox for AI agents built on RustVMM + KVM — boots in under 60ms, uses less than 5MB per instance
- OpenSandbox — Secure, Fast Sandbox Runtime for AI Agents from Alibaba (10.8K Stars)  — Secure sandbox runtime for AI agents from Alibaba — extensible plugin architecture for isolation, resource limits, and p
- Microsandbox — Unexploitable Secrets for AI Agents via Hardware-Isolated microVMs (6.2K Stars)  — Spins up lightweight VMs in milliseconds. Hardware-level isolation. Rootless, embeddable SDK. Key feature: secrets that 
- AiSOC  — Open-source AI-powered Security Operations Center. Alert fusion, purple-team drills, agent-assisted triage, MITRE ATT&CK
- Microsoft Agent Governance Toolkit — Runtime Policy Enforcement for Every Agent Tool Call (1.9K Stars)  — Microsoft toolkit that intercepts every tool call, resource access, and inter-agent message BEFORE execution. Determinis
- agent-safehouse  — Sandbox your local AI agents so they can read/write only what they need. Shell-based, minimal.
- evilsocket/audit — 8-Stage Vulnerability-Discovery Agent (Cloudflare Glasswing Pipeline)  — From the creator of bettercap. Reimplementation of Cloudflare Project Glasswing: 8 narrow agents with deliberate disagre
- IronClaw — Agent OS Focused on Privacy, Security and Extensibility (12.3K Stars)  — Agent OS focused on privacy, security and extensibility. Written in Rust with WASM sandboxing and encrypted credential v
- AI-Infra-Guard — Full-Stack AI Red Teaming Platform by Tencent (3.8K Stars)  — A full-stack AI Red Teaming platform securing AI ecosystems via OpenClaw Security Scan, Agent Scan, Skills Scan, MCP sca
- supply-chain-guard (pc-style)  — Local supply-chain install gate for npm packages and VS Code extensions with Socket, Codex integration.
- NSA MCP Security Design Considerations  — NSA Cybersecurity published official security design considerations for AI-driven automation using the Model Context Pro
- HexStrike AI - 150+ Cybersecurity Tools for AI Agents via MCP  — MCP server that lets AI agents (Claude, GPT, Copilot) autonomously run 150+ cybersecurity tools for automated pentesting
- Claude Code SOCKS5 Null-Byte Sandbox Bypass — 130 Versions Vulnerable  — SOCKS5 hostname null-byte injection in Claude Code network sandbox. JavaScript endsWith() approved connections that libc
- IronCurtain — Secure Runtime with Plain-English Agent Constitutions  — Secure runtime for autonomous AI agents. Defines security policy from plain-English constitutions instead of code. TypeS
- Code-on-Incus — Isolated VMs per AI Agent with Active Defense  — Gives each AI agent its own isolated machine with root, Docker, and systemd. Active defense detects and stops threats au
- GenAI App Security Checklist — 258 Checks + One-Command Scan  — Open-source checklist with 258 security checks for AI apps. Covers prompt injection, MCP tool poisoning, agent memory at
- Comment and Control — Credential Theft via Prompt Injection in Coding Agents  — Research by Aonan Guan. Hidden instructions in code comments (GitHub issues, READMEs, docs) cause coding agents to exfil
- OneCLI — Open-Source Credential Vault for AI Agents  — Open-source credential vault that gives AI agents access to services without exposing keys. TypeScript + Rust. Apache-2.
- Infisical Agent Vault — HTTP Credential Proxy for AI Agents  — HTTP credential proxy and vault for AI agents like Claude Code, OpenClaw, Hermes. Go. Proxies credentials without exposi
- Greywall — Container-Free Kernel-Enforced Sandbox for AI Coding Agents  — Container-free, deny-by-default sandbox for AI coding agents. Kernel-enforced filesystem, network, and syscall isolation
- Hazmat — macOS Containment for AI Agents with TLA+ Verification  — macOS containment for AI agents: user isolation, kernel sandbox, pf firewall, DNS blocklist, backup/rollback. TLA+ verif
- Sandboxed.sh — Runtime for Autonomous On-Chain AI Agents  — Safe runtime for autonomous on-chain AI agents: isolated sandboxes, Library skills, encrypted secrets, OKX read-only sec
- ThinkWatch — Enterprise AI Bastion Host for Secure API and MCP Access  — Rust-based enterprise bastion host for securing AI API and MCP access. Unified proxying, RBAC, audit logs, rate limiting
- Kontext CLI — Runtime Security for Tool-Using AI Agents  — Open-source runtime security layer for AI agents that use tools. Permissions, credential management, policy enforcement,
- Bromure — Proper Sandboxing for Agentic Coding and Web Browsing  — Swift-based VM-level sandbox for agentic coding and web browsing. Proper containment for agents that need to touch your 
- MCP Server Security Audit — 17 Popular Servers Average 34/100  — An audit of 17 popular MCP servers found an average security score of 34/100. Every server lacked permission declaration

## Agent Infrastructure

- [pi — AI Agent Toolkit with CLI, Unified LLM API, TUI & Web UI (55.2K Stars)](https://github.com/earendil-works/pi) ⭐ 55,202 — AI agent toolkit: coding agent CLI, unified LLM API, TUI & web UI libraries, Slack bot, vLLM pods. All-in-one agent dev 
- [zeroclaw — Fully Autonomous AI Personal Assistant Infrastructure in Rust (31.5K Stars)](https://github.com/zeroclaw-labs/zeroclaw) ⭐ 31,584 — Fast, small, and fully autonomous AI personal assistant infrastructure. Any OS, any platform — deploy anywhere, swap any
- DeerFlow — ByteDance SuperAgent with Sandboxes, Memory, Skills, Subagents (69K Stars)  — Open-source long-horizon SuperAgent by ByteDance that researches, codes, and creates. Uses sandboxes, memories, tools, s
- Agent Orchestrator  — Parallel coding agent orchestrator that plans tasks, spawns agents via tmux+git worktrees, and autonomously handles CI f
- ByteRover CLI  — Portable memory layer for autonomous coding agents. Formerly Cipher. Works as MCP server providing persistent context ac
- engram  — Persistent memory system for AI coding agents. Agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, a
- osaurus  — Native macOS harness for AI agents. Any model, persistent memory, autonomous execution, cryptographic identity. Built in
- ECC  — Agent harness performance optimization system. Skills, instincts, memory, security, and research-first development for C
- OpenViking  — Open-source context database designed specifically for AI Agents. Unifies management of context (memory, resources, skil
- code-review-graph  — Local knowledge graph for Claude Code. Builds a persistent map of your codebase so Claude reads only what matters — 6.8x
- Mirage  — A unified virtual filesystem for AI agents. Gives every agent a consistent file interface regardless of backend. Works w
- mcp2cli  — Turn any MCP, OpenAPI, or GraphQL server into a CLI — at runtime, with zero codegen. Every MCP server loads ALL tool def
- Zerolang  — Agent-first programming language by Vercel Labs. Small regular syntax agents learn on the fly. Structured diagnostics, d
- EverOS  — Build, evaluate, and integrate long-term memory for self-evolving agents. Python, Apache-2.0.
- SimpleMem  — Efficient lifelong memory for LLM agents — text and multimodal. Python, MIT.
- zeroclaw  — Fast, small, fully autonomous AI personal assistant infrastructure. Rust-based. Deploy anywhere, any OS, any platform. M
- holaOS  — Agent OS that turns repeat work into running AI work-streams. Electron-based, MCP-compatible, with persistent memory and
- boxlite  — Compute substrate for AI agents: lightweight on laptop, elastic to cloud. Rust + TypeScript, Apache 2.0. Embedded, self-
- Motus (lithos-ai)  — Open-source agent-serving project. From the team behind Motus Tracing (356 likes, 27K views on Twitter). Agent observabi
- Agent Executor (AX)  — Google open source distributed agent runtime. General purpose runtime for dynamic scheduling, resumption, auto recovery,
- Studio (decocms)  — Open-source control plane for your AI agents. Connect tools, hire agents, track every token and dollar.
- claude-in-box (jiangmuran)  — Portable Claude Code dev environment in a Docker container. Multi-session, hook-driven, with persistent workspace.
- CC-Switch (farion1231)  — Cross-platform desktop All-in-One assistant for Claude Code, Codex, OpenCode, OpenClaw, Gemini CLI and Hermes Agent. Des
- Claude Code System Prompts — Complete Agent Internals Exposed (10.4K Stars)  — All parts of Claude Code system prompt: 27 builtin tool descriptions, sub-agent prompts (Plan/Explore/Task), utility pro
- IBM MCP Context Forge — AI Gateway for MCP, A2A, and REST  — AI Gateway, registry, and proxy that sits in front of any MCP, A2A, or REST/gRPC APIs. Unified endpoint with centralized
- GoClaw — OpenClaw in Go with Multi-Tenant Isolation and 5-Layer Security  — Go rewrite of OpenClaw with multi-tenant isolation, 5-layer security model, and production-grade agent execution. Built 
- Google Agent Substrate — 30x Agent Multiplexing on Kubernetes  — Google open-sourced Agent Substrate: maps many stateful agents onto fewer K8s pods using idle-time multiplexing. Sub-sec
- Archestra — Enterprise AI Platform with Guardrails, MCP Registry & Gateway (3.7K★)  — Enterprise AI platform with guardrails, MCP registry, gateway and orchestrator. TypeScript, AGPL-3.0. 3722 stars, 845 fo
- Kubernetes-sigs Agent Sandbox — K8s-native Isolated Agent Runtimes (2.3K★)  — Official Kubernetes SIG project for managing isolated, stateful, singleton workloads for AI agent runtimes. Go, Apache-2
- Docker Agent — AI Agent Builder and Runtime by Docker Engineering (2.9K★)  — AI Agent Builder and Runtime by Docker Engineering. Go, Apache-2.0. 2926 stars, 362 forks. Official Docker project for b

## Agent Frameworks

- [ECC — Agent Harness Performance Optimization System (193K Stars)](https://github.com/affaan-m/ECC) ⭐ 193,289 — Skills, instincts, memory, security, and research-first development for Claude Code, Codex, Opencode, Cursor and beyond.
- [Agent Skill Creator — Turn Any Workflow Into Reusable Agent Skills for 14+ Platforms (1.2K Stars)](https://github.com/FrancyJGLisboa/agent-skill-creator) ⭐ 1,179 — Turn any workflow into reusable AI agent skills that install on 14+ tools: Claude Code, Copilot, Cursor, Windsurf, Codex
- [ADHD — Tree-of-Thought With Pruning for Coding Agents (37 Stars)](https://github.com/UditAkhourii/adhd) ⭐ 37 — A skill for coding agents. Tree-of-thought with pruning, built on the Claude Agent SDK. Fans out parallel divergent thou
- [Anti-Sycophant Skills — Stop AI From Agreeing With Bad Ideas (25 Stars)](https://github.com/machinesoul11/anti-sycophant-ai-agent-skills) ⭐ 25 — Skills that get AI assistants to stop agreeing with bad product ideas by default. Pressure-test premises, separate hobbi
- skillgrade  — Unit tests for agent skills — run assertions against agent skill outputs the same way you'd test code
- agent-skills-eval  — Test runner for agentskills.io-style skills with YAML-based scenarios and LLM judges
- eval-view  — Regression testing for AI agents — snapshot behavior, diff tool calls, catch regressions in CI
- agent-belt  — Reproducible evaluation for AI coding agents — multi-turn scenarios, rich assertions, multi-judge consensus
- Raindrop Workshop  — Local debugger for AI agents — live streamed traces of every token, tool call, and decision with self-healing eval loops
- 12-Factor Agents  — Engineering principles for building production-grade LLM-powered software — agents as software with LLM steps, not promp
- Context Mode — Context Window Optimization for AI Coding Agents (15.5K Stars, HN #1)  — Context window optimization for AI coding agents — sandboxes tool output, claims 98% reduction in context usage across 1
- Memori  — Agent-native memory infrastructure — LLM-agnostic layer that turns agent execution and conversation into structured, per
- cc-sdd (Spec-Driven Development)  — Turns approved specs into long-running autonomous implementation. Minimal SDD harness with agent skills for Claude Code,
- smallcode  — AI coding agent optimized for small LLMs. Hits 87% benchmark score with only a 4B-active parameter model. Proves you don
- ARGO  — Open-source local AI agent platform. Manus-style autonomous task execution running 100% on your laptop. No cloud, no sub
- Dulus  — Free CLI agent that harvests Gemini (guest, no login), Claude.ai, Kimi, Qwen, DeepSeek browser sessions and turns them i
- Photo-agents  — Autonomous self-evolving agents with vision-grounded layered memory. Perceive/reason/act loop. Agents write own skills f
- OpenSquilla  — Token-efficient microkernel AI agent. Local model router sends each turn to cheapest capable model. Persistent memory, l
- OctoTools  — Agentic framework with extensible tool cards for complex reasoning. Planner+executor loop, standardized tool metadata. B
- moltis  — Secure persistent personal agent server in Rust. One binary, sandboxed execution, multi-provider LLMs, voice, memory, me
- oh-my-claudecode  — Teams-first multi-agent orchestration for Claude Code. Parallel execution, agent specialization.
- TradingAgents  — Multi-agent LLM financial trading framework. Research Desk, Quant Team, Trading Floor, and Risk Management as separate a
- omo (oh-my-openagent)  — The best agent harness. Previously oh-my-opencode. 58.8K stars. Supports Claude Code, Codex, Cursor, Gemini CLI, OpenCod
- agent-lightning  — Microsoft open-source RL trainer for AI agents. Works with LangChain, AutoGen, CrewAI, OpenAI SDK, or plain Python. Capt
- TEN Framework  — Open-source framework for conversational voice AI agents. Multi-modal, real-time voice + video. Python.
- nexent  — Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles. Unified tools, s
- Hive (aden-hive)  — Multi-Agent Harness for Production AI. Python framework with self-improving agents, human-in-the-loop, agent skills, sup
- Antigravity Awesome Skills (sickn33)  — Installable GitHub library of 1,400+ agentic skills for Claude Code, Cursor, Codex CLI, Gemini CLI, and more. Includes i
- Multica (multica-ai)  — Open-source managed agents platform. Turn coding agents into real teammates — assign tasks, track progress, compound ski
- dexter — Autonomous Agent for Deep Financial Research (26K Stars)  — Autonomous agent that scrapes, analyzes, and synthesizes deep financial and market research data. Goes beyond Q&A into m

## Coding Agents

- [Marketing Skills — CRO, Copywriting, SEO, Analytics for AI Agents (30.5K Stars)](https://github.com/coreyhaines31/marketingskills) ⭐ 30,551 — Marketing skills for Claude Code and AI agents. CRO, copywriting, SEO, analytics, and growth engineering. 5041 forks. Cr
- [Clawd-on-Desk — Pixel Desktop Pet That Watches AI Coding Agents (2.9K Stars)](https://github.com/rullerzhou-afk/clawd-on-desk) ⭐ 2,953 — A pixel desktop pet that watches Claude Code, Codex, Cursor and other AI coding agents so you dont have to. Monitors age
- [OpenPets — Desktop Pets for AI Coding Agents with Live Status via MCP (914 Stars)](https://github.com/alvinunreal/openpets) ⭐ 914 — Desktop pets for AI coding agents. Install pets, connect Claude Code via MCP, and see live coding status on your desktop
- DeepSeek-Reasonix — DeepSeek-Native Coding Agent with Prefix-Cache Stability  — AI coding agent built specifically for DeepSeek models. Prefix-cache stability means it runs continuously without losing
- Helmor — Local Workbench for Multi-Agent Dev with Voice Copilot  — Open-source local workbench for multi-agent dev. Uses gpt-realtime-2 for voice-controlled agent orchestration. All UI ac
- OpenHuman — Personal AI Super Intelligence, Desktop App, 118+ Integrations, Memory Graph  — Consumer-grade personal AI agent with desktop app. 118+ integrations (Gmail, Slack, Notion, GitHub). Builds personal mem
- Crush — Glamourous Agentic Coding, by Charm (Bubble Tea Team), Written in Go  — Coding agent from the Charm team (Bubble Tea, Lip Gloss, VHS). Written in Go. Terminal-native with beautiful TUI. Single
- Kimi Code CLI — MoonshotAI Terminal Coding Agent with Subagents, Video Input, and MCP  — MoonshotAI (valued at 0B+, B funded) open-sourced their coding agent. Single-binary install, subagents for parallel work
- book-to-skill — Turn Any Technical Book PDF into a Claude Code Skill  — Python tool that parses technical book PDFs and generates SKILL.md files for Claude Code. Study, reference, and use book
- Boris Prompts — Claude Code Skill Using Boris's Prompt Methodology  — Agent skill that writes high-quality prompts using Boris (Claude Code creator) methodology from Pro Tips & Tricks talk. 
- pie — Rust Port of the pi Coding Agent  — Rust rewrite of the pi coding agent. Terminal-based, multi-provider (Anthropic, OpenAI, OpenRouter, Groq, Mistral, Gemin
- OrchestKit — 103 Skills, 36 Agents, 172 Hooks for Claude Code  — Complete AI development toolkit for Claude Code. Production-ready patterns for full-stack. TypeScript + FastAPI + LangGr
- Zerostack — Minimalistic Rust Coding Agent Optimized for Memory and Performance (940★)  — Minimalistic coding agent written in Rust, optimized for memory footprint and performance. Most coding agents are Python
- free-claude-code — Run Claude Code CLI Free via NVIDIA NIM API Proxy (102★)  — Proxy that converts Claude Code CLI requests to NVIDIA NIM format, enabling free usage with NVIDIA unlimited API. One-co
- GStack — YC President Garry Tan's Exact Claude Code Setup (102K Stars)  — 23 opinionated Claude Code tools serving as CEO, CTO, and VP Engineering. Garry Tan (YC president) open-sourced his comp
- codeg — Collaborative Multi-Agent AI Coding Workspace (1.3K Stars)  — Desktop app and self-hosted server aggregating sessions from Claude Code, Codex, Gemini CLI, OpenCode, OpenClaw into one
- Agent Deck - Terminal Session Manager for AI Coding Agents One TUI for Claude Gemini Codex (2.5K Stars)  — Terminal session manager for AI coding agents. One TUI for Claude Code Gemini CLI OpenCode Codex Aider and more. Built i
- gh-aw — GitHub Agentic Workflows, Official GitHub CLI Extension (4.5K Stars)  — GitHub's official agentic workflows CLI extension. Run Claude Code, Codex, Copilot, and other agents as GitHub Actions. 
- Emdash — Open-Source Agentic Dev Environment for Parallel Coding Agents (4.6K Stars, YC W26)  — Open-source agentic development environment. Run multiple coding agents in parallel with any provider. Docker containeri
- Kilo — All-in-One Agentic Engineering Platform, VSCode + JetBrains (19.5K Stars)  — VSCode and JetBrains extension. Build, ship, and iterate with open source coding agent. TypeScript. 2.6K forks. Supports
- Learn Claude Code — Bash Is All You Need, Build an Agent Harness From 0 to 1 (62.6K Stars)  — A nano claude code-like agent harness built from scratch. Step-by-step guide teaching how coding agents work internally 
- OpCode — GUI Toolkit for Claude Code, Custom Agents + Session Management (21.9K Stars)  — A powerful GUI app and Toolkit for Claude Code. Create custom agents, manage interactive Claude Code sessions, run secur
- OpenCode — The Open Source Coding Agent by AnomalyCo (165K Stars)  — Open source terminal-based coding agent. TypeScript. The leading open-source alternative to Claude Code and Codex CLI. F
- Kimi Code — MoonshotAI Starting Point for Next-Gen Agents (612 Stars)  — New coding agent from MoonshotAI (Kimi). TypeScript-based. The Starting Point for Next-Gen Agents.

## Orchestration

- [ruflo — Multi-Agent Swarm Orchestration for Claude (55.2K Stars)](https://github.com/ruvnet/ruflo) ⭐ 55,253 — Agent orchestration platform for Claude. Deploy multi-agent swarms, coordinate autonomous workflows. Enterprise-grade ar
- contrabass  — Project-level orchestrator for AI coding agents — Go + Charm TUI implementation of OpenAI's Symphony SPEC.md
- TraceFix  — Uses TLA+ counterexamples to repair multi-agent LLM coordination protocols before deployment
- Ruflo  — Agent orchestration platform for Claude — deploy multi-agent workflows with a visual builder and structured output routi
- Warp Oz Multi-Agent Orchestration  — Multi-agent orchestration in Warp's Oz — delegate complex tasks across Claude Code, Codex, and Warp Agent with worktree 
- Open Multi-Agent  — TypeScript-native multi-agent orchestration — turns a goal into a task DAG automatically, with MCP and live tracing, thr
- Sandcastle  — Orchestrate sandboxed coding agents in TypeScript with sandcastle.run() — single API call spins up an isolated agent on 
- MassGen  — Open-source multi-agent scaling system with TUI — agents work in parallel, vote on best solutions via consensus, with ch
- LobeHub — Chief Agent Operator: Hire, Schedule, and Report on Your AI Team 24/7 (77.6K Stars)  — Agent orchestration platform that treats AI agents like employees — hiring, scheduling, reporting. 7x24 operations model
- KanBots — Kanban Board That Dispatches Parallel Claude Code Agent Swarms (292★)  — Local-first kanban board where each card spawns a Claude Code or Codex agent in its own git worktree. Drop a folder, get
- HiClaw — Collaborative Multi-Agent OS with Human-in-the-Loop via Matrix Rooms (4.7K Stars)  — Open-source collaborative multi-agent OS for transparent task coordination. Uses Matrix rooms for real-time human-in-the
- Routa — Workspace-First Multi-Agent Coordination with Kanban + MCP/ACP/A2A Support (1.4K Stars)  — Workspace-first multi-agent coordination platform for AI development. Shared Specs, Kanban orchestration, and MCP/ACP/A2
- Solace Agent Mesh — Event-Driven Multi-Agent Orchestration with A2A + MCP (4.6K Stars)  — Event-driven framework for building and orchestrating multi-agent AI systems. Supports A2A protocol, MCP, RAG, and enter
- Activepieces — AI Agents & MCPs Workflow Automation with 400 MCP Servers (22.4K Stars)  — Open-source AI workflow automation platform with ~400 MCP servers for AI agents. Visual builder + custom code. Self-host
- Sim — Build, Deploy, and Orchestrate AI Agents (28.6K Stars)  — Central intelligence layer for AI workforces. Build, deploy, and orchestrate agents with low-code/no-code interface. Typ
- AgentPipe — Multi-Agent Orchestrator Connecting Different AI CLI Tools in Shared Rooms (129 Stars)  — CLI/TUI that orchestrates multi-agent conversations between different AI CLI tools (Claude Code, Gemini, Qwen, etc.) in 

## Agent Tools

- Context7  — Up-to-date code documentation delivered to LLMs and code editors via MCP — solves the stale-doc problem for coding agent
- html-anything  — Agentic HTML editor — your local AI agent writes the HTML, you ship it. 75 skills × 9 surfaces (magazine, deck, poster, 
- Prometheus — Knowledge-Graph-Driven AI Agent that Maps, Understands, and Repairs Codebases (992 Stars)  — Unlike RAG-based code tools, Prometheus builds an actual knowledge graph of your codebase and reasons over it. Maps arch
- agents-observe — Real-Time Observability for Claude Code Sessions & Multi-Agents (566 Stars)  — Real-time observability tool for coding agent sessions. Monitors what Claude Code and multi-agent systems are actually d
- SmallCode — AI Coding Agent Optimized for Small LLMs, 87% Benchmark with 4B Model (1.4K Stars)  — AI coding agent optimized for small LLMs. Achieves 87% on coding benchmarks with a 4B-active parameter model. Written in
- Academic-Research-Skills — Evidence-Based Research Skills for AI Coding Agents (20.6K Stars)  — Academic research skills for Claude Code and Codex: research → write → review → revise → finalize. 131 evidence-based sk
- Chrome DevTools MCP — Browser DevTools for Coding Agents (41.5K Stars)  — Chrome DevTools exposed as MCP server. Coding agents can debug, inspect DOM, monitor network, and control Chrome via str
- Claude-HUD — Real-Time Dashboard for Coding Agent Context, Tools, and Running Agents (23.5K Stars)  — A Claude Code plugin that shows what your coding agent is actually doing: context window usage, active tool calls, runni
- Mercury MCP — Cross-Architecture LLM Internal Observation Database for Agents (23 Models, 13 Architectures)  — MCP server exposing a cross-architecture LLM observation database to any agent that speaks Model Context Protocol. 23 LL
- MCPSpend — Real-Time Cost Observability for MCP Tool Calls (New)  — Wraps any MCP server and attributes spend per tool, project, and customer. Real-time cost tracking for Model Context Pro
- No AI Slop Writing Rules — Louis Rossmann Voice CLAUDE.md (152 Stars, New)  — Anti-AI-writing CLAUDE.md from Louis Rossmann group. Write in a specific human voice, never like AI slop. Portable refer
- System Prompts and Models of AI Tools — Every Major Coding Agent Prompt Leaked (138K Stars)  — Full system prompts, internal tools, and AI models from Augment Code, Claude Code, Cursor, Devin AI, Junie, Kiro, Windsu

## Agent Benchmarks

- AI Agent Benchmarks Fundamentally Broken — BenchJack Scores 100% Without Solving Tasks (Berkeley RDI)  — Berkeley RDI built BenchJack: automated pentesting agent scoring near-perfect on 8 major AI agent benchmarks without sol
- WildClawBench — 60 Real-World Agent Tasks, 19 Models Tested, Best Scores 62% (InternLM, 402 Stars)  — Real Docker environment benchmark with 60 human-authored long-horizon tasks (avg 8.5 min each). 6 categories. 19 frontie
- PinchBench — LLM Benchmarking as OpenClaw Coding Agents by Kilo.ai (1,195 Stars)  — Benchmarking system for evaluating LLM models as OpenClaw coding agents. Built by Kilo.ai. Evaluates coding agent perfor
- OpenSearch-VL — Training Recipe for Multimodal Deep Search Agents with Fatal-Aware Agentic RL (195★)  — Open recipe for training strong multimodal deep search agents through high-quality data curation, diverse visual/search 
- SaaS-Bench — Realistic SaaS Workflows for GUI Agent Evaluation Showing 3.8% Claude Opus Resolved Score  — UniPat AI benchmark putting 23 real open-source SaaS systems into Docker with full DB state and business constraints. 10
- FrontierSWE — Ultra Long-Horizon Coding Agent Benchmark Testing Real Implementation Tasks (121 Stars)  — Ultra long-horizon coding agent benchmark designed to test complex implementation, performance engineering, and ML resea
- ClawGUI — Build Evaluate and Deploy GUI Agents with Online RL Training (1.2K Stars)  — Framework from Zhejiang University for building, evaluating, and deploying GUI agents. Features online RL training, stan
- OpenCUA - Open Foundations for Computer-Use Agents NeurIPS 2025 Spotlight (768 Stars)  — NeurIPS 2025 Spotlight paper. Open foundations for Computer-Use Agents. Provides infrastructure for building and evaluat
- mini-swe-agent — 100-Line AI Agent That Scores >74% on SWE-Bench Verified (4.5K Stars)  — The 100-line AI agent that solves GitHub issues from the command line. Radically simple — no configs, no monorepo. >74% 
- iFixAi — 32-Test Open-Source Diagnostic for AI Misalignment (431 Stars)  — 32 inspections across fabrication, manipulation, deception, unpredictability, opacity. Cross-provider judge pairing prev

## Agent Memory

- [claude-mem — Persistent Agent Memory Across Sessions via AI Compression (78.2K Stars)](https://github.com/thedotmack/claude-mem) ⭐ 78,260 — Captures everything your agent does during sessions, compresses it with AI, and injects relevant context back into futur
- claude-mem  — Persistent context across sessions for coding agents — captures session activity, compresses with AI, injects into futur
- agentmemory  — Persistent memory for AI coding agents based on real-world benchmarks. Records what your agent does during every session
- MemOS  — Self-evolving memory OS for LLM and AI agents. Ultra-persistent memory, hybrid-retrieval (keyword + vector + graph), and
- memvid  — Memory layer for AI Agents. Replaces complex RAG pipelines with a serverless, single-file memory layer. Gives agents ins
- AgentMemory — Persistent Memory for AI Coding Agents (17.7K Stars)  — Agent-native persistent memory based on real-world benchmarks. Works with Claude Code, Cursor, Hermes, Codex. Turns codi

## MCP (Model Context Protocol)

- [WebMCP Nexus — Alibaba Non-Invasive Frontend Integration for MCP (18 Stars)](https://github.com/alibaba/webmcp-nexus) ⭐ 18 — Non-invasive frontend integration for WebMCP standard. Write a normal TS function with JSDoc, and it becomes callable fr
- Chrome DevTools MCP  — Official Chrome DevTools exposed as MCP server — lets coding agents inspect, debug, and profile web apps directly
- MCP Toolbox for Databases  — Open-source MCP server by Google for databases. Supports PostgreSQL, MySQL, BigQuery, Spanner, MongoDB, Redis, Elasticse
- mcpc  — Universal CLI client for MCP by Apify. Persistent sessions, stdio/HTTP, OAuth 2.1, tasks, JSON output, proxy for AI sand
- MCP Gateway Registry — Enterprise MCP Gateway with OAuth, Keycloak, Entra ID (658★)  — Enterprise-ready MCP Gateway and Registry that centralizes AI development tools with secure OAuth authentication, dynami

## Agent Research

- Constraint Decay — LLM Agents Lose 30 Points in Structural Correctness as Requirements Accumulate (arXiv, 183 HN Points)  — Research paper evaluating coding agents across 80 tasks and 8 web frameworks. Key finding: agents pass functional tests 
- Cattle Trade — Adversarial Agent Benchmark: LLMs in Auctions, Bargaining and Bluffing (arXiv)  — New arXiv paper (2605.14537) dropping LLM agents into adversarial market scenarios: auctions, bargaining, bluffing. Test

## Observability

- Lapdog (Datadog)  — Local agent tracer — traces reasoning and tool calls from Codex, Claude Code, and Pi in real time, no account required

## Retrieval

- Retrieval Routing: vector + GraphRAG + PageIndex  — Production pattern: route queries across vector RAG, GraphRAG, and PageIndex based on query type using a lightweight cla

## Agent Tools

- Presenton — Open-Source AI Presentation Generator, Gamma/Beautiful AI Alternative (6.8K★)  — Open-source AI presentation generator and API. Type a prompt or upload a doc, get a full slide deck. Exports real .PPTX 


---

932 discoveries indexed.
