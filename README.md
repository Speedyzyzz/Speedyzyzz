<div align="center">

# Balavignesh

### Systems & Audio DSP Engineer • Upstream Contributor • Voice AI Infrastructure

<p align="center">
  <a href="https://balavignesh.dev"><img src="https://img.shields.io/badge/Portfolio-balavignesh.dev-000000?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" /></a>
  <a href="https://www.linkedin.com/in/balavignesh-vt/"><img src="https://img.shields.io/badge/LinkedIn-Balavignesh-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://github.com/Speedyzyzz"><img src="https://img.shields.io/badge/GitHub-Speedyzyzz-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://github.com/Speedyzyzz/cadence"><img src="https://img.shields.io/badge/Cadence-v0.2.0-00F0FF?style=for-the-badge&logo=rust&logoColor=black" alt="Cadence" /></a>
</p>

```
Rust  •  Tokio  •  WebRTC  •  Audio DSP  •  Python  •  TypeScript  •  FastAPI  •  Docker
```

</div>

---

## ⚡ TL;DR

I am an **Infrastructure and Systems Engineer** based in Coimbatore, India building zero-downtime audio streaming runtimes and distributed AI pipelines. Upstream contributor to **LiveKit Agents** and **BasedHardware Omi**.

• ⚡ **Current Focus:** Creator of **[Cadence](https://github.com/Speedyzyzz/cadence)**, an ultra-low-latency audio failover proxy and DSP splicing plane in Rust (648k frames/sec, 5.84ms failover, 0 dropped frames).
• 🎙️ **Upstream Contributor:** Core framework contributor to [LiveKit Agents](https://github.com/livekit/agents) and [BasedHardware Omi](https://github.com/BasedHardware/omi).
• 🚀 **Production Proof:** [cadence](https://github.com/Speedyzyzz/cadence), [balavignesh.dev](https://balavignesh.dev).

---

## 🌐 Upstream Open Source Engineering

Active contributor hardening production voice AI frameworks and distributed wearable runtimes:

### 🎙️ [LiveKit Agents](https://github.com/livekit/agents) (Core Framework Contributor)
• **[PR #2710](https://github.com/livekit/agents-js/pull/2710):** `fix(agents): avoid retaining stream items on abort signal in readStream (#2658)` — Eliminates a massive 1,812 MB production memory leak and 52,000+ dangling AudioFrames in long-lived voice sessions. Independently profiled on LiveKit Cloud.
• **[PR #7976](https://github.com/livekit/agents/pull/7976):** `fix(deepgram): guard empty languages list in multilingual STT decoding` — Prevents fatal IndexError crashes during dynamic language switching in real-time multilingual voice agents. Verified and approved by core maintainer Chenwei Long.
• **[PR #7978](https://github.com/livekit/agents/pull/7978):** `fix(elevenlabs): propagate non-retryable STT errors instead of swallowing them` — Terminates zombie websocket sessions immediately on fatal auth and input errors instead of looping into reconnection storms.

### 🧠 [BasedHardware Omi](https://github.com/BasedHardware/omi) (Backend Systems Hardening)
• **[PR #23618](https://github.com/BasedHardware/omi/pull/23618):** `fix(database): chunk Firestore batch operations into safe sizes for memories and folders` — Prevents fatal 500 batch limit exceptions on massive folder mutations. Verified and officially approved by core maintainer Aryan Gupta.
• **[PR #22183](https://github.com/BasedHardware/omi/pull/22183):** `fix(backend): harden memory vector search & hydration pipeline against NoneType crashes and tombstoned vector leaks` — Fails closed against stale/deleted memory vectors, eliminates NoneType score comparison exceptions, and ensures hermetic hydration. Verified and approved by core collaborator David Zhang.
• **[PR #22220](https://github.com/BasedHardware/omi/pull/22220):** `fix(goals): guard qualitative goals against NoneType compare crashes and coerce suggestion floats` — Hardens AI goal advice pipelines and response schemas against unhandled NoneType comparisons and malformed LLM numerical outputs. Verified and approved by core collaborator David Zhang.
• **[PR #22836](https://github.com/BasedHardware/omi/pull/22836):** `fix(payment): guard stripe webhook against null metadata and missing item price lookups` — Eliminates unhandled 500 crashes during subscription webhook processing with 100% hermetic unit test verification.

---

## 🛠️ Flagship Systems & Frontier Runtimes

### 1. ⚡ [Cadence](https://github.com/Speedyzyzz/cadence) — Zero-Downtime Audio DSP Failover Proxy for Real-Time Voice AI
> **Rust • Tokio • Axum 0.7 • WebRTC Framing • Hann Crossfading • SIMD Lag Search • Tagged v0.2.0 • 100% Green CI**
• **Sub-6ms Failover:** Splicing primary TTS stalls (350ms injected) in **5.84 milliseconds** with **0 dropped audio frames** and zero audible click ($C^1$ continuity).
• **Massive Throughput:** Benchmarked at 10,000 concurrent audio streams processing **648,194 frames per second** with only **3.39 µs average splice overhead**.
• **LiveKit Drop-in:** Native Python plugin (`livekit-plugins-cadence`) providing one-line drop-in resilience for voice AI pipelines.
• **Empirical Proof:** WAV artifacts and benchmark suites committed under `tests/artifacts/` (`cadence_5ms_hann_spliced.wav`).

### 2. ⏱️ [Chronicle](https://github.com/Speedyzyzz/chronicle) — Deterministic Record-and-Replay Runtime for Coding Agents
> **FastAPI • Next.js 15 • Python 3.11+ • BLAKE3 • Lamport/Vector Clocks • 100% ChronicleBench Convergence**
• **Causal Event Ledger:** Intercepts every tool call, environment read, and subprocess mutation into an append-only event stream ordered by Lamport and vector clocks.
• **Content-Addressed State Trees:** Hashes filesystem mutations and deltas via streaming BLAKE3 hashing, enabling instant point-in-time state rollback.
• **Pure Replay & Divergence Localization:** Reproduces past agent executions with **zero external LLM API calls** by re-hydrating causal inputs from the ledger, pinpointing divergence within $\pm 0$ events.
• **Verification:** 13/13 Pytest suite passing offline and 40/40 benchmark tasks passing on `ChronicleBench` (100% convergence).

### 3. 🛡️ [Aegis Runtime](https://github.com/Speedyzyzz/aegis-runtime) — Policy-Enforcing Transaction Layer & Runtime Authorization Guardrail
> **FastAPI • Next.js 15 • Action IR • Two-Phase Commit • BLAKE3 Merkle Audit • 100% AegisBench Defense**
• **Typed Action IR & Quantitative Blast Radius:** Intercepts raw tool calls and normalizes them into canonical typed IR across SQL, Filesystem, HTTP, and Shell with quantitative risk scoring (0–100).
• **Two-Phase Commit & Scoped Attenuation:** Enforces a prepare/commit boundary with single-use, TTL-attenuated cryptographic capability tokens that eliminate TOCTOU race conditions.
• **Cryptographic Audit Chain:** Generates append-only BLAKE3 Merkle-linked audit receipts for every executed action, providing tamper-evident proof of compliance.
• **Adversarial Benchmark:** 100/100 adversarial cases defended on `AegisBench` (0% unauthorized side effects, 0 duplicate executions).

### 4. 🤖 [DevAgent](https://github.com/Speedyzyzz/devagent) — Policy-Constrained Autonomous Software-Engineering Runtime
> **Next.js 15 App Router • React 19 • FastAPI • Python 3.11+ • Sandboxed Tools • 100% Benchmark Resolution**
• **Autonomous Debugging Runtime:** Governs an LLM through deterministic filesystem exploration, lexical search (`ripgrep` with regex fallback), AST-validated atomic patchers, and subprocess test runners.
• **Empirical Benchmark Proof:** Tested against a 5-bug benchmark evaluation suite with a **100% verified resolution rate (5/5 bugs passed)** in under 6 turns average.
• **Defensive Sandbox:** Enforces strict realpath isolation, blocking path traversals (`../../`), external symlink escapes, and `.env`/`.git` access.

---

## 💻 Tech Stack & Tooling

```
Languages:      Rust, Python 3.11+, TypeScript, JavaScript, SQL, C, Bash
Systems:        Tokio, WebRTC Audio Framing, DSP (Hann Crossfading, SIMD), Axum
Backend:        FastAPI, Node.js, Express, SQLAlchemy, Pydantic v2, RESTful APIs
Frontend:       Next.js 15 (App Router), React 19, Tailwind CSS, Framer Motion
Data & Storage: PostgreSQL (Window Functions, FTS, pgvector), Redis (Pub/Sub), SQLite
Infra & DevOps: Docker, Docker Compose, Git Workflows, Linux Kernel Tuning, GitHub Actions CI/CD
```

---

## 📬 Get in Touch

• 🌐 **Personal Website:** [balavignesh.dev](https://balavignesh.dev)
• 💼 **LinkedIn:** [linkedin.com/in/balavignesh-vt](https://www.linkedin.com/in/balavignesh-vt/)
• 🐙 **GitHub:** [@Speedyzyzz](https://github.com/Speedyzyzz)
