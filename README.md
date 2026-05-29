# datacore-cookbook

Jupyter notebooks demonstrating real-world workflows on [DataCore](https://datacore.vn) — Vietnamese financial and alternative data.

## Sections

### 01. Getting started

Available now:
- `01-quickstart.ipynb` — Connect, search, pull your first dataset
- `02-auth-and-rate-limits.ipynb` — API keys, tiers, retries with exponential backoff
- `03-caching-and-performance.ipynb` — Local parquet cache patterns

### 02. Equity research

Available now:
- `01-vn30-fundamentals.ipynb` — P/E, P/B, ROE screener on VN30
- `02-sector-rotation.ipynb` — Top-3 sector rotation vs VN-Index

Planned:
- `03-dividend-yield-screener.ipynb` — High-yield Vietnamese equities
- `04-earnings-surprise.ipynb` — Post-earnings drift on HOSE

### 03. Factor investing

Available now:
- `01-fama-french-vn.ipynb` — Build VN equivalents of SMB / HML via 2x3 sorts

Planned:
- `02-momentum-12-1.ipynb` — Classic momentum on VN equities
- `03-low-vol.ipynb` — Low-volatility anomaly on HOSE
- `04-quality-score.ipynb` — Piotroski F-score, adapted for VAS

### 04. Alternative data

Available now:
- `01-ecommerce-signals.ipynb` — Shopee transaction data → nowcast MSN/VNM/MWG

Planned:
- `02-satellite-port-traffic.ipynb` — Saigon Port throughput
- `03-social-sentiment.ipynb` — Vietnamese-language NLP on tickers
- `04-supply-chain.ipynb` — Manufacturing PMI nowcasting

### 05. Macro / economic

Planned:
- `01-cpi-nowcasting.ipynb`
- `02-fx-vnd-regime.ipynb`
- `03-monetary-policy-events.ipynb`

### 06. ESG

Planned:
- `01-emissions-disclosure.ipynb`
- `02-governance-scores.ipynb`

### 07. Agents & LLMs

Available now:
- `01-mcp-claude-desktop.ipynb` — Connect DataCore MCP to Claude Desktop

Planned:
- `02-research-agent.ipynb` — Build an autonomous research agent
- `03-rag-on-filings.ipynb` — RAG over HOSE/HNX disclosures

## Setup

```bash
pip install -r requirements.txt
jupyter lab
```

Set your API key:
```bash
export DATACORE_API_KEY=dc_...
```

Get a free key at [datacore.vn/keys](https://datacore.vn/keys).

## Contributing

PRs welcome. Each notebook should:
- Run end-to-end with a free-tier key
- Cite dataset IDs explicitly
- Include a short "Why this matters" intro

## License

MIT
