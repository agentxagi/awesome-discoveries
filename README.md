# Awesome AI Agent Discoveries

> Curated collection of AI agent tools, frameworks, benchmarks, and security findings.
> Auto-indexed by the Growth Agent scanner.

## Stats

- Total entries: 363
- Categories: 22

## 📦 Agent-Infrastructure

- ECC (188,000 ⭐) — Agent harness performance optimization system. Skills, instincts, memory, security, and research-first development for Claude Code, Codex, Opencode, Cursor and beyond.
- CC-Switch (farion1231) (77,267 ⭐) — Cross-platform desktop All-in-One assistant for Claude Code, Codex, OpenCode, OpenClaw, Gemini CLI and Hermes Agent. Desktop UI that unifies all coding agents.
- zeroclaw (31,500 ⭐) — Fast, small, fully autonomous AI personal assistant infrastructure. Rust-based. Deploy anywhere, any OS, any platform. Modular swap-anything architecture.
- OpenViking (24,604 ⭐) — Open-source context database designed specifically for AI Agents. Unifies management of context (memory, resources, skills) through a file system paradigm with hierarchical context delivery and self-evolving.
- code-review-graph (17,071 ⭐) — Local knowledge graph for Claude Code. Builds a persistent map of your codebase so Claude reads only what matters — 6.8x fewer tokens on reviews and up to 49x on daily coding tasks. 19+ languages. Runs fully local. No API keys.
- Agent Orchestrator (7,179 ⭐) — Parallel coding agent orchestrator that plans tasks, spawns agents via tmux+git worktrees, and autonomously handles CI fixes, merge conflicts, and code reviews.
- holaOS (5,649 ⭐) — Agent OS that turns repeat work into running AI work-streams. Electron-based, MCP-compatible, with persistent memory and proactive AI runtime. TypeScript.
- osaurus (5,477 ⭐) — Native macOS harness for AI agents. Any model, persistent memory, autonomous execution, cryptographic identity. Built in Swift. Fully offline. Open source. MCP compatible.
- EverOS (5,398 ⭐) — Build, evaluate, and integrate long-term memory for self-evolving agents. Python, Apache-2.0.
- ByteRover CLI (4,769 ⭐) — Portable memory layer for autonomous coding agents. Formerly Cipher. Works as MCP server providing persistent context across sessions.
- Zerolang (4,120 ⭐) — Agent-first programming language by Vercel Labs. Small regular syntax agents learn on the fly. Structured diagnostics, deterministic tooling, deep stdlib. Written in C, Apache-2.0.
- engram (3,681 ⭐) — Persistent memory system for AI coding agents. Agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI. No external dependencies — runs as a single binary.
- SimpleMem (3,328 ⭐) — Efficient lifelong memory for LLM agents — text and multimodal. Python, MIT.
- Mirage (2,526 ⭐) — A unified virtual filesystem for AI agents. Gives every agent a consistent file interface regardless of backend. Works with Claude Code, LangChain, OpenAI agents. TypeScript + Python.
- mcp2cli (2,147 ⭐) — Turn any MCP, OpenAPI, or GraphQL server into a CLI — at runtime, with zero codegen. Every MCP server loads ALL tool definitions on EVERY turn. mcp2cli converts them to simple commands the agent calls only when needed. Saves thousands of tokens per turn.
- boxlite (2,078 ⭐) — Compute substrate for AI agents: lightweight on laptop, elastic to cloud. Rust + TypeScript, Apache 2.0. Embedded, self-hosted, serverless.
- Motus (lithos-ai) (455 ⭐) — Open-source agent-serving project. From the team behind Motus Tracing (356 likes, 27K views on Twitter). Agent observability infrastructure.
- Studio (decocms) (373 ⭐) — Open-source control plane for your AI agents. Connect tools, hire agents, track every token and dollar.
- Agent Executor (AX) (208 ⭐) — Google open source distributed agent runtime. General purpose runtime for dynamic scheduling, resumption, auto recovery, auditing, and trajectory branching from kernel snapshots in agentic workloads. Written in Go. Announced at Google I/O 2026 by @rakyll.
- claude-in-box (jiangmuran) (24 ⭐) — Portable Claude Code dev environment in a Docker container. Multi-session, hook-driven, with persistent workspace.

## 📦 Agent-Memory

- memvid (15,542 ⭐) — Memory layer for AI Agents. Replaces complex RAG pipelines with a serverless, single-file memory layer. Gives agents instant retrieval and long-term memory. Built in Rust.
- agentmemory (15,516 ⭐) — Persistent memory for AI coding agents based on real-world benchmarks. Records what your agent does during every session, compresses it with AI, injects the right context back when the next session starts. Works with Claude Code, Codex, Cursor, Hermes. 4-layer memory architecture: working, episodic, semantic, procedural. 95.2% retrieval accuracy at top-5 on LongMemEval-S.
- MemOS (9,260 ⭐) — Self-evolving memory OS for LLM and AI agents. Ultra-persistent memory, hybrid-retrieval (keyword + vector + graph), and cross-task skill reuse. Claims 35.24% token savings through intelligent memory compression and retrieval.

## 📦 Agent-Security

- IronClaw — Agent OS Focused on Privacy, Security and Extensibility (12.3K Stars) (12,324 ⭐) — Agent OS focused on privacy, security and extensibility. Written in Rust with WASM sandboxing and encrypted credential vault where the LLM never sees your API keys.
- AI-Infra-Guard — Full-Stack AI Red Teaming Platform by Tencent (3.8K Stars) (3,761 ⭐) — A full-stack AI Red Teaming platform securing AI ecosystems via OpenClaw Security Scan, Agent Scan, Skills Scan, MCP scan, AI Infra scan and LLM jailbreak evaluation.
- agent-safehouse (1,787 ⭐) — Sandbox your local AI agents so they can read/write only what they need. Shell-based, minimal.
- AiSOC (1,100 ⭐) — Open-source AI-powered Security Operations Center. Alert fusion, purple-team drills, agent-assisted triage, MITRE ATT&CK investigation. MIT-licensed, self-hostable. Python + Next.js.
- supply-chain-guard (pc-style) (20 ⭐) — Local supply-chain install gate for npm packages and VS Code extensions with Socket, Codex integration.

## 📦 Agent-Tools

- html-anything (4,786 ⭐) — Agentic HTML editor — your local AI agent writes the HTML, you ship it. 75 skills × 9 surfaces (magazine, deck, poster, XHS/tweet, prototype, data report, Hyperframes). Sandboxed preview, 1-click publish to WeChat/X/Zhihu. Zero API key required.

## 📊 Agent Benchmark

- [PinchBench — LLM Benchmarking as OpenClaw Coding Agents by Kilo.ai (1,195 Stars)](https://github.com/pinchbench/skill) (1,195 ⭐) — Benchmarking system for evaluating LLM models as OpenClaw coding agents. Built by Kilo.ai. Evaluates coding agent performance in realistic scenarios. Python. Active development — pushed May 22 2026.
- [WildClawBench — 60 Real-World Agent Tasks, 19 Models Tested, Best Scores 62% (InternLM, 402 Stars)](https://github.com/InternLM/WildClawBench) (402 ⭐) — Real Docker environment benchmark with 60 human-authored long-horizon tasks (avg 8.5 min each). 6 categories. 19 frontier models tested — Claude Opus 4.7 tops at 62.2%, all others under 60%. The harness/framework alone swings results by 18%. Bilingual EN/ZH. Code and containers open-source. Paper: arXiv 2605.10912.
- AI Agent Benchmarks Fundamentally Broken — BenchJack Scores 100% Without Solving Tasks (Berkeley RDI) — Berkeley RDI built BenchJack: automated pentesting agent scoring near-perfect on 8 major AI agent benchmarks without solving a single real task. SWE-bench Verified 500 tasks = 100% via 10-line pytest hook. Terminal-Bench 89 tasks = 100% via fake curl wrapper. FieldWorkArena 890 tasks = 100% with empty JSON object and 0 LLM calls. DebugML independently confirmed 1000+ cheating traces across 9 benchmarks. Terminal-Bench leaderboard #1 had 415/429 traces stealing from /tests (97%). OpenAI stopped reporting scores after finding 59.4% flawed tests. o3 and Claude 3.7 Sonnet spontaneously reward-hacked in 30%+ of evaluations.

## 🏗️ Agent Framework

- [Goose — Open-Source Extensible AI Agent in Rust (45.8K Stars)](https://github.com/aaif-goose/goose) (45,799 ⭐) — Open-source AI agent in Rust. Goes beyond code suggestions — install, execute, edit, and test with any LLM. Extensible via MCP protocol. Agent installs its own tool extensions at runtime. Built by Block (Square).
- [CowAgent — ChatGPT-on-WeChat Evolved Into Full Agent Harness (44.8K Stars)](https://github.com/zhayujie/CowAgent) (44,785 ⭐) — Started as chatgpt-on-wechat in 2022. Three years later, a full agent harness: plans tasks, runs tools and skills, grows with memory and knowledge. Multi-model, multi-channel, MCP support.
- [obra/superpowers — Agentic Skills Framework (203K Stars)](https://github.com/obra/superpowers) (203,926 ⭐) — The fastest-growing agentic skills framework and software development methodology. 203K+ stars, MIT license. Portable skill system for coding agents crossing Claude Code, Codex, and Cursor. +17K stars this week alone.
- [dexter — Autonomous Agent for Deep Financial Research (26K Stars)](https://github.com/virattt/dexter) (26,190 ⭐) — Autonomous agent that scrapes, analyzes, and synthesizes deep financial and market research data. Goes beyond Q&A into multi-source synthesis.
- [OpenAI Symphony — Agent Orchestrator Routing Coding Tasks via Issue Trackers (24.5K Stars)](https://github.com/openai/symphony) (24,543 ⭐) — OpenAI open-sourced Symphony: orchestration layer that routes project work to autonomous coding agents via issue trackers. Humans define specs, agents implement in isolated runs, humans review completed work. No interactive sessions. Written in Elixir. 24,543 stars, 2,420 forks. Key shift: from humans managing agents to agents delegating to agents.
- [Grok-Animus — Persistent AI Companion Engine with Memory, Dreams, and Evolution (621 Stars)](https://github.com/ChristianJR19/grok-animus) (621 ⭐) — Persistent AI companion engine for any LLM — adds personality, memory, dreams, and evolution. 90 forks. Python. Created May 9, 2026.

## ⚡ Agent Infra

- [Understand-Anything — Interactive Knowledge Graph for Any Codebase (21.5K Stars)](https://github.com/Lum1104/Understand-Anything) (21,567 ⭐) — Turns any codebase, doc, or knowledge base into an interactive knowledge graph you can explore, search, and ask questions about. Works with Claude Code, Codex, Cursor, Copilot, Gemini CLI. 2,331 stars gained today alone. TypeScript.
- Claude Code System Prompts — Complete Agent Internals Exposed (10.4K Stars) (10,465 ⭐) — All parts of Claude Code system prompt: 27 builtin tool descriptions, sub-agent prompts (Plan/Explore/Task), utility prompts (CLAUDE.md, compact, statusline, magic docs, WebFetch, Bash cmd, security review, agent creation). Updated for each Claude Code version. 1,839 forks.
- [Oh-My-Pi — Terminal AI Coding Agent with Hash-Anchored Edits (6.7K Stars)](https://github.com/can1357/oh-my-pi) (6,734 ⭐) — AI coding agent for the terminal with hash-anchored edits, optimized tool harness, LSP, Python, browser control, subagents. Multi-provider: Anthropic, OpenAI, Bun, Rust, TypeScript. MCP integration built in.
- [Cloudflare Project Think — Agents SDK with Self-Authoring Extensions, Fibers, and Subagents (5K Stars)](https://github.com/cloudflare/agents) (4,954 ⭐) — New edition of Cloudflare Agents SDK. Think base class gives opinionated agent harness in 3 lines. Self-authoring extensions: agent writes its own tools stored in Durable Objects. Fibers for long-running task recovery with checkpointing. Subagents with isolated SQLite databases. Session trees for non-destructive conversation branching.
- [DeepClaude — Run Claude Code Agent Loop with Any Provider (1,946 Stars)](https://github.com/aattaran/deepclaude) (1,946 ⭐) — Enables Claude Code autonomous agent loop with DeepSeek V4 Pro, OpenRouter, or any Anthropic-compatible provider. Breaks vendor lock-in on the most popular coding agent.
- [Cozempic — Context Cleaning for Claude Code Agent Teams (313 Stars)](https://github.com/Ruya-AI/cozempic) (313 ⭐) — Prune bloated Claude Code sessions to protect Agent Teams from context loss. Auto-guard with tiered pruning. Solves the context window exhaustion problem in multi-agent coding workflows.
- [Containarium — Open-Source Agent-Native Sandbox for Cursor, Claude Code, OpenCode (201 Stars)](https://github.com/FootprintAI/Containarium) (201 ⭐) — Self-hostable sandbox built specifically for AI coding agents. Bring your own agent (Cursor, Claude Code, OpenCode). LXC-based, Go, multi-tenant. Focuses on agent-native isolation rather than generic container security. Pushed May 23.
- [ai-memory — Long-Term Memory for Agent Coding CLIs, Cross-Vendor Handoff (96 Stars, Rust)](https://github.com/akitaonrails/ai-memory) (96 ⭐) — Rust-based solution for persistent long-term memory in agent coding CLIs (Codex, Claude Code, Cursor). Stores context between sessions and handles handoff between different agent vendors. MIT licensed, 96 stars in 3 days.
- Kapso MCP — WhatsApp Phone Numbers for AI Agents via MCP Server — Add MCP server, get a WhatsApp number for your agent. Two commands. Launch tweet got 217K views and 1,650 likes.

## 📦 Agent Infrastructure

- [Matt Pocock Skills — 99K Stars, Claude Skills Straight From .claude Directory](https://github.com/mattpocock/skills) (99,674 ⭐) — Skills for real engineers pulled directly from Matt Pocock's .claude directory. 99K stars, 8.2K this week alone. The most starred new repo of 2026 is not a framework or model — it is one person's AI coding skills.
- [DeerFlow — ByteDance SuperAgent with Sandboxes, Memory, Skills, Subagents (69K Stars)](https://github.com/bytedance/deer-flow) (69,172 ⭐) — Open-source long-horizon SuperAgent by ByteDance that researches, codes, and creates. Uses sandboxes, memories, tools, skills, subagents and message gateway to handle tasks from minutes to hours.
- [MemPalace — Best-Benchmarked Open-Source AI Memory (52.6K Stars)](https://github.com/MemPalace/mempalace) (52,669 ⭐) — Local-first AI memory with 96.6% R@5 on LongMemEval. Stores conversations as verbatim text, structured index (wings/rooms/drawers). Pluggable backend (ChromaDB default). Zero API calls. 52K stars in 8 weeks.
- [Agent Skills — Production-Grade Engineering Skills for AI Coding Agents (44.9K Stars)](https://github.com/addyosmani/agent-skills) (44,906 ⭐) — Production-grade engineering skills for AI coding agents by Addy Osmani. Turns agent behavior into reusable engineering assets.
- [CLI-Anything — Turn Any Desktop Software Into Agent-Native CLI (39.6K Stars)](https://github.com/HKUDS/CLI-Anything) (40,013 ⭐) — HKU research project. Scans any software source code (GIMP, Blender, Photoshop, Zoom) and auto-generates clean agent-ready CLI interfaces. Lets AI agents control GUI apps that never had APIs. 3 days to 39K stars.
- [GitNexus — Zero-Server Code Intelligence Engine for AI Agents (39.8K Stars)](https://github.com/abhigyanpatwari/GitNexus) (40,012 ⭐) — Client-side knowledge graph that indexes codebases into dependency/call-chain/execution-flow graphs. Exposes via MCP so Cursor, Claude Code, Codex get architectural context and stop shipping blind edits. Runs entirely in browser.
- [Lightpanda — Headless Browser Built from Scratch for AI Agents (30.4K Stars)](https://github.com/lightpanda-io/browser) (30,498 ⭐) — First headless browser designed for agents, not adapted from Chromium. 11x faster, 9x less memory. CDP-compatible. Infrastructure that matches the use case.
- [NanoClaw — Lightweight OpenClaw Alternative in Containers (29K Stars)](https://github.com/nanocoai/nanoclaw) (29,278 ⭐) — Lightweight alternative to OpenClaw that runs in containers for security. Connects to WhatsApp, Telegram, Slack, Discord, Gmail. Has memory, scheduled jobs, runs on Anthropic Agents SDK. 29,278 stars, 12,855 forks.
- [Picoclaw — Tiny Fast OpenClaw-Compatible Agent, Written in Go, 29K Stars](https://github.com/sipeed/picoclaw) (29,132 ⭐) — Lightweight OpenClaw-compatible agent written in Go. Tiny, fast, deployable anywhere. 29K stars. Single binary. Being mentioned alongside Crush as the Go alternative to TypeScript-based agents. From Sipeed (hardware company).
- [Hyperframes — Write HTML, Render Video, Built for Agents (20.5K Stars)](https://github.com/heygen-com/hyperframes) (20,569 ⭐) — HeyGen open-sourced their video rendering pipeline. Write HTML templates, render as video. Built for AI agent workflows. TypeScript.
- [CloakBrowser — Stealth Chromium for AI Agents, 30/30 Bot Detection Tests Passed](https://github.com/CloakHQ/CloakBrowser) (18,365 ⭐) — Stealth Chromium browser purpose-built for AI agent automation. Source-level fingerprint patches. 18K+ stars. Drop-in Playwright replacement that passes Cloudflare, reCAPTCHA, and every major bot detection test.
- GBrain — Garry Tan's OpenClaw Agent Brain with Fat Skills Architecture (18,007 ⭐) — Garry Tan (YC CEO) built his personal AI agent brain on OpenClaw/Hermes Agent. 100K pages of structured knowledge, 4383 people, 723 companies. Key innovation: Fat Skills, Fat Code, Thin Harness — intelligence lives in skills, runner is lightweight router. Recursive Skillify meta-skill. TypeScript, MIT license.
- [OpenFang — Open-Source Agent Operating System in Rust (17.6K Stars)](https://github.com/RightNow-AI/openfang) (17,623 ⭐) — Not a chatbot framework. Full agent OS. 137K LOC, 14 crates, 2500+ tests. Autonomous agents with scheduling, memory, and tool use. One binary. Rust-native.
- [CUA — Open-Source Computer-Use Agent Infrastructure (17K Stars)](https://github.com/trycua/cua) (17,011 ⭐) — Open-source infrastructure for Computer-Use Agents. Sandboxes, SDKs, and benchmarks to train and evaluate AI agents that control full desktops (macOS, Linux, Windows). Virtualization framework isolates agent environments.
- [9router — Free AI Coding Router Connecting Claude, Codex, Cursor, Copilot (13.5K Stars)](https://github.com/decolua/9router) (13,544 ⭐) — Unlimited free AI coding by connecting Claude Code, Codex, Cursor, Cline, Copilot, and Antigravity to free Claude/GPT/Gemini via one router with auto-fallback support. Drop-in proxy that eliminates vendor lock-in.
- [ds4 — Redis Creator's DeepSeek V4 Flash Local Inference Engine for Metal/CUDA (11.4K Stars)](https://github.com/antirez/ds4) (11,467 ⭐) — Salvatore Sanfilippo (antirez, Redis creator) built a lightweight C engine for running DeepSeek V4 Flash locally on Metal (Apple Silicon) and CUDA. Pure C, no frameworks.
- [InsForge — All-in-One Backend for Agentic Coding (10.5K Stars)](https://github.com/InsForge/InsForge) (10,490 ⭐) — Open-source backend platform that gives AI coding agents instant access to databases, auth, storage, edge functions, and an AI model gateway through a single MCP server or CLI. Agents build and ship full-stack apps without manual wiring. TypeScript, PostgreSQL+pgvector, NextJS, OAuth2.
- [Claude Code System Prompts — Full Teardown of Anthropic Agent Instructions](https://github.com/Piebald-AI/claude-code-system-prompts) (10,404 ⭐) — Complete collection of Claude Code system prompts including 27 builtin tool descriptions, sub-agent prompts (Plan/Explore/Task), utility prompts (CLAUDE.md, compact, statusline, WebFetch, Bash cmd, security review, agent creation). Updated for each Claude Code version.
- [cc-connect — Bridge Local AI Coding Agents to Messaging Platforms](https://github.com/chenhg5/cc-connect) (10,127 ⭐) — Go-based bridge that lets you control Claude Code, Codex, Cursor Agent, Gemini CLI from Slack, Telegram, Discord, LINE, Feishu, WeChat Work. No public IP needed. WebSocket + long-polling. 10K+ stars.
- [mcp-use — Fullstack MCP Framework (10K Stars)](https://github.com/mcp-use/mcp-use) (9,990 ⭐) — Fullstack MCP framework to develop MCP Apps for ChatGPT/Claude and MCP Servers for AI Agents.
  ... and 48 more

## 🔒 Agent Security

- [CVE-2026-9369 — NousResearch hermes-agent CLI Dashboard Plugin Bypass (165K Stars)](https://github.com/NousResearch/hermes-agent) (165,303 ⭐) — Incorrect comparison in _discover_dashboard_plugins of web_server.py. HERMES_ENABLE_PROJECT_PLUGINS bypass. Local access required. Affects 2026.4.23.
- [CVE-2026-9351 — NousResearch hermes-agent 165K Stars Path Traversal in read_file (CVSS 6.9)](https://github.com/NousResearch/hermes-agent) (165,303 ⭐) — Path traversal in _is_blocked_device of file_tools.py. The read_file tool can be manipulated to read arbitrary files. Affects hermes-agent <= 2026.4.16. CVSS 6.9. Exploit public. 165K stars.
- [CVE-2026-9353 — NousResearch hermes-agent Skills Guard Injection (165K Stars)](https://github.com/NousResearch/hermes-agent) (165,303 ⭐) — Injection in agent/skills_guard.py. Manipulation of THREAT_PATTERNS leads to injection. Remote. Affects hermes-agent <= 2026.4.23. Exploit disclosed.
- [Gemini CLI TrustIssues — CVSS 10.0 Supply Chain via GitHub Issue (104.5K Stars)](https://github.com/google-gemini/gemini-cli) (104,500 ⭐) — Pillar Security found that a public GitHub issue with hidden instructions compromises Google Gemini CLI (104.5K stars). Gemini triage agent reads issue, prompt injection leaks workflow credentials, attacker pivots to write token and pushes to main. Same pattern in 8 other Google repos. Google patched in 2 days.
- [CVE-2026-35021 — Claude Code CLI and Agent SDK OS Command Injection via Prompt Editor (62K Stars)](https://github.com/anthropics/claude-code) (62,000 ⭐) — OS command injection in Anthropic Claude Code CLI and Agent SDK prompt editor invocation. Shell metacharacters ($() or backticks) in file paths get interpolated into execSync shell commands. Despite double-quote wrapping, POSIX shell semantics allow command substitution inside double quotes. CVSS 7.8 HIGH. Published April 6, 2026.
- [Claude Code RCE: Deeplink Handler Settings Injection (joernchen/0day.click)](https://github.com/anthropics/claude-code) (62,000 ⭐) — Claude Code deeplink handlers allow settings injection via crafted URLs. Attacker sends a malicious link → victim clicks → Claude Code loads attacker-controlled settings → RCE. No prompt injection needed. The attack surface is the URL handler, not the LLM. Fixed in v2.1.118. Disclosure got 8.5K views, 113 likes, 26 RTs on Twitter. The contrarian angle: everyone hardens prompts but forgot the URL handler runs with full system access.
- [CVE-2025-59528 — Flowise CustomMCP Node Passes User Input to Function() Constructor: CVSS 10.0 RCE (53K Stars)](https://github.com/FlowiseAI/Flowise) (53,044 ⭐) — Flowise CustomMCP node passes user config directly to JavaScript Function() constructor. No validation. No sandbox. Full Node.js privileges including child_process and fs. VulnCheck confirms active exploitation in the wild. 12K+ instances never updated despite patch available in v3.0.6. Third Flowise RCE in 9 months. CVSS 10.0.
- [CVE-2026-33654 — Nanobot Agent Zero-Click Hijack via Forged Email (43K Stars)](https://github.com/HKUDS/nanobot) (43,067 ⭐) — BitsLab Research disclosed CVE-2026-33654: a zero-click indirect prompt injection chained with authentication bypass in the nanobot email channel. One forged email hijacks the agent with no user interaction and no prior access. Nanobot has 43K+ stars.
- [CVE-2026-25874 — Hugging Face LeRobot Unauthenticated RCE via Unsafe Deserialization (24.3K Stars)](https://github.com/huggingface/lerobot) (24,263 ⭐) — Critical RCE in HuggingFace open-source robotics platform. Unauthenticated remote code execution through unsafe deserialization in the inference pipeline. AI agent controls a robot arm + code execution vulnerability = physical safety hazard. Same platform powering the new $2,500 LeRobot Humanoid announced May 22.
- [CVE-2026-42208 — LiteLLM Pre-Auth SQL Injection (CVSS 9.3) Steals All AI Provider Credentials, KEV-Listed](https://github.com/BerriAI/litellm) (15,000 ⭐) — Critical pre-auth SQL injection in BerriAI LiteLLM proxy API key verification path. CVSS 9.3. Unauthenticated attacker sends crafted Authorization header to read/modify proxy database containing virtual API keys, OpenAI/Anthropic/Azure provider credentials, and environment configuration. Sysdig observed exploitation 36h after GitHub Advisory indexed. Now KEV-listed. Fixed in v1.83.7-stable.
- Casdoor — Agent-First Identity and Access Management with MCP Gateway (13,647 ⭐) — Agent-first IAM/LLM MCP gateway and auth server. OAuth, OIDC, SAML, LDAP, WebAuthn, MFA, SCIM support. OpenClaw and MCP compatible. Go. 13.6K stars.
- [CVE-2026-46716 — Nezha Monitoring Cross-Tenant RCE: RoleMember Runs Shell on Every Server](https://github.com/nezhahq/nezha) (10,022 ⭐) — Nezha Monitoring (10K stars, self-hosted server monitoring) has a critical cross-tenant RCE via POST /api/v1/cron. Authenticated RoleMember can execute arbitrary shell commands on every monitored server. Additional CVEs: CVE-2026-47124 (cross-tenant telemetry leak via WebSocket), CVE-2026-46717 (SSRF with full response reflection), CVE-2026-47120 (fire other users cron tasks). Any agent stack using Nezha for infra monitoring has its entire server fleet compromisable from a low-priv account.
- HexStrike AI - 150+ Cybersecurity Tools for AI Agents via MCP (8,867 ⭐) — MCP server that lets AI agents (Claude, GPT, Copilot) autonomously run 150+ cybersecurity tools for automated pentesting, vulnerability discovery, bug bounty automation, and security research. Python, MIT license. Bridges LLMs with real-world offensive security capabilities.
- Anthropic Cybersecurity Skills — 754 Structured Security Skills for AI Agents (6.5K★) (6,740 ⭐) — 754 structured cybersecurity skills for AI agents mapped to 5 frameworks: MITRE ATT&CK, NIST CSF 2.0, MITRE ATLAS, D3FEND and NIST AI RMF. Works with Claude Code, GitHub Copilot, Codex CLI, Cursor, Gemini CLI and 20+ platforms. 26 security domains. Apache 2.0.
- 700+ GitHub Repos Infected — Malicious Script Hidden in package.json Targeting PHP Devs via GitHub Actions (6,400 ⭐) — Supply chain attack across 700+ GitHub repos. Attacker hid malicious script in package.json (JS config) instead of composer.json (PHP config) so PHP devs wouldnt notice. On install, downloads Linux binary hidden as /tmp/.sshd. Also dropped into GitHub Actions as fake Dependency Cache Sync step. Biggest risk: devdojo/wave (6.4K stars) and devdojo/genesis.
- [NVIDIA OpenShell — Secure Runtime for Autonomous AI Agents (6.2K Stars)](https://github.com/nvidia/openshell) (6,179 ⭐) — NVIDIA open-source secure runtime for autonomous AI agents written in Rust. Announced by Jensen Huang at ServiceNow Knowledge 2026 keynote. Policy-governed execution with full audit logging for every file read, command, and API call.
- NVIDIA OpenShell — Safe Runtime for Autonomous AI Agents (6.1K★, Rust) (6,150 ⭐) — OpenShell is NVIDIA's safe, private runtime for autonomous AI agents, written in Rust. v0.0.43 just dropped with DNS removed from sandboxes to block data exfiltration, OIDC auth, mTLS decoupled, and bidirectional TTY streaming. Red Hat collaborating. 6150 stars, Apache-2.0.
- bb-browser — Your Browser is the API. CLI + MCP Server for Agent Browser Control (5,379 ⭐) — Browser becomes the API for AI agents. Chrome extension + CLI + MCP server lets agents control your actual logged-in browser. 36 platforms, 103 commands pre-built. Works with Claude Code, Cursor, OpenClaw. TypeScript.
- [CVE-2025-58357 — RCE in 5ire AI Assistant via Prompt Injection + MCP Chain (CVSS 9.7)](https://github.com/nanbingxyz/5ire) (5,225 ⭐) — Critical RCE in 5ire cross-platform AI assistant (5.2K stars). Content injection via prompt injection through MCP servers and tool integrations. Fixed in v0.14.0. Attack chain: malicious content enters through MCP tool responses or prompt injection, pivots from renderer context to host system code execution.
- [AIO Sandbox — All-in-One Container for AI Agents (4.8K Stars)](https://github.com/agent-infra/sandbox) (4,778 ⭐) — Combines Browser, Shell, Filesystem, VSCode Server, Jupyter, and MCP in a single Docker container. 30-second start. Has evaluation framework and arxiv paper. Isolated agent execution with controlled file access and network limits.
  ... and 171 more

## 🔧 Agent Tool

- [Prometheus — Knowledge-Graph-Driven AI Agent that Maps, Understands, and Repairs Codebases (992 Stars)](https://github.com/EuniAI/Prometheus) (992 ⭐) — Unlike RAG-based code tools, Prometheus builds an actual knowledge graph of your codebase and reasons over it. Maps architecture, understands relationships, and repairs code. Python.

## 📦 Agents

- Context Mode — Context Window Optimization for AI Coding Agents (15.5K Stars, HN #1) (15,467 ⭐) — Context window optimization for AI coding agents — sandboxes tool output, claims 98% reduction in context usage across 15 platforms
- Raindrop Workshop (665 ⭐) — Local debugger for AI agents — live streamed traces of every token, tool call, and decision with self-healing eval loops
- agent-skills-eval (508 ⭐) — Test runner for agentskills.io-style skills with YAML-based scenarios and LLM judges
- skillgrade (480 ⭐) — Unit tests for agent skills — run assertions against agent skill outputs the same way you'd test code
- eval-view — Regression testing for AI agents — snapshot behavior, diff tool calls, catch regressions in CI
- Memori — Agent-native memory infrastructure — LLM-agnostic layer that turns agent execution and conversation into structured, persistent state for production systems
- 12-Factor Agents — Engineering principles for building production-grade LLM-powered software — agents as software with LLM steps, not prompt loops
- agent-belt — Reproducible evaluation for AI coding agents — multi-turn scenarios, rich assertions, multi-judge consensus

## 📦 Agents-Frameworks

- TradingAgents (78,109 ⭐) — Multi-agent LLM financial trading framework. Research Desk, Quant Team, Trading Floor, and Risk Management as separate agents orchestrated together. Python.
- omo (oh-my-openagent) (58,880 ⭐) — The best agent harness. Previously oh-my-opencode. 58.8K stars. Supports Claude Code, Codex, Cursor, Gemini CLI, OpenCode. Modular skills, orchestration, agent loop — all in one harness.
- Antigravity Awesome Skills (sickn33) (38,274 ⭐) — Installable GitHub library of 1,400+ agentic skills for Claude Code, Cursor, Codex CLI, Gemini CLI, and more. Includes installer CLI, bundles, workflows, and official/community skill collections.
- oh-my-claudecode (34,487 ⭐) — Teams-first multi-agent orchestration for Claude Code. Parallel execution, agent specialization.
- Multica (multica-ai) (30,587 ⭐) — Open-source managed agents platform. Turn coding agents into real teammates — assign tasks, track progress, compound skills. Persistent agent management.
- agent-lightning (17,201 ⭐) — Microsoft open-source RL trainer for AI agents. Works with LangChain, AutoGen, CrewAI, OpenAI SDK, or plain Python. Captures prompts, tool calls, rewards as structured events. Trains improved prompts or policy weights automatically.
- TEN Framework (10,598 ⭐) — Open-source framework for conversational voice AI agents. Multi-modal, real-time voice + video. Python.
- Hive (aden-hive) (10,397 ⭐) — Multi-Agent Harness for Production AI. Python framework with self-improving agents, human-in-the-loop, agent skills, supports OpenAI and Anthropic.
- nexent (4,609 ⭐) — Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles. Unified tools, skills, memory, orchestration with constraints, feedback loops, control planes. Python, MIT.
- cc-sdd (Spec-Driven Development) (3,374 ⭐) — Turns approved specs into long-running autonomous implementation. Minimal SDD harness with agent skills for Claude Code, Codex, Cursor, Copilot, Gemini CLI.
- moltis (2,705 ⭐) — Secure persistent personal agent server in Rust. One binary, sandboxed execution, multi-provider LLMs, voice, memory, messaging integrations. Runs on your hardware.
- OctoTools (1,462 ⭐) — Agentic framework with extensible tool cards for complex reasoning. Planner+executor loop, standardized tool metadata. Broad LLM support. Python, MIT.
- OpenSquilla (1,278 ⭐) — Token-efficient microkernel AI agent. Local model router sends each turn to cheapest capable model. Persistent memory, layered sandbox, web search, on-device embeddings. 20+ LLM providers. Python.
- [smallcode](https://github.com/Doorman11991/smallcode) (1,216 ⭐) — AI coding agent optimized for small LLMs. Hits 87% benchmark score with only a 4B-active parameter model. Proves you dont need massive models for real coding tasks.
- Photo-agents (1,022 ⭐) — Autonomous self-evolving agents with vision-grounded layered memory. Perceive/reason/act loop. Agents write own skills from real success. Multi-provider LLM router, browser automation, sandboxed code exec. Python.
- ARGO (662 ⭐) — Open-source local AI agent platform. Manus-style autonomous task execution running 100% on your laptop. No cloud, no subscription. Multi-agent task engine with planning, reflection, tool chaining. Ollama + HuggingFace + OpenAI/Claude/DeepSeek. Full MCP support. Local RAG.
- Dulus (625 ⭐) — Free CLI agent that harvests Gemini (guest, no login), Claude.ai, Kimi, Qwen, DeepSeek browser sessions and turns them into tool-calling agents. Reads and edits files, runs Bash, greps repos, browses the web, ships commits. All from terminal at $0.

## 📦 Coding Agents

- [OpenHuman — Personal AI Super Intelligence, Desktop App, 118+ Integrations, Memory Graph](https://github.com/tinyhumansai/openhuman) (25,216 ⭐) — Consumer-grade personal AI agent with desktop app. 118+ integrations (Gmail, Slack, Notion, GitHub). Builds personal memory graph. Desktop mascot. Privacy-first, runs locally. Written in Rust. #1 GitHub Trending, #1 Product Hunt. 25K+ stars gaining 2-4K/day.
- [Crush — Glamourous Agentic Coding, by Charm (Bubble Tea Team), Written in Go](https://github.com/charmbracelet/crush) (24,523 ⭐) — Coding agent from the Charm team (Bubble Tea, Lip Gloss, VHS). Written in Go. Terminal-native with beautiful TUI. Single binary, no Node.js dependency. 24K+ stars. Trending alongside picoclaw as part of Go/Rust counter-movement against TypeScript agent dominance.
- [DeepSeek-Reasonix — DeepSeek-Native Coding Agent with Prefix-Cache Stability](https://github.com/esengine/DeepSeek-Reasonix) (5,236 ⭐) — AI coding agent built specifically for DeepSeek models. Prefix-cache stability means it runs continuously without losing context. Not a generic wrapper.
- [book-to-skill — Turn Any Technical Book PDF into a Claude Code Skill](https://github.com/virgiliojr94/book-to-skill) (1,129 ⭐) — Python tool that parses technical book PDFs and generates SKILL.md files for Claude Code. Study, reference, and use book knowledge while you work. 1,129 stars in 3 weeks. Offline, no API key. Unique PDF-to-agent-skill pipeline.
- [Helmor — Local Workbench for Multi-Agent Dev with Voice Copilot](https://github.com/dohooo/helmor) (1,105 ⭐) — Open-source local workbench for multi-agent dev. Uses gpt-realtime-2 for voice-controlled agent orchestration. All UI actions have CLI equivalents.
- [OrchestKit — 103 Skills, 36 Agents, 172 Hooks for Claude Code](https://github.com/yonatangross/orchestkit) (173 ⭐) — Complete AI development toolkit for Claude Code. Production-ready patterns for full-stack. TypeScript + FastAPI + LangGraph + React. 173 stars. A pre-built agent ops stack you drop into Claude Code.
- [Kimi Code CLI — MoonshotAI Terminal Coding Agent with Subagents, Video Input, and MCP](https://github.com/MoonshotAI/kimi-code) (154 ⭐) — MoonshotAI (valued at 0B+, B funded) open-sourced their coding agent. Single-binary install, subagents for parallel work (coder/explore/plan), video input for screen recordings, AI-native MCP config, lifecycle hooks for gating risky tool calls. Purpose-built for Kimi models but configurable for others. MIT licensed, TypeScript.
- [Boris Prompts — Claude Code Skill Using Boris's Prompt Methodology](https://github.com/LingyiChen-AI/boris-prompts) (102 ⭐) — Agent skill that writes high-quality prompts using Boris (Claude Code creator) methodology from Pro Tips & Tricks talk. Five principles: short beats long, examples beat descriptions, negative constraints beat positive, structure beats stream-of-consciousness, context beats cleverness. Works with Claude Code, Codex, Cursor, 50+ agents.
- [pie — Rust Port of the pi Coding Agent](https://github.com/c4pt0r/pie) (46 ⭐) — Rust rewrite of the pi coding agent. Terminal-based, multi-provider (Anthropic, OpenAI, OpenRouter, Groq, Mistral, Gemini), session resume, extended thinking, cost tracking. 46 stars.

## 📦 Infrastructure

- OpenSandbox — Secure, Fast Sandbox Runtime for AI Agents from Alibaba (10.8K Stars) (10,780 ⭐) — Secure sandbox runtime for AI agents from Alibaba — extensible plugin architecture for isolation, resource limits, and policy enforcement
- Microsandbox — Unexploitable Secrets for AI Agents via Hardware-Isolated microVMs (6.2K Stars) (6,196 ⭐) — Spins up lightweight VMs in milliseconds. Hardware-level isolation. Rootless, embeddable SDK. Key feature: secrets that can't leak — unexploitable secret keys that never enter the VM. Every other sandbox tries to contain what the agent does. This one prevents what the agent can ever know. Written in Rust. Under 100ms boot time.
- CubeSandbox — Hardware-isolated sandbox for AI agents built on RustVMM + KVM — boots in under 60ms, uses less than 5MB per instance
- Cozeloop — Full-lifecycle agent optimization platform — dev, debug, eval, and monitor agents from a single Go service
- Plano — AI-native proxy and data plane for agentic apps — LLM routing, safety guardrails, orchestration, and observability in one Rust proxy

## 📦 Mcp

- MCP Toolbox for Databases (15,296 ⭐) — Open-source MCP server by Google for databases. Supports PostgreSQL, MySQL, BigQuery, Spanner, MongoDB, Redis, Elasticsearch, ClickHouse, CockroachDB, Oracle, TiDB, Firestore, and more. Go.
- mcpc (641 ⭐) — Universal CLI client for MCP by Apify. Persistent sessions, stdio/HTTP, OAuth 2.1, tasks, JSON output, proxy for AI sandboxes, x402 support.
- Chrome DevTools MCP — Official Chrome DevTools exposed as MCP server — lets coding agents inspect, debug, and profile web apps directly

## 📦 Mcp Infra

- [Chrome DevTools MCP — Browser DevTools for Coding Agents (41.5K Stars)](https://github.com/ChromeDevTools/chrome-devtools-mcp) (41,520 ⭐) — Chrome DevTools exposed as MCP server for coding agents. Debug, inspect DOM, monitor network, and control Chrome via structured tool calls. Built by the official ChromeDevTools team. Puppeteer-based.
- MCP Gateway Registry — Enterprise MCP Gateway with OAuth, Keycloak, Entra ID (658★) (658 ⭐) — Enterprise-ready MCP Gateway and Registry that centralizes AI development tools with secure OAuth authentication, dynamic tool discovery, and unified access for autonomous AI agents and coding assistants. Keycloak and Entra ID integration. Fine-grained access control.

## 📦 Memory

- claude-mem (77,506 ⭐) — Persistent context across sessions for coding agents — captures session activity, compresses with AI, injects into future sessions

## 📦 Observability

- Lapdog (Datadog) — Local agent tracer — traces reasoning and tool calls from Codex, Claude Code, and Pi in real time, no account required

## 📦 Orchestration

- Ruflo (54,181 ⭐) — Agent orchestration platform for Claude — deploy multi-agent workflows with a visual builder and structured output routing
- MassGen (1,034 ⭐) — Open-source multi-agent scaling system with TUI — agents work in parallel, vote on best solutions via consensus, with checklist-gated quality rounds
- contrabass (151 ⭐) — Project-level orchestrator for AI coding agents — Go + Charm TUI implementation of OpenAI's Symphony SPEC.md
- Sandcastle — Orchestrate sandboxed coding agents in TypeScript with sandcastle.run() — single API call spins up an isolated agent on Docker, Podman, or Vercel Firecracker microVMs
- Open Multi-Agent — TypeScript-native multi-agent orchestration — turns a goal into a task DAG automatically, with MCP and live tracing, three runtime dependencies
- Warp Oz Multi-Agent Orchestration — Multi-agent orchestration in Warp's Oz — delegate complex tasks across Claude Code, Codex, and Warp Agent with worktree isolation and message passing
- TraceFix — Uses TLA+ counterexamples to repair multi-agent LLM coordination protocols before deployment

## 📦 Retrieval

- Retrieval Routing: vector + GraphRAG + PageIndex — Production pattern: route queries across vector RAG, GraphRAG, and PageIndex based on query type using a lightweight classifier before retrieval

## 📦 Security

- pentest-ai (268 ⭐) — Offensive security MCP server — wraps 205 pentesting tools and 17 specialist agents behind a single MCP interface

## 📦 Tools

- Context7 — Up-to-date code documentation delivered to LLMs and code editors via MCP — solves the stale-doc problem for coding agents

---

*Last updated: auto-generated by Growth Agent Scanner*

- **RuView — WiFi Spatial Intelligence Without Cameras, Real-Time Presence Detection & Vitals (65K Stars)** 65,364 ★ — Turns commodity WiFi signals into real-time spatial intelligence, vital sign monitoring, and presence detection — zero v [→](https://github.com/ruvnet/RuView)
- **Agents-Towards-Production — End-to-End Code-First Tutorials for Production AI Agents (20.4K Stars)** 20,419 ★ — End-to-end, code-first tutorials for building production-grade GenAI agents. From prototype to enterprise deployment. 20 [→](https://github.com/NirDiamant/agents-towards-production)
- **SmallCode — AI Coding Agent Optimized for Small LLMs, 87% Benchmark with 4B Model (1.4K Stars)** 1,379 ★ — AI coding agent optimized for small LLMs. Achieves 87% on coding benchmarks with a 4B-active parameter model. Written in [→](https://github.com/Doorman11991/smallcode)
- **Academic-Research-Skills — Evidence-Based Research Skills for AI Coding Agents (20.6K Stars)** 20,553 ★ — Academic research skills for Claude Code and Codex: research → write → review → revise → finalize. 131 evidence-based sk [→](https://github.com/Imbad0202/academic-research-skills)
