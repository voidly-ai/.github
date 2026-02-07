# VOIDLY

**The Global Censorship Intelligence Network**

[![Status](https://img.shields.io/badge/status-active-success)](https://voidly.ai/status)
[![Data](https://img.shields.io/badge/measurements-11.7M-blue)](https://voidly.ai/data)
[![Incidents](https://img.shields.io/badge/incidents-4,481-orange)](https://voidly.ai/censorship-index/incidents)
[![Countries](https://img.shields.io/badge/countries-51-green)](https://voidly.ai/censorship-index)
[![Model](https://img.shields.io/badge/AI-99.8%25%20F1-purple)](https://voidly.ai/methodology)

---

## What is Voidly?

Voidly is a nonprofit censorship research network that aggregates, analyzes, and publishes global internet censorship data. We combine measurements from OONI, IODA, Censored Planet, and our own probes to create the most comprehensive censorship intelligence available.

**Our data powers:**
- Researchers studying internet freedom
- Journalists investigating digital rights
- AI systems that need real-time censorship context
- Privacy tools that adapt to censorship patterns

---

## The Data

| Metric | Value | Description |
|--------|-------|-------------|
| **Live Measurements** | 11.7M | Real-time OONI network measurements |
| **Historical Records** | 1.6M | 10-year censorship archive (120 countries) |
| **Labeled Incidents** | 4,481 | Confirmed censorship events |
| **Countries Tracked** | 51 | Active monitoring coverage |
| **Data Sources** | 4 | OONI, IODA, Censored Planet, Voidly |

### AI Classification

Our ML model identifies real censorship events from network noise:

- **F1 Score:** 99.8%
- **ROC AUC:** 1.000
- **Algorithm:** GradientBoosting (sklearn)
- **Training Data:** 37K labeled incidents

---

## Access the Data

### Public API

```bash
# Get censorship index (all countries)
curl https://api.voidly.ai/data/censorship-index.json

# Get country details
curl https://api.voidly.ai/data/country/IR

# Get methodology
curl https://api.voidly.ai/data/methodology
```

Full documentation: [voidly.ai/api-docs](https://voidly.ai/api-docs)

### HuggingFace Datasets

- **Live Index:** [emperor-mew/global-censorship-index](https://huggingface.co/datasets/emperor-mew/global-censorship-index)
- **Historical Archive:** [emperor-mew/ooni-censorship-historical](https://huggingface.co/datasets/emperor-mew/ooni-censorship-historical)

### AI Integrations

| Platform | Integration |
|----------|-------------|
| Claude / Cursor | [MCP Server](https://github.com/voidly-ai/mcp-server) - `npx @voidly/mcp-server` |
| ChatGPT | [OpenAI Action](https://github.com/voidly-ai/chatgpt-action) |
| Custom | [REST API](https://voidly.ai/api-docs) |

---

## Repositories

| Repo | Description |
|------|-------------|
| [voidly-public](https://github.com/voidly-ai/voidly-public) | Research documentation, schemas, and API examples |
| [mcp-server](https://github.com/voidly-ai/mcp-server) | Claude/Cursor MCP integration |
| [chatgpt-action](https://github.com/voidly-ai/chatgpt-action) | ChatGPT/OpenAI action spec |

---

## Privacy & VPN Tools

Beyond research, Voidly provides free privacy tools:

- **VPN:** Free WireGuard VPN with AI-powered routing → [voidly.ai/vpn](https://voidly.ai/vpn)
- **VoidMail:** Zero-knowledge encrypted email → [voidly.ai/mail](https://voidly.ai/mail)
- **Extensions:** Censorship monitoring for Chrome/Firefox → [voidly.ai/extension](https://voidly.ai/extension)

These tools feed anonymous telemetry back into our research network.

---

## Citing Voidly

If you use Voidly data in research, please cite:

```
Voidly Global Censorship Index. (2026). https://voidly.ai/censorship-index
```

Or use our incident reports:
```
Voidly Censorship Incident Database. (2026). https://voidly.ai/censorship-index/incidents
```

---

## Links

- **Website:** [voidly.ai](https://voidly.ai)
- **Censorship Index:** [voidly.ai/censorship-index](https://voidly.ai/censorship-index)
- **Open Data:** [voidly.ai/data](https://voidly.ai/data)
- **API Docs:** [voidly.ai/api-docs](https://voidly.ai/api-docs)
- **Methodology:** [voidly.ai/methodology](https://voidly.ai/methodology)
- **Twitter/X:** [@Voidly_ai](https://x.com/Voidly_ai)

---

## License

- **Data:** [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) - Free to use with attribution
- **Code:** MIT License where applicable

---

*Built by researchers who believe internet freedom is a fundamental human right.*
