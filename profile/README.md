# VOIDLY

**The Global Censorship Intelligence Network**

[![Status](https://img.shields.io/badge/status-active-success)](https://voidly.ai/status)
[![Data](https://img.shields.io/badge/measurements-16M+-blue)](https://voidly.ai/data)
[![Incidents](https://img.shields.io/badge/incidents-5,700+-orange)](https://voidly.ai/censorship-index)
[![Countries](https://img.shields.io/badge/countries-126+-green)](https://voidly.ai/censorship-index)
[![Model](https://img.shields.io/badge/classifier-99.8%25%20F1-purple)](https://voidly.ai/methodology)

---

## What is Voidly?

Voidly is a **censorship research network** operated by Ai Analytics LLC that aggregates, classifies, and publishes global internet censorship data. We combine measurements from OONI, IODA, Censored Planet, and our own probe network into ML-classified, citable censorship intelligence.

**Who uses it:**
- Researchers studying internet freedom
- Journalists investigating digital rights
- Developers building circumvention tools
- Civil society organizations monitoring censorship

---

## The Data

| Metric | Value |
|--------|-------|
| **OONI Corpus** | 2.2B+ raw measurements (source we aggregate from) |
| **Voidly Live Samples** | 16M+ multi-source measurements |
| **Historical Records** | 1.6M (10-year archive) |
| **Documented Incidents** | 5,700+ (citable with evidence) |
| **Countries Tracked** | 126+ |
| **Evidence Items** | 25,000+ (OONI + IODA + CensoredPlanet) |
| **Data Sources** | 5 (OONI, IODA, CensoredPlanet, Citizen Lab, Voidly Probes) |

---

## Intelligence Products

| Product | Description |
|---------|-------------|
| [**Censorship Index**](https://voidly.ai/censorship-index) | Live country rankings with composite scores |
| [**Incident Database**](https://voidly.ai/live) | 5,700+ citable incidents with evidence permalinks |
| [**Claim Verification**](https://voidly.ai/verify) | Fact-check censorship claims against evidence |
| [**Domain Risk**](https://voidly.ai/domain/twitter.com) | Per-domain blocking status across all countries |
| [**7-Day Forecast**](https://voidly.ai/elections) | Shutdown risk predictions using ML + event calendar |
| [**Platform Risk**](https://voidly.ai/platforms) | Per-platform censorship scores (12 platforms) |
| [**ISP Risk Index**](https://voidly.ai/isps) | ISP-level censorship scoring and comparison |
| [**Accessibility API**](https://voidly.ai/accessibility) | Real-time "can users access X in Y?" oracle |
| [**Election Briefings**](https://voidly.ai/elections) | Election-censorship correlation analysis |
| [**Real-Time Alerts**](https://voidly.ai/api-docs#alerts) | Webhook notifications for censorship events |

---

## Access the Data

### For Developers

| Platform | Integration |
|----------|-------------|
| Claude / Cursor / Windsurf | `npx @voidly/mcp-server` — [27 tools](https://github.com/voidly-ai/mcp-server) |
| ChatGPT | [OpenAI Action](https://github.com/voidly-ai/chatgpt-action) |
| Any HTTP client | [REST API](https://voidly.ai/api-docs) + [llms.txt](https://voidly.ai/llms.txt) |

### For Researchers

| Format | Link |
|--------|------|
| REST API | [voidly.ai/api-docs](https://voidly.ai/api-docs) |
| HuggingFace (live) | [global-censorship-index](https://huggingface.co/datasets/emperor-mew/global-censorship-index) |
| HuggingFace (archive) | [ooni-censorship-historical](https://huggingface.co/datasets/emperor-mew/ooni-censorship-historical) |
| RSS/Atom | [Incident feeds](https://api.voidly.ai/data/incidents/feed.rss) |
| Bulk Export | CSV, JSONL via [API](https://voidly.ai/api-docs) |

---

## Repositories

| Repo | Description |
|------|-------------|
| [mcp-server](https://github.com/voidly-ai/mcp-server) | MCP server for Claude/Cursor (27 tools) |
| [voidly-probe-app](https://github.com/voidly-ai/voidly-probe-app) | Desktop probe app (macOS, Windows, Linux) |
| [community-probe](https://github.com/voidly-ai/community-probe) | Run a probe node from your network |
| [chatgpt-action](https://github.com/voidly-ai/chatgpt-action) | OpenAI/ChatGPT integration |
| [voidly-public](https://github.com/voidly-ai/voidly-public) | Research docs, architecture, and API examples |

---

## Citing Voidly

```bibtex
@misc{voidly2026,
  title  = {Voidly Global Censorship Index},
  author = {{Voidly Research}},
  year   = {2026},
  url    = {https://voidly.ai/censorship-index}
}
```

Individual incidents are citable: `https://voidly.ai/censorship-index/incidents/IR-2026-0142`

---

**All data is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).** Free to use with attribution.

[Website](https://voidly.ai) · [Open Data](https://voidly.ai/data) · [API Docs](https://voidly.ai/api-docs) · [Methodology](https://voidly.ai/methodology) · [𝕏](https://x.com/Voidly_ai)
