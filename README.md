<p align="center">
  <h1 align="center">AXL Sophon</h1>
</p>

<h3 align="center">Intelligence observer for multi-agent swarm networks</h3>

<p align="center">
  <em>Parse cognitive operations. Track beliefs. Compute consensus. Signal intelligence.</em>
</p>

<p align="center">
  <a href="https://github.com/AXLPROTOCOL/axl-sophon/actions/workflows/ci.yml"><img src="https://github.com/AXLPROTOCOL/axl-sophon/actions/workflows/ci.yml/badge.svg" alt="CI"></a>
  <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License"></a>
  <a href="https://pypi.org/project/axl-core/"><img src="https://img.shields.io/badge/AXL-v2.1-22c55e.svg" alt="AXL v2.1"></a>
  <a href="https://axlprotocol.org"><img src="https://img.shields.io/badge/protocol-axlprotocol.org-22c55e.svg" alt="Protocol"></a>
</p>

<p align="center">
  <a href="https://axlprotocol.org">Website</a> ·
  <a href="https://axlprotocol.org/rosetta">Rosetta</a> ·
  <a href="https://lang.axlprotocol.org">Documentation</a> ·
  <a href="https://github.com/AXLPROTOCOL/axl-core">axl-core</a>
</p>

---

Part of the [AXL Protocol](https://axlprotocol.org) ecosystem.

## What is Sophon?

Sophon is an omniscient observer that sits inside AXL-speaking agent networks. It parses cognitive operation packets (OBS, INF, CON, MRG, SEK, YLD, PRD), tracks per-agent belief states over time, computes network consensus, traces influence chains, and produces actionable intelligence signals.

Sophon (from Greek σοφία, "wisdom") — a real-time intelligence engine that extracts collective knowledge from multi-agent deliberation networks.

## Architecture

```
ANY AGENT NETWORK (MiroFish, CrewAI, AutoGen, LangGraph...)
│
▼ AXL packets (or English with LLM extraction)
┌─────────────────────────────────┐
│           SOPHON                │
│                                 │
│  Ingest → Parse → Track →      │
│  Analyze → Signal → Record     │
│                                 │
│  Endpoints:                     │
│    /signal    — real-time call  │
│    /beliefs   — agent states    │
│    /consensus — network view    │
│    /replay    — historical      │
│    /stream    — WebSocket feed  │
└─────────────────────────────────┘
│
▼ consumed by
2D Dashboard │ 3D Renderer │ Blender Pipeline │ CLI │ Trading Bot
```

## Seven Cognitive Operations

Sophon parses and tracks these AXL v2.1 operations:

| Operation | Verb | What it does |
|-----------|------|-------------|
| `OBS` | Observe | Raw data, no interpretation |
| `INF` | Infer | Draw conclusion from observations |
| `CON` | Contradict | Disagree with another agent's inference |
| `MRG` | Merge | Synthesize conflicting views |
| `SEK` | Seek | Ask for more information |
| `YLD` | Yield | Change mind based on new evidence |
| `PRD` | Predict | Forward-looking claim with confidence |

## Products

| Product | Description | Status |
|---------|------------|--------|
| [AXL Protocol](https://axlprotocol.org/rosetta) | Universal agent communication language | Live |
| [axl-core](https://github.com/AXLPROTOCOL/axl-core) | Python parser, emitter, validator, CLI | [PyPI](https://pypi.org/project/axl-core/) |
| **AXL Sophon** | Swarm intelligence observer | Development |
| MachIndex | Agent discovery and search | Planned |

## Requirements

- Python 3.11+
- Agent network speaking AXL v2.1+ (or English with degraded extraction)
- Minimum agent model size: 4B parameters for full cognitive grammar compliance

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License

Apache 2.0 — [AXLPROTOCOL INC](https://axlprotocol.org) · Diego Carranza · 2026
