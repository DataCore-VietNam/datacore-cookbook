# datacore-cookbook

Jupyter notebooks demonstrating real-world workflows on [DataCore](https://datacore.vn) — Vietnamese financial and alternative data.

## Sections

### 01. Getting started
- `01-quickstart.ipynb` — Connect, search, pull your first dataset
- `02-auth-and-rate-limits.ipynb` — API keys, tiers, retries
- `03-caching-and-performance.ipynb` — Local parquet cache patterns

### 02. Equity research
- `01-vn30-fundamentals.ipynb` — P/E, P/B, ROE screener
- `02-sector-rotation.ipynb` — Rotate across HOSE sectors
- `03-dividend-yield-screener.ipynb` — High-yield Vietnamese equities
- `04-earnings-surprise.ipynb` — Post-earnings drift on HOSE

### 03. Factor investing
- `01-fama-french-vn.ipynb` — Build VN equivalents of SMB / HML
- `02-momentum-12-1.ipynb` — Classic momentum on VN equities
- `03-low-vol.ipynb` — Low-volatility anomaly on HOSE
- `04-quality-score.ipynb` — Piotroski F-score, adapted for VAS

### 04. Alternative data
- `01-ecommerce-signals.ipynb` — Shopee / Tiki transaction data
- `02-satellite-port-traffic.ipynb` — Saigon Port throughput
- `03-social-sentiment.ipynb` — Vietnamese-language NLP on tickers
- `04-supply-chain.ipynb` — Manufacturing PMI nowcasting

### 05. Macro / economic
- `01-cpi-nowcasting.ipynb`
- `02-fx-vnd-regime.ipynb`
- `03-monetary-policy-events.ipynb`

### 06. ESG
- `01-emissions-disclosure.ipynb`
- `02-governance-scores.ipynb`

### 07. Agents & LLMs
- `01-mcp-claude-desktop.ipynb` — Connect DataCore MCP to Claude
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
