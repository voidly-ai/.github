# VOIDLY

    ██╗   ██╗ ██████╗ ██╗██████╗ ██╗  ██╗   ██╗
    ██║   ██║██╔═══██╗██║██╔══██╗██║  ╚██╗ ██╔╝
    ██║   ██║██║   ██║██║██║  ██║██║   ╚████╔╝ 
    ╚██╗ ██╔╝██║   ██║██║██║  ██║██║    ╚██╔╝  
     ╚████╔╝ ╚██████╔╝██║██████╔╝███████╗██║   
      ╚═══╝   ╚═════╝ ╚═╝╚═════╝ ╚══════╝╚═╝   

AI-powered VPN that learns to defeat censorship

Experimental • Open Source • Privacy-First

Free access. No signup. No logs. A smarter way to fight network restrictions.

---

## 🎯 Mission

We're building an AI that learns from real-world censorship attempts to keep you connected.

The Exchange:
- You get: Free VPN, AI-optimized routing, privacy protection
- We get: Anonymous telemetry to train the AI
- The world gets: A tool that gets smarter at defeating censorship every single day

No profit motive. No data selling. Research-first.

---

## 🔗 Quick Links

- Website: https://voidly.ai
- Get VPN: https://voidly.ai/vpn
- Status: https://voidly.ai/status
- Metrics: https://voidly.ai/metrics
- AI Deep Dive: https://github.com/voidly-ai/voidly/blob/main/docs/AI_DEEP_DIVE.md
- API Docs: https://github.com/voidly-ai/voidly/blob/main/docs/API.md
- Architecture: https://github.com/voidly-ai/voidly/blob/main/docs/ARCHITECTURE.md
- GitHub Org: https://github.com/voidly-ai
- X (Twitter): https://x.com/Voidly_ai
- Telegram: https://t.me/+4laJpSoUooY5MWEx

---

## 🧠 How the AI Works

    USER (Iran) → Requests VPN Connection
                    ↓
    API → Intelligence Service: "Best route for Iran?"
                    ↓
    XGBoost Model Analyzes:
      • Censorship intensity (HIGH)
      • Recent block events (DPI/RST patterns)
      • Node performance (health, latency, load)
      • Historical success rates (per country/node)
      • Time-of-day patterns
      • Protocol selection (obfuscate? TLS wrapping?)
                    ↓
    AI Predicts: Amsterdam + WireGuard-over-TLS + Port 443
    Confidence: 95% | Reasoning: "High censorship detected; HTTPS mimicry optimal"
                    ↓
    Config Generated → User Connects → ✓ SUCCESS
                    ↓
    Telemetry (anonymous) → Training Data Updated
                    ↓
    Next Model → Even Smarter

Current stats:
- Model: XGBoost v2
- Training data: 8,429+ samples
- Accuracy: 92% AUC-ROC (target: 95%+)
- Inference time: ~47ms
- Features: 13 dimensions (location, threat level, node health, time patterns)

---

## 🌍 Global Network

13 Active Exit Nodes • 5 Continents • <50ms Average Latency

    🌍 EUROPE (3)              🌎 NORTH AMERICA (5)       🌏 ASIA (3)
    ├─ Frankfurt, Germany      ├─ New York, USA           ├─ Tokyo, Japan
    ├─ London, UK              ├─ Chicago, USA            ├─ Singapore
    └─ Amsterdam, Netherlands  ├─ Silicon Valley, USA     └─ Bangalore, India
                               ├─ Toronto, Canada
    🌏 OCEANIA (1)             └─ Mexico City, Mexico     🌎 SOUTH AMERICA (1)
    └─ Sydney, Australia                                   └─ São Paulo, Brazil

Smart routing:
- Real-time health monitoring (CPU, latency, bandwidth)
- Automatic fallbacks (seamless switching)
- Obfuscation (WireGuard-over-TLS/443) for high-censorship regions
- Geographic optimization (proximity when relevant)
- Threat-adaptive selection (protocols/ports based on risk)

Uptime: 99.8% • Status: https://voidly.ai/status

---

## 🔒 Privacy

We collect (anonymous, aggregate):
- Connection success/failure and performance metrics
- Node health (CPU, load, reachability, bandwidth)
- Censorship events by country (aggregated patterns)

We never collect:
- Browsing history
- Per-user DNS queries
- Post-connection IP addresses
- Personally identifiable information

Nodes operate privacy-first:
- RAM-only posture (no persistent traffic logs)
- Ephemeral session configs (discarded after disconnect)
- Zero-knowledge architecture (we cannot see your traffic)

Example telemetry record (aggregate only):

    ┌─ Connection Event ────────────────────┐
    │ Country:     [IR]                     │
    │ Node:        [AMS]                    │
    │ Outcome:     SUCCESS                  │
    │ Latency:     45ms                     │
    │ Protocol:    wireguard_obfs           │
    │ Censorship:  DPI_DETECTED             │
    └───────────────────────────────────────┘
      → Used for training; never tied to a person

---

## 🚀 Get Started (2 minutes)

For users:
1. Visit https://voidly.ai/vpn
2. Generate keys and a config (client-side)
3. Scan QR code with WireGuard
4. Connect ✓

Requirements:
- WireGuard app (iOS/Android/Desktop). That's it.

---

## 💻 Tech Stack

Frontend (voidly.ai)
- Next.js 14 (App Router), TypeScript, Tailwind
- RainbowKit + Wagmi (Web3 wallet connection)
- Vercel/Cloudflare Pages

API (api.voidly.ai)
- Cloudflare Workers (TypeScript)
- D1 (SQLite) for sessions, R2 for config backups
- SIWE (wallet authentication), ethers.js (NFT verification)

Intelligence (intelligence.voidly.ai)
- Node.js + Python FastAPI
- XGBoost v2 (production), TFJS/ONNX (planned)
- TimescaleDB (time-series telemetry), Redis (jobs/cache)

VPN Infrastructure
- WireGuard (protocol), Nginx (reverse proxy + SSL)
- 13 global exit nodes
- Python agents (telemetry + health checks)
- Systemd (service orchestration)

Web3 (optional premium tier)
- Base (Ethereum L2)
- Hardhat + Solidity
- OpenZeppelin (ERC-721)

Deep dive: https://github.com/voidly-ai/voidly/blob/main/docs/AI_DEEP_DIVE.md

---

## 🤝 Contributing

We welcome contributions in:
- Traffic obfuscation and DPI evasion
- ML research (features, retraining, drift detection)
- Agent/node automation, monitoring, ops
- Security reviews and pen testing
- UX improvements for non-technical users

Quick start:

    git clone https://github.com/voidly-ai/voidly.git
    cd voidly
    make install
    make test

Workflow:
- Fork → Branch → Commit → PR with description

Resources:
- Contributing Guide: https://github.com/voidly-ai/voidly/blob/main/CONTRIBUTING.md
- Quickstart: https://github.com/voidly-ai/voidly/blob/main/QUICKSTART.md
- Architecture: https://github.com/voidly-ai/voidly/blob/main/docs/ARCHITECTURE.md
- API Docs: https://github.com/voidly-ai/voidly/blob/main/docs/API.md

---

## 🗺️ Roadmap

Phase 2: Global Expansion (40% complete)
- 13 global nodes across 5 continents
- XGBoost ML model v2 (92% accuracy)
- 8,429+ training samples (grow to 20K+)
- AI-powered routing in production
- Traffic obfuscation research (GAN shaping) in progress

Phase 3: Decentralization (planned)
- Protocol obfuscation (HTTPS mimicry, TLS wrapping)
- GAN-based traffic shaping (production-ready)
- Community-run nodes, on-chain registry
- P2P mesh networking
- 50+ nodes globally

Phase 4: Autonomy (research)
- Continuous learning vs live censors
- Real-time DPI fingerprint adaptation
- Decentralized governance (DAO)
- Fully autonomous network

---

## 📊 Live Metrics

Dashboards:
- Network Status: https://voidly.ai/status
- Metrics: https://voidly.ai/metrics
- Intelligence Health: https://intelligence.voidly.ai/health

Current performance snapshot:

    ┌─ NETWORK STATUS ──────────────────────┐
    │ Nodes Online:       13/13 ✓           │
    │ Avg Latency:        47ms              │
    │ Success Rate:       95%+              │
    │ Uptime:             99.8%             │
    │ Active Sessions:    [LIVE]            │
    │ AI Model:           XGBoost v2        │
    │ Training Samples:   8,429+            │
    └───────────────────────────────────────┘

---

## 🛡️ Security

Found a vulnerability?
- Critical: security@voidly.ai (PGP available on request)
- Non-critical: open an issue at https://github.com/voidly-ai/voidly/issues

We don’t run paid bounties (research project), but valid reports receive public credit.

---

## ⚖️ License

MIT License (open source, permissive). Use it, fork it, improve it. No warranty.

---

## ⚠️ Disclaimer

    EXPERIMENTAL SOFTWARE — USE AT YOUR OWN RISK

    - Active research project; expect occasional breakage
    - Not audited by third-party security firms (yet)
    - No guarantees or warranties of any kind

For proven anonymity: Use Tor Browser + Tails OS  
For advancing censorship evasion research: Use Voidly

---

## 💡 Philosophy

Why Free?  
- Privacy is a human right. Paywalls create a two-tier internet.

Why Open Source?  
- Trust requires transparency. Audit it. Break it. Improve it.

Why AI?  
- Censors adapt. Static VPNs get blocked. ML trained on real attempts stays ahead.

Why Telemetry?  
- You can’t fight what you can’t measure. Data is anonymous, aggregate, performance-only.

Vision  
- An AI that learns faster than censors can adapt. A network that’s unstoppable.

---

## 🚀 Join the Mission

Use it: Every connection trains the AI  
Share it: Help people in censored regions  
Build it: Contribute code, research, ideas  
Break it: Find bugs, report issues  
Fork it: Start your own network  

    [SYSTEM_STATUS]
    ├─ NODES: 13/13 OPERATIONAL ✓
    ├─ AI: LEARNING 🧠
    ├─ UPTIME: 99.8% 📡
    └─ MISSION: ACTIVE 🚀

> END_TRANSMISSION
