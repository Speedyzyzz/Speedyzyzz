<div align="center">

# Balavignesh

### Product Engineer • Full-Stack Systems • Agentic AI Architectures

<p align="center">
  <a href="https://balavignesh.dev"><img src="https://img.shields.io/badge/Portfolio-balavignesh.dev-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/balavignesh-v-t-72b157297/"><img src="https://img.shields.io/badge/LinkedIn-Balavignesh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/Speedyzyzz"><img src="https://img.shields.io/badge/GitHub-Speedyzyzz-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
</p>

```
TypeScript  •  Next.js 15  •  React 19  •  Python  •  FastAPI  •  PostgreSQL  •  Redis  •  Docker
```

</div>

---

## ⚡ TL;DR

I am a **Product Engineer** based in India who builds high-velocity web platforms, resilient distributed backends, and agentic AI systems. I treat language models as untrusted, schema-bounded workers and focus on deterministic reliability, asynchronous concurrency safety, and snappy, accessible user interfaces.

- 💼 **Current Role:** Associate Product Engineer at **Zenthiran** — Architected multi-portal authentication, cross-domain session hydration, and token concurrency barriers.
- 🏛️ **Previous Experience:** Full Stack & AI Associate at **SNS iHubs** — Built automated multi-agent pipelines and rapid incubator MVPs.
- 🚀 **Production Proof:** [gdta2026.com](https://gdta2026.com) (Next.js 15 + Three.js 3D WebGL), [balavignesh.dev](https://balavignesh.dev).

---

## 🛠️ Flagship Systems & Frontier Runtimes

### 1. ⏱️ [Chronicle](https://github.com/Speedyzyzz/chronicle) — Deterministic Record-and-Replay Runtime for Coding Agents
> **FastAPI • Next.js 15 • Python 3.11+ • BLAKE3 • Lamport/Vector Clocks • 100% ChronicleBench Convergence**
- **Causal Event Ledger:** Intercepts every tool call, environment read, and subprocess mutation into an append-only event stream ordered by Lamport and vector clocks.
- **Content-Addressed State Trees:** Hashes filesystem mutations and deltas via streaming BLAKE3 hashing, enabling instant point-in-time state rollback.
- **Pure Replay & Divergence Localization:** Reproduces past agent executions with **zero external LLM API calls** by re-hydrating causal inputs from the ledger, pinpointing divergence within $\pm 0$ events.
- **Verification:** 13/13 Pytest suite passing offline and 40/40 benchmark tasks passing on `ChronicleBench` (100% convergence).

### 2. 🛡️ [Aegis Runtime](https://github.com/Speedyzyzz/aegis-runtime) — Policy-Enforcing Transaction Layer & Runtime Authorization Guardrail
> **FastAPI • Next.js 15 • Action IR • Two-Phase Commit • BLAKE3 Merkle Audit • 100% AegisBench Defense**
- **Typed Action IR & Quantitative Blast Radius:** Intercepts raw tool calls and normalizes them into canonical typed IR across SQL, Filesystem, HTTP, and Shell with quantitative risk scoring (0–100).
- **Two-Phase Commit & Scoped Attenuation:** Enforces a prepare/commit boundary with single-use, TTL-attenuated cryptographic capability tokens that eliminate TOCTOU race conditions.
- **Cryptographic Audit Chain:** Generates append-only BLAKE3 Merkle-linked audit receipts for every executed action, providing tamper-evident proof of compliance.
- **Adversarial Benchmark:** 100/100 adversarial cases defended on `AegisBench` (0% unauthorized side effects, 0 duplicate executions).

### 3. 🤖 [DevAgent](https://github.com/Speedyzyzz/devagent) — Policy-Constrained Autonomous Software-Engineering Runtime
> **Next.js 15 App Router • React 19 • FastAPI • Python 3.11+ • Sandboxed Tools • 100% Benchmark Resolution**
- **Autonomous Debugging Runtime:** Governs an LLM through deterministic filesystem exploration, lexical search (`ripgrep` with regex fallback), AST-validated atomic patchers, and subprocess test runners.
- **Empirical Benchmark Proof:** Tested against a 5-bug benchmark evaluation suite with a **100% verified resolution rate (5/5 bugs passed)** in under 6 turns average.
- **Defensive Sandbox:** Enforces strict realpath isolation, blocking path traversals (`../../`), external symlink escapes, and `.env`/`.git` access.
- **Mission Control UI:** Next.js 15 interface streaming real-time Server-Sent Events (SSE) telemetry, collapsible tool accordions, and unified diff syntax viewers.
- **Verification:** 33/33 automated tests passing across tool contracts, security perimeters, and multi-turn engine loops.

### 4. 🔀 [PatchBay](https://github.com/Speedyzyzz/patchbay) — Semantic API-Evolution & AST Migration Infrastructure
> **FastAPI • Next.js 15 • LibCST • TypeScript Compiler AST • OpenAPI Diff • 100% API-MigrateBench Pass**
- **Whole-Repo Call-Site Graph:** Parses monorepo source files via LibCST to construct a bidirectional API usage graph connecting consumers to breaking endpoints.
- **Contract Diffing & Synthesis:** Computes breaking schema diffs between upstream API versions and synthesizes minimal, type-safe AST rewrites preserving formatting and comments.
- **Empirical Benchmark Proof:** 50/50 breaking-change tasks passed on `API-MigrateBench` with 100% typecheck recovery and 0.85 average diff ratio.

### 5. 🐝 [HiveMind](https://github.com/Speedyzyzz/hivemind) — Collaborative Multiplayer Durable-Agent Runtime
> **FastAPI • WebSocket Gateway • Yjs CRDTs • Event-Sourced FSM • Distributed Leases • HiveBench Verified**
- **Decoupled Architecture:** Separates human/agent collaborative intent editing (via Yjs CRDTs) from authoritative tool execution managed by an event-sourced FastAPI FSM.
- **Distributed Leases & Crash Recovery:** Grants atomic, TTL-heartbeat execution leases to active agents with automatic watchdog eviction upon worker failure.
- **Human Intervention Controls:** Seamlessly pause, steer, or seize execution authority mid-flight without corrupting state or leaving orphaned subprocesses.
- **Stress-Tested:** Verified across 50 concurrent virtual actors and simulated worker crash scenarios with 0 lease collisions.

### 6. 🧪 [ForgeLab](https://github.com/Speedyzyzz/forgelab) — Ephemeral Production-Faithful Test Environments
> **FastAPI • Next.js 15 • Copy-on-Write Database Clones • HTTP Replay Proxy • Sub-Second Cold Start**
- **Sub-Second Database Replicas:** Provisions lightweight copy-on-write SQLite/Postgres clones with deterministic keyed pseudonymization preserving relational foreign keys.
- **HTTP Dependency Recording & Replay:** Captures external outbound traffic and replays deterministic network fixtures with programmable fault injection (latency, 500/504 errors).
- **Leak-Proof Watchdog:** Automatically sweeps orphaned containers, ports, and temporary volumes upon agent termination or crash.
- **Benchmark (`ForgeBench`):** 20/20 defect scenarios detected with 0.17ms p95 cold-start latency.

### 7. 🎙️ [MeetSync](https://github.com/Speedyzyzz/meetsync) — Enterprise Meeting Intelligence Platform
> **Next.js 15 App Router • React 19 • FastAPI • PostgreSQL 16 FTS • Redis 7 • Pydantic v2 • Docker**
- **Defensive Extraction:** Ingests raw meeting transcripts and audio files with strict Pydantic v2 schemas and prompt injection boundary fences.
- **7-Stage Finite State Machine:** Managed background processing pipeline (`UPLOADED` → `TRANSCRIBING` → `EXTRACTING` → `INDEXING` → `COMPLETED`) offloaded to asynchronous Redis worker daemons.
- **Enterprise Isolation:** Multi-tenant PBKDF2/JWT isolation, lexical PostgreSQL `tsvector` full-text search, and bidirectional timestamp citations linking tasks to verbatim transcript lines.
- **Verification:** 14/14 automated Pytest test suite with passing Next.js production builds.

### 8. 💎 [Prism OS](https://github.com/Speedyzyzz/prism) — AI-Powered Commerce Operating System
> **LangGraph • FastAPI • Next.js 15 • Generative UI • Python 3.11 • Multi-Modal AI**
- Replaces static eCommerce funnels with an intent-driven conversational commerce agent that understands user context and visual inspiration.
- Features multi-agent state nodes (Planner, Vision, Retriever, Executor, Reflection) streaming generative UI components and inline checkouts.
- Includes a Merchant Command Center with real-time fraud risk auditing and review authenticity verification.

### 9. 🛡️ [Axiom](https://github.com/Speedyzyzz/Axiom) — AttackChain AI (Deterministic SOC Investigation)
> **Python • FastAPI • SQLAlchemy • React Flow • MITRE ATT&CK Mapping • Claude Opus**
- Reconstructs reproducible attack chains from disparate enterprise security telemetry (VPN logs, authentication events, firewall traces).
- Uses a deterministic correlation engine rather than relying on hallucination-prone LLM logic for ground truth.
- Provides interactive investigation graph visualizations and transparent 100-point incident risk confidence scoring.

### 10. 🎯 [Pilot Carrom](https://github.com/Speedyzyzz/pilot-carrom) — Mobile & Web 2D Physics Game
> **TypeScript • Custom 2D Rigid-Body Physics • Capacitor • Vite • Android & Web**
- Tournament-feel carrom game featuring custom 2D elastic collision resolution and continuous turn mechanics.
- Features minimalist tactile HUD, smooth striker dragging controls, procedural Web Audio sound synthesis, and automated Android APK builds.

---

## 💻 Tech Stack & Tooling

```
Frontend:       Next.js 15 (App Router), React 19, TypeScript, Tailwind CSS, Framer Motion, Three.js
Backend:        Python 3.11+, FastAPI, Node.js, Express, SQLAlchemy, Pydantic v2, RESTful APIs
Data & Storage: PostgreSQL (Window Functions, FTS, pgvector), Redis (Pub/Sub, Queues), SQLite, Prisma
AI & Agents:    LangGraph, Multi-Step Tool Calling, Structured JSON Extraction, RAG, OpenAI, Claude
Infra & DevOps: Docker, Docker Compose, Git Workflows, Linux/Bash, GitHub Actions CI/CD
```

---

## 📬 Get in Touch

- 🌐 **Personal Website:** [balavignesh.dev](https://balavignesh.dev)
- 💼 **LinkedIn:** [linkedin.com/in/balavignesh-v-t-72b157297](https://www.linkedin.com/in/balavignesh-v-t-72b157297/)
- 🐙 **GitHub:** [@Speedyzyzz](https://github.com/Speedyzyzz)
