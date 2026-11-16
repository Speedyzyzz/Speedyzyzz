# Balavignesh

### Systems & AI Infrastructure Engineer | Coimbatore, India

Upstream contributor to **LiveKit Agents**, **BasedHardware Omi** (PR #22220 merged by founder Nik Shevchenko), and **Mixxx DJ** (PR #17467). Creator of **Cadence**, an ultra low latency audio failover proxy benchmarked at 648k frames per second. Passed the Soup AI systems evaluation with a 25.72 percent held out perplexity reduction.

[LinkedIn](https://linkedin.com/in/balavignesh-vt) • [Email](mailto:speedyzyzz@gmail.com) • [Website](https://balavignesh.dev) • [![Status](https://img.shields.io/badge/Status-Open%20to%20Opportunities-success)]()

---

### About

Third year computer science undergraduate in India building deterministic AI agent infrastructure, low latency real time systems, and upstream open source audio engines. 

Outside college lectures, I spend my time hunting memory leaks in production WebRTC frameworks, hardening backend database runtimes for consumer wearables, and engineering reproducible post training evaluation pipelines.

---

### Highlights

| System / Repository | Description & Production Proof |
| :--- | :--- |
| **[Cadence](https://github.com/Speedyzyzz/cadence)** | Zero downtime audio failover proxy for voice AI. Splices primary TTS stalls in 5.84ms with 0 dropped frames. Benchmarked at 648,000 frames per second with 3.39µs splice overhead. Rust, WebRTC, Tokio, SIMD. |
| **[LiveKit Agents](https://github.com/livekit/agents)** | Core framework contributor. Profiled and eliminated a 1,812 MB memory leak and 52,000 dangling AudioFrames on LiveKit Cloud (PR #2710). Guarded dynamic language switches against fatal IndexError crashes (PR #7976). |
| **[BasedHardware Omi](https://github.com/BasedHardware/omi)** | Backend systems hardening for AI wearables. Authored PR #22220 merged directly by founder Nik Shevchenko. Hardened vector hydration and batched Firestore memory operations across 500-batch limits. |
| **[Mixxx DJ](https://github.com/mixxxdj/mixxx)** | Real time audio DSP contributor (PR #17467). Clamped dynamic ring buffer bounds in EchoEffect engine, eliminating fatal assertion crashes under low BPM and high sample rates. Verified by core maintainers. |
| **[Soup Evaluation Suite](https://github.com/Speedyzyzz/soup-takehome)** | Complete post training and mathematical verification engine for Qwen2.5-1.5B. Achieved a 25.72 percent held out perplexity reduction (3.1160 down to 2.3145) with bit exact frozen layer isolation and 90.19 percent 4 bit Top 1 agreement. |

---

### Writing & Deep Dives

• **[WeightGuard: Mathematical Verification for LoRA Adapters](https://github.com/Speedyzyzz/soup-takehome)**: How matrix Frobenius norms and SVD spectral energy detect silent adapter detachment before production deployment.  
• **[Cadence: Sub 6ms Audio Failover in Real Time Voice Fleets](https://github.com/Speedyzyzz/cadence)**: Deterministic audio splicing without phase cancellation or audible clicks.
