<h1 align="center">Hi, I'm Aileen 👋</h1>

<p align="center">
  Solana / DeFi research · prop-AMM &amp; MEV simulation · on-chain trading bots · AI agents
</p>

<p align="center">
  <a href="https://github.com/lilaclilac09?tab=repositories"><img src="https://img.shields.io/badge/repos-101-8957e5?style=flat-square" alt="repos"></a>
  <img src="https://img.shields.io/badge/focus-Solana%20%C2%B7%20MEV%20%C2%B7%20AI%20agents-14b8a6?style=flat-square" alt="focus">
</p>

---

## ⭐ Featured — KeyShield · *spec-driven*

> **[keyshield](https://github.com/lilaclilac09/keyshield)** — *"iCloud Keychain for your API keys."*  A zero-knowledge vault that stores your API keys as ciphertext, hands agents **scoped session tokens** instead of raw keys, and accelerates calls through a Rust proxy.

🔗 [Live site](https://keyshield-sync-worker.vercel.app) · 📄 [SPEC.md](https://github.com/lilaclilac09/keyshield/blob/main/SPEC.md) · 📝 [**Build process & spec-driven write-up →**](./keyshield-process.md)

- 🔐 **Zero-knowledge** — AES-256-GCM encryption in the browser (WebAuthn PRF / wallet signature → HKDF-SHA256); the server only ever stores ciphertext and *cannot* decrypt at rest
- 🎫 **Scoped delegation** — agents receive `ksv2_…` session tokens with per-agent scopes, spending caps, and expiry; revocation is immediate (next request → `401`)
- ⚡ **Fast** — Rust reverse proxy with a two-tier cache (memory + disk) + single-flight dedup → **50–80 ms** hot path for Solana RPCs
- 🧩 **Spec-first** — `SPEC.md` (v0.1) pinned the protocol and invariants *before* code; the TypeScript vault, Rust proxy, Python SDK, MCP server, and Solana on-chain program all trace back to it
- 🛣️ **In design — x402 payments** — pay-per-call stablecoin settlement (USDC on Solana) so an agent's `spend_cap_usd` becomes a hard, autonomous budget · [details →](./keyshield-process.md)

<sub>Stack: `TypeScript` · `Rust` · `Python` · MCP · Solana · x402</sub>

---

## 🛠️ My Projects

### 🌊 Solana Prop-AMM Research & Simulation

- **[pamm-a](https://github.com/lilaclilac09/pamm-a)** — research & implementation sandbox for prop AMMs, market making, and Solana simulation `Rust`
- **[solana-pamm-MEV-binary-monte-analysis-contagious-pools](https://github.com/lilaclilac09/solana-pamm-MEV-binary-monte-analysis-contagious-pools)** — Monte-Carlo / binary analysis of MEV contagion across pools · [site](https://solana-pamm-mev-binary-monte-analys.vercel.app) `Jupyter`
- **[solana-pamm-MEV-binary-monte-analysis-w-o-rawdata](https://github.com/lilaclilac09/solana-pamm-MEV-binary-monte-analysis-w-o-rawdata)** — the analysis pipeline, raw data stripped `Jupyter`
- **[Prop-AMM-Toxic-Flow-Guard-1230-w-o-jito-bundle-w-pretty-front](https://github.com/lilaclilac09/Prop-AMM-Toxic-Flow-Guard-1230-w-o-jito-bundle-w-pretty-front)** — toxic-flow guard for prop AMMs with a clean front-end `TypeScript`
- **[Prop-AMM-Toxic-Order-Monitor](https://github.com/lilaclilac09/Prop-AMM-Toxic-Order-Monitor)** — real-time toxic-order monitoring for prop AMMs `TypeScript`
- **[propamm-laserstream-bot](https://github.com/lilaclilac09/propamm-laserstream-bot)** — prop-AMM bot built on a Helius LaserStream feed `TypeScript`

### 🤖 Trading Bots & On-Chain Tools

- **[HumidiFi-Sentinel-Bot_with-bundle-detection-ugly-front](https://github.com/lilaclilac09/HumidiFi-Sentinel-Bot_with-bundle-detection-ugly-front)** — HumidiFi sentinel bot with bundle detection (Helius API)
- **[Hyperliquid-HYPE-Whale-Tracker](https://github.com/lilaclilac09/Hyperliquid-HYPE-Whale-Tracker)** — tracks HYPE whale activity on Hyperliquid `TypeScript`
- **[jupiter-swap-w-o-wallet-price-feed](https://github.com/lilaclilac09/jupiter-swap-w-o-wallet-price-feed)** — Jupiter swap price feed and pairs, no wallet required `TypeScript`
- **[BNB-Memecoin-Copy-Trade-Architect](https://github.com/lilaclilac09/BNB-Memecoin-Copy-Trade-Architect)** — copy-trading architecture for BNB memecoins `TypeScript`
- **[RPCsol_pnl](https://github.com/lilaclilac09/RPCsol_pnl)** — Solana RPC-based PnL tracker `JavaScript`
- **[MPPSOL-agents](https://github.com/lilaclilac09/MPPSOL-agents)** — agent framework for Solana market-making `JavaScript`

### 🔐 Security & Reverse Engineering

- **[re-agent](https://github.com/lilaclilac09/re-agent)** — RE agent: Binary Ninja bridge + Claude tool-calling loop for stateful binary analysis `Python`
- **[keyshield_font](https://github.com/lilaclilac09/keyshield_font)** — KeyShield front-end / vault UI `TypeScript`
- **[hideaway](https://github.com/lilaclilac09/hideaway)** — experiments in secret hiding / obfuscation `Rust`

### 🧠 AI Agents & Automation

- **[multiagentclaw](https://github.com/lilaclilac09/multiagentclaw)** — multi-agent orchestration experiments `Python`
- **[Vibe-Coding-Task-Manager](https://github.com/lilaclilac09/Vibe-Coding-Task-Manager)** — task manager for vibe-coding workflows
- **[tamagochi-agent-interface](https://github.com/lilaclilac09/tamagochi-agent-interface)** — playful tamagotchi-style agent UI


### 📚 Interactive Courses

- **[solana-speed-demons](https://github.com/lilaclilac09/solana-speed-demons)** — 7-module course on Solana validator internals: Firedancer, Samba MEV, Delorean, pmm-sim `HTML`
- **[autoresearch-course](https://github.com/lilaclilac09/autoresearch-course)** — 4-module course on autonomous LLM-driven research loops `HTML`

### 🎨 Web Apps & Fun

- **[aileen_machina_01](https://github.com/lilaclilac09/aileen_machina_01)** — personal site for tech blogs · [site](https://aileen-machina-01.vercel.app) `TypeScript`
- **[fortune_cookie](https://github.com/lilaclilac09/fortune_cookie)** — fortune-cookie web app · [site](https://fortune-cookie-sand.vercel.app) `TypeScript`
- **[meme.vote](https://github.com/lilaclilac09/meme.vote)** — vote on memes, tally the results
- **[dart-watch](https://github.com/lilaclilac09/dart-watch)** — dart / watch experiment `TypeScript`


<p align="center"><sub>📍 Mars · Building at the intersection of Solana, MEV, and AI agents</sub></p>
