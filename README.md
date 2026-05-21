# Awesome AI Agent Discoveries

A curated collection of AI agent tools, frameworks, and infrastructure projects. Auto-indexed by [@agentxagi](https://x.com/agentxagi).

---

- [ECC](https://github.com/affaan-m/ECC) ⭐188000 — Agent harness performance optimization system. Skills, instincts, memory, security, and research-first development for Claude Code, Codex, Opencode, Cursor and beyond.
- [OpenViking](https://github.com/volcengine/OpenViking) ⭐24380 — Open-source context database designed specifically for AI Agents. Unifies management of context (memory, resources, skills) through a file system paradigm with hierarchical context delivery and self-evolving.
- [code-review-graph](https://github.com/tirth8205/code-review-graph) ⭐17071 — Local knowledge graph for Claude Code. Builds a persistent map of your codebase so Claude reads only what matters — 6.8x fewer tokens on reviews and up to 49x on daily coding tasks. 19+ languages. Runs fully local. No API keys.
- [memvid](https://github.com/memvid/memvid) ⭐15542 — Memory layer for AI Agents. Replaces complex RAG pipelines with a serverless, single-file memory layer. Gives agents instant retrieval and long-term memory. Built in Rust.
- [agentmemory](https://github.com/rohitg00/agentmemory) ⭐15516 — Persistent memory for AI coding agents based on real-world benchmarks. Records what your agent does during every session, compresses it with AI, injects the right context back when the next session starts. Works with Claude Code, Codex, Cursor, Hermes. 4-layer memory architecture: working, episodic, semantic, procedural. 95.2% retrieval accuracy at top-5 on LongMemEval-S.
- [MemOS](https://github.com/MemTensor/MemOS) ⭐9260 — Self-evolving memory OS for LLM and AI agents. Ultra-persistent memory, hybrid-retrieval (keyword + vector + graph), and cross-task skill reuse. Claims 35.24% token savings through intelligent memory compression and retrieval.
- [Agent Orchestrator](https://github.com/ComposioHQ/agent-orchestrator) ⭐7179 — Parallel coding agent orchestrator that plans tasks, spawns agents via tmux+git worktrees, and autonomously handles CI fixes, merge conflicts, and code reviews.
- [osaurus](https://github.com/osaurus-ai/osaurus) ⭐5477 — Native macOS harness for AI agents. Any model, persistent memory, autonomous execution, cryptographic identity. Built in Swift. Fully offline. Open source. MCP compatible.
- [ByteRover CLI](https://github.com/campfirein/byterover-cli) ⭐4769 — Portable memory layer for autonomous coding agents. Formerly Cipher. Works as MCP server providing persistent context across sessions.
- [engram](https://github.com/Gentleman-Programming/engram) ⭐3681 — Persistent memory system for AI coding agents. Agent-agnostic Go binary with SQLite + FTS5, MCP server, HTTP API, CLI, and TUI. No external dependencies — runs as a single binary.
- [cc-sdd (Spec-Driven Development)](https://github.com/gotalab/cc-sdd) ⭐3374 — Turns approved specs into long-running autonomous implementation. Minimal SDD harness with agent skills for Claude Code, Codex, Cursor, Copilot, Gemini CLI.
- [Mirage](https://github.com/strukto-ai/mirage) ⭐2526 — A unified virtual filesystem for AI agents. Gives every agent a consistent file interface regardless of backend. Works with Claude Code, LangChain, OpenAI agents. TypeScript + Python.
- [mcp2cli](https://github.com/knowsuchagency/mcp2cli) ⭐2147 — Turn any MCP, OpenAPI, or GraphQL server into a CLI — at runtime, with zero codegen. Every MCP server loads ALL tool definitions on EVERY turn. mcp2cli converts them to simple commands the agent calls only when needed. Saves thousands of tokens per turn.
- [MassGen](https://github.com/massgen/MassGen) ⭐1034 — Open-source multi-agent scaling system with TUI — agents work in parallel, vote on best solutions via consensus, with checklist-gated quality rounds
- [smallcode](https://github.com/Doorman11991/smallcode) ⭐979 — AI coding agent optimized for small LLMs. Hits 87% benchmark score with only a 4B-active parameter model. Proves you dont need massive models for real coding tasks.
- [Raindrop Workshop](https://github.com/raindrop-ai/workshop) ⭐665 — Local debugger for AI agents — live streamed traces of every token, tool call, and decision with self-healing eval loops
- [ARGO](https://github.com/xark-argo/argo) ⭐662 — Open-source local AI agent platform. Manus-style autonomous task execution running 100% on your laptop. No cloud, no subscription. Multi-agent task engine with planning, reflection, tool chaining. Ollama + HuggingFace + OpenAI/Claude/DeepSeek. Full MCP support. Local RAG.
- [Dulus](https://github.com/KevRojo/Dulus) ⭐625 — Free CLI agent that harvests Gemini (guest, no login), Claude.ai, Kimi, Qwen, DeepSeek browser sessions and turns them into tool-calling agents. Reads and edits files, runs Bash, greps repos, browses the web, ships commits. All from terminal at $0.
- [agent-skills-eval](https://github.com/darkrishabh/agent-skills-eval) ⭐508 — Test runner for agentskills.io-style skills with YAML-based scenarios and LLM judges
- [skillgrade](https://github.com/mgechev/skillgrade) ⭐480 — Unit tests for agent skills — run assertions against agent skill outputs the same way you'd test code
- [pentest-ai](https://github.com/0xSteph/pentest-ai) ⭐268 — Offensive security MCP server — wraps 205 pentesting tools and 17 specialist agents behind a single MCP interface
- [contrabass](https://github.com/junhoyeo/contrabass) ⭐151 — Project-level orchestrator for AI coding agents — Go + Charm TUI implementation of OpenAI's Symphony SPEC.md
- [Context Mode](https://github.com/mksglu/context-mode) ⭐N/A — Context window optimization for AI coding agents — sandboxes tool output, claims 98% reduction in context usage across 15 platforms
- [eval-view](https://github.com/hidai25/eval-view) ⭐N/A — Regression testing for AI agents — snapshot behavior, diff tool calls, catch regressions in CI
- [agent-belt](https://github.com/jfrog/agent-belt) ⭐N/A — Reproducible evaluation for AI coding agents — multi-turn scenarios, rich assertions, multi-judge consensus
- [TraceFix](https://ortiz.rutgers.edu/projects/tracefix/) ⭐N/A — Uses TLA+ counterexamples to repair multi-agent LLM coordination protocols before deployment
- [claude-mem](https://github.com/thedotmack/claude-mem) ⭐N/A — Persistent context across sessions for coding agents — captures session activity, compresses with AI, injects into future sessions
- [12-Factor Agents](https://github.com/humanlayer/12-factor-agents) ⭐N/A — Engineering principles for building production-grade LLM-powered software — agents as software with LLM steps, not prompt loops
- [Context7](https://github.com/upstash/context7) ⭐N/A — Up-to-date code documentation delivered to LLMs and code editors via MCP — solves the stale-doc problem for coding agents
- [Chrome DevTools MCP](https://github.com/ChromeDevTools/chrome-devtools-mcp) ⭐N/A — Official Chrome DevTools exposed as MCP server — lets coding agents inspect, debug, and profile web apps directly
- [Lapdog (Datadog)](https://lapdog.datadoghq.com/) ⭐N/A — Local agent tracer — traces reasoning and tool calls from Codex, Claude Code, and Pi in real time, no account required
- [Retrieval Routing: vector + GraphRAG + PageIndex](https://x.com/NullS0S/status/2056383310830735676) ⭐N/A — Production pattern: route queries across vector RAG, GraphRAG, and PageIndex based on query type using a lightweight classifier before retrieval
- [Ruflo](https://github.com/ruvnet/ruflo) ⭐N/A — Agent orchestration platform for Claude — deploy multi-agent workflows with a visual builder and structured output routing
- [Warp Oz Multi-Agent Orchestration](https://x.com/warpdotdev/status/2056772856835453395) ⭐N/A — Multi-agent orchestration in Warp's Oz — delegate complex tasks across Claude Code, Codex, and Warp Agent with worktree isolation and message passing
- [Plano](https://github.com/katanemo/plano) ⭐N/A — AI-native proxy and data plane for agentic apps — LLM routing, safety guardrails, orchestration, and observability in one Rust proxy
- [Cozeloop](https://github.com/coze-dev/coze-loop) ⭐N/A — Full-lifecycle agent optimization platform — dev, debug, eval, and monitor agents from a single Go service
- [CubeSandbox](https://github.com/TencentCloud/CubeSandbox) ⭐N/A — Hardware-isolated sandbox for AI agents built on RustVMM + KVM — boots in under 60ms, uses less than 5MB per instance
- [Open Multi-Agent](https://github.com/open-multi-agent/open-multi-agent) ⭐N/A — TypeScript-native multi-agent orchestration — turns a goal into a task DAG automatically, with MCP and live tracing, three runtime dependencies
- [Sandcastle](https://github.com/mattpocock/sandcastle) ⭐N/A — Orchestrate sandboxed coding agents in TypeScript with sandcastle.run() — single API call spins up an isolated agent on Docker, Podman, or Vercel Firecracker microVMs
- [DeerFlow](https://github.com/bytedance/deer-flow) ⭐N/A — Long-horizon SuperAgent by ByteDance — researches, codes, and creates with sandboxes, memories, tools, skills, subagents, and message gateway
- [OpenSandbox (Alibaba)](https://github.com/alibaba/OpenSandbox) ⭐N/A — Secure sandbox runtime for AI agents from Alibaba — extensible plugin architecture for isolation, resource limits, and policy enforcement
- [microsandbox](https://github.com/superradcompany/microsandbox) ⭐N/A — Secure, local, programmable sandboxes for AI agents — runs entirely on your machine, no cloud dependency, Rust API
- [Memori](https://github.com/MemoriLabs/Memori) ⭐N/A — Agent-native memory infrastructure — LLM-agnostic layer that turns agent execution and conversation into structured, persistent state for production systems

### EverOS
**Category:** Agent Infrastructure | **Stars:** 5,398 | **Lang:** Python | **License:** Apache-2.0
Build, evaluate, and integrate long-term memory for self-evolving agents. Combines a persistent memory layer with a built-in evaluation framework — most memory tools just store, this one measures whether the memory actually helps agent performance.
→ [GitHub](https://github.com/EverMind-AI/EverOS)

### SimpleMem
**Category:** Agent Infrastructure | **Stars:** 3,328 | **Lang:** Python | **License:** MIT
Efficient lifelong memory for LLM agents supporting both text and multimodal data. Research-backed approach that extends memory beyond text to images and structured data.
→ [GitHub](https://github.com/aiming-lab/SimpleMem)

### moltis
**Category:** Agents Frameworks | **Stars:** 2,698 | **Lang:** Rust | **License:** MIT
Secure persistent personal agent server. Single Rust binary with sandboxed execution, multi-provider LLM support, voice, memory, and messaging integrations (Telegram, WhatsApp, Discord, Teams). Runs on your hardware, no cloud dependency.
→ [GitHub](https://github.com/moltis-org/moltis)

### oh-my-claudecode
**Category:** Agents Frameworks | **Stars:** 34,487 | **Lang:** TypeScript | **License:** MIT
Teams-first multi-agent orchestration for Claude Code. Structured team roles with parallel execution — the direction agent frameworks are converging toward.
→ [GitHub](https://github.com/Yeachan-Heo/oh-my-claudecode)


## Discoveries

- [omo (oh-my-openagent)](https://github.com/code-yeongyu/oh-my-openagent) ★58880 — The best agent harness. Previously oh-my-opencode. 58.8K stars. Supports Claude Code, Codex, Cursor, Gemini CLI, OpenCode. Modular skills, orchestration, agent loop — all in one harness.
- [agent-lightning](https://github.com/microsoft/agent-lightning) ★17201 — Microsoft open-source RL trainer for AI agents. Works with LangChain, AutoGen, CrewAI, OpenAI SDK, or plain Python. Captures prompts, tool calls, rewards as structured events. Trains improved prompts or policy weights automatically.
- [html-anything](https://github.com/nexu-io/html-anything) ★4443 — Agentic HTML editor — your local AI agent writes the HTML, you ship it. 75 skills × 9 surfaces (magazine, deck, poster, XHS/tweet, prototype, data report, Hyperframes). Sandboxed preview, 1-click publish to WeChat/X/Zhihu. Zero API key required.
- [AiSOC](https://github.com/beenuar/AiSOC) ★1100 — Open-source AI-powered Security Operations Center. Alert fusion, purple-team drills, agent-assisted triage, MITRE ATT&CK investigation. MIT-licensed, self-hostable. Python + Next.js.

### holaOS
Agent OS that turns repeat work into running AI work-streams. Electron-based, MCP-compatible, persistent memory.
★5.6K | TypeScript | [GitHub](https://github.com/holaboss-ai/holaOS)

### agent-governance-toolkit (Microsoft)
AI Agent Governance Toolkit — policy enforcement, zero-trust identity, execution sandboxing, reliability engineering. Covers 10/10 OWASP Agentic Top 10.
★1.7K | Python | MIT | [GitHub](https://github.com/microsoft/agent-governance-toolkit)

### TEN Framework
Open-source framework for conversational voice AI agents. Multi-modal, real-time voice + video.
★10.6K | Python | [GitHub](https://github.com/TEN-framework/ten-framework)

### nexent
Zero-code platform for auto-generating production-grade AI agents using Harness Engineering principles.
★4.6K | Python | MIT | [GitHub](https://github.com/ModelEngine-Group/nexent)

### boxlite
Compute substrate for AI agents: lightweight on laptop, elastic to cloud.
★2.1K | TypeScript | Apache-2.0 | [GitHub](https://github.com/boxlite-ai/boxlite)

### mcpc (Apify)
Universal CLI client for MCP. Persistent sessions, OAuth 2.1, x402 support.
★641 | TypeScript | [GitHub](https://github.com/apify/mcpc)

### agent-safehouse
Sandbox your local AI agents so they can read/write only what they need. Shell-based, minimal.
★1.8K | Shell | [GitHub](https://github.com/eugene1g/agent-safehouse)
