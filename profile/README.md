``` markdown
# VOIDLY
```


**AI-powered censorship intelligence network**  
Free VPN • Zero-Knowledge Email • On-Chain Messaging • Browser Extensions

[![Status](https://img.shields.io/badge/status-active-success)](https://voidly.ai/status)
[![Uptime](https://img.shields.io/badge/uptime-99.8%25-brightgreen)](https://voidly.ai/metrics)
[![Nodes](https://img.shields.io/badge/nodes-13%2F13-blue)](https://voidly.ai/vpn)
[![Model](https://img.shields.io/badge/AI-XGBoost%20v2-orange)](https://github.com/voidly-ai/voidly/blob/main/docs/AI_DEEP_DIVE.md)

---

## 🎯 Mission

Build an AI that learns from real-world censorship faster than censors can adapt.

**The Exchange:**
- **You get:** Free privacy tools (VPN, encrypted email, blockchain messaging)
- **We get:** Anonymous telemetry to train the AI
- **World gets:** Tools that get smarter every single day

No profit motive. No data selling. **Research-first.**

---

## 🚀 What We Built

### 1. **AI-Powered VPN** → [voidly.ai/vpn](https://voidly.ai/vpn)
- 13 global WireGuard nodes across 5 continents
- XGBoost ML routing (~92% accuracy)
- Traffic obfuscation (HTTPS mimicry, Cloak, QUIC-like)
- Self-healing infrastructure
- **Free tier:** 5GB/month, no signup required

### 2. **VoidMail** → [voidly.ai/mail](https://voidly.ai/mail)
- Zero-knowledge encrypted email
- Server **cannot** decrypt your messages
- Anonymous aliases (e.g., `x7k2p9@voidly.ai`)
- IMAP/SMTP support
- Calendar & contacts (encrypted)
- Secure links to non-Voidly users

### 3. **ChainMail** → [voidly.ai/chainmail](https://voidly.ai/chainmail)
- Wallet-to-wallet messaging on Base blockchain
- Censorship-resistant (on-chain storage)
- No central servers
- Contract: `0xFC82C29aCAfB5E0b17460B599E1CBB1d4f672079`

### 4. **Browser Extensions**
- **Censorship Monitor:** Tests ~100 domains hourly → [Live](https://voidly.ai/extension)
- **Secure Inbox:** Quick VoidMail access → [Live](https://voidly.ai/extension)
- **ChainMail:** Web3 messaging → Pending approval

### 5. **Intelligence API** (Planned)
- Real-time censorship data
- Public REST API
- Community reports
- Country-level analytics

---

## 🧠 How the AI Works
```

USER (Iran) → Requests VPN Connection ↓ API → Intelligence Service: "Best route for Iran?" ↓ XGBoost Model Analyzes: • Censorship intensity (HIGH) • Recent block events (DPI/RST patterns) • Node performance (health, latency, load) • Historical success rates (per country/node) • Time-of-day patterns • Protocol selection (obfuscate? TLS wrapping?) ↓ AI Predicts: Amsterdam + WireGuard-over-TLS + Port 443 Confidence: 95% | Reasoning: "High censorship; HTTPS mimicry optimal" ↓ Config Generated → User Connects → ✓ SUCCESS ↓ Telemetry (anonymous) → Training Data Updated ↓ Next Model → Even Smarter``` 

**Current Stats:**
- Model: XGBoost v2
- Training data: 8,500+ samples
- Accuracy: 92% AUC-ROC (target: 95%+)
- Inference: ~47ms
- Features: 13 dimensions

---

## 🌍 Global Network

**13 Active Nodes • 5 Continents • <50ms Avg Latency • 99.8% Uptime**
```

🌍 EUROPE (3) 🌎 NORTH AMERICA (5) 🌏 ASIA (3) ├─ Frankfurt, Germany ├─ New York, USA ├─ Tokyo, Japan ├─ London, UK ├─ Chicago, USA ├─ Singapore └─ Amsterdam, Netherlands ├─ Silicon Valley, USA └─ Bangalore, India ├─ Toronto, Canada 🌏 OCEANIA (1) └─ Mexico City, Mexico 🌎 SOUTH AMERICA (1) └─ Sydney, Australia └─ São Paulo, Brazil``` 

**Smart Features:**
- Real-time health monitoring (CPU, latency, bandwidth)
- Automatic fallbacks (seamless switching)
- Obfuscation (WireGuard-over-TLS/443) for high-censorship regions
- Geographic optimization
- Threat-adaptive selection

---

## 🔒 Privacy Guarantees

### ✅ What We Collect (Anonymous, Aggregate)
- Connection success/failure metrics
- Node health (CPU, load, bandwidth)
- Censorship events by country
- Performance telemetry

### ❌ What We NEVER Collect
- Browsing history
- DNS queries tied to users
- Post-connection IP addresses
- Personally identifiable information

### 🔐 Zero-Knowledge Architecture
- **VoidMail:** Server stores only ciphertext
- **VPN Nodes:** RAM-only posture, ephemeral configs
- **ChainMail:** On-chain storage (currently base64, E2E planned)

**Example Telemetry (Aggregate Only):**
```

┌─ Connection Event ────────────────────┐ │ Country: [IR] │ │ Node: [AMS] │ │ Outcome: SUCCESS │ │ Latency: 45ms │ │ Protocol: wireguard_obfs │ │ Censorship: DPI_DETECTED │ └───────────────────────────────────────┘ → Used for training; never tied to a person``` 

### 🛡️ Transparency
- **Open Source:** [github.com/voidly-ai](https://github.com/voidly-ai)
- **ZK Proofs:** `0x948Cd0F9206D5625b97A9D4e365992E5a82c7FF3` (Base L2)
- **Gradient Registry:** `0xC6926fFfb60C6D5Bd1bDd2f8FbF57c169710Dc44` (Base L2)
- **Privacy Policy:** [voidly.ai/c/privacy](https://voidly.ai/c/privacy)

---

## 🚀 Get Started (2 Minutes)

### For Users

**VPN:**
1. Visit [voidly.ai/vpn](https://voidly.ai/vpn)
2. Generate keys (client-side, no signup)
3. Scan QR or download `.conf`
4. Connect ✓

**VoidMail:**
1. Sign in at [voidly.ai/vpn](https://voidly.ai/vpn)
2. Create mail account
3. Use webmail or IMAP/SMTP:
   - IMAP: `mail.voidly.ai:993` (SSL)
   - SMTP: `mail.voidly.ai:587` (STARTTLS)

**ChainMail:**
1. Connect wallet (Base network)
2. Go to [voidly.ai/chainmail](https://voidly.ai/chainmail)
3. Send message to any `0x...` address

---

## 💻 Tech Stack

### Frontend
- **Next.js 14** (App Router) + TypeScript + TailwindCSS
- **wagmi** + **ethers.js** (Web3)
- **TweetNaCl** (Client-side encryption)

### Backend
- **Cloudflare Workers** (Edge API)
- **Express** + **PostgreSQL** (VoidMail/ChainMail)
- **TimescaleDB** + **Redis** (Intelligence)
- **Python FastAPI** (ML serving)

### ML
- **XGBoost v2** (Production routing)
- **Federated Learning** (IPFS gradient sharing)
- **Ed25519 signatures** (Gradient attestations)

### Infrastructure
- **WireGuard** + **Cloak** (Obfuscation)
- **systemd** (Service orchestration)
- **Caddy** (Reverse proxy)
- **Ubuntu 22.04 LTS**

### Blockchain
- **Base L2** (Ethereum)
- **Solidity** (Smart contracts)
- **Hardhat** (Development)

---

## 📊 Live Metrics

**Real-Time Dashboards:**
- Network Status: [voidly.ai/status](https://voidly.ai/status)
- Metrics: [voidly.ai/metrics](https://voidly.ai/metrics)
- Intelligence Health: [intelligence.voidly.ai/health](https://intelligence.voidly.ai/health)
```

┌─ NETWORK STATUS ──────────────────────┐ │ Nodes Online: 13/13 ✓ │ │ Avg Latency: 47ms │ │ Success Rate: 95%+ │ │ Uptime: 99.8% │ │ Active Sessions: [LIVE] │ │ AI Model: XGBoost v2 │ │ Training Samples: 8,500+ │ │ Federated Nodes: 13/13 │ └───────────────────────────────────────┘``` 

---

## 🤝 Contributing

We welcome contributions in:
- Traffic obfuscation & DPI evasion
- ML research (features, training, drift detection)
- Node automation & monitoring
- Security audits & pen testing
- UX improvements

**Quick Start:**
```

bash git clone https://github.com/voidly-ai/voidly.git cd voidly
See REFERENCE.md for setup``` 

**Resources:**
- [REFERENCE.md](./REFERENCE.md) - Complete technical reference
- [TROUBLESHOOTING.md](./TROUBLESHOOTING.md) - Debug procedures
- [Architecture Docs](https://github.com/voidly-ai/voidly/blob/main/docs/ARCHITECTURE.md)
- [API Docs](https://github.com/voidly-ai/voidly/blob/main/docs/API.md)

---

## 🗺️ Roadmap

### ✅ Phase 1: Foundation (Complete)
- 13 global nodes across 5 continents
- XGBoost ML routing (92% accuracy)
- Traffic obfuscation (Cloak, WireGuard-over-TLS)
- VoidMail with zero-knowledge encryption
- ChainMail on Base blockchain
- Browser extensions (live on Chrome + Firefox)
- Multi-method auth (wallet, Google, Twitter, email)

### 🔄 Phase 2: Enhancement (In Progress)
- Intelligence API public launch
- Real-time censorship dashboard
- Improved handshake detection
- iOS & desktop apps (native VPN integration)
- ChainMail E2E encryption (upgrade from base64)
- GAN-based traffic shaping

### 🔮 Phase 3: Decentralization (Planned)
- Community-run nodes + on-chain registry
- P2P mesh networking
- DAO governance
- 50+ nodes globally
- Autonomous network operation

---

## 🔗 Links

- **Website:** [voidly.ai](https://voidly.ai)
- **VPN:** [voidly.ai/vpn](https://voidly.ai/vpn)
- **VoidMail:** [voidly.ai/mail](https://voidly.ai/mail)
- **ChainMail:** [voidly.ai/chainmail](https://voidly.ai/chainmail)
- **Status:** [voidly.ai/status](https://voidly.ai/status)
- **GitHub:** [github.com/voidly-ai](https://github.com/voidly-ai)
- **Twitter/X:** [@Voidly_ai](https://x.com/Voidly_ai)
- **Telegram:** [t.me/+4laJpSoUooY5MWEx](https://t.me/+4laJpSoUooY5MWEx)

**Smart Contracts (Base L2):**
- ChainMail: `0xFC82C29aCAfB5E0b17460B599E1CBB1d4f672079`
- ZK Privacy Proofs: `0x948Cd0F9206D5625b97A9D4e365992E5a82c7FF3`
- Gradient Registry: `0xC6926fFfb60C6D5Bd1bDd2f8FbF57c169710Dc44`

---

## 🛡️ Security

**Found a vulnerability?**
- Critical: `security@voidly.ai` (PGP available on request)
- Non-critical: [Open an issue](https://github.com/voidly-ai/voidly/issues)

Valid reports receive public credit.

---

## ⚖️ License

**MIT License** (Open Source, Permissive)

Use it. Fork it. Improve it. No warranty.

---

## ⚠️ Disclaimer

**EXPERIMENTAL SOFTWARE — USE AT YOUR OWN RISK**

- Active research project; expect occasional breakage
- Not audited by third-party security firms (yet)
- No guarantees or warranties of any kind

**For proven anonymity:** Use Tor Browser + Tails OS  
**For advancing censorship evasion research:** Use Voidly

---

## 💡 Philosophy

**Why Free?**  
Privacy is a human right. Paywalls create a two-tier internet.

**Why Open Source?**  
Trust requires transparency. Audit it. Break it. Improve it.

**Why AI?**  
Censors adapt. Static VPNs get blocked. ML trained on real attempts stays ahead.

**Why Telemetry?**  
You can't fight what you can't measure. Data is anonymous, aggregate, performance-only.

**Vision:**  
An AI that learns faster than censors can adapt. A network that's unstoppable.

---

## 🚀 Join the Mission

- **Use it:** Every connection trains the AI
- **Share it:** Help people in censored regions
- **Build it:** Contribute code, research, ideas
- **Break it:** Find bugs, report issues
- **Fork it:** Start your own network

---
```

[SYSTEM_STATUS] ├─ VPN NODES: 13/13 OPERATIONAL ✓ ├─ VOIDMAIL: ACTIVE 📧 ├─ CHAINMAIL: ON-CHAIN 🔗 ├─ AI MODEL: LEARNING 🧠 ├─ EXTENSIONS: LIVE 🔍 ├─ UPTIME: 99.8% 📡 └─ MISSION: ACTIVE 🚀
END_TRANSMISSION``` 

---

**Built with 🖤 by researchers who believe privacy and freedom of information are fundamental human rights.**
```
