# DataCore Cookbook

> Production-grade Jupyter notebooks for **quantitative finance on the Vietnamese stock market** — equity research, factor investing, and alternative data on HOSE, HNX, and the VN30, powered by the [DataCore](https://datacore.vn) financial data API.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Release](https://img.shields.io/github/v/release/DataCore-VietNam/datacore-cookbook?include_prereleases&sort=semver)](https://github.com/DataCore-VietNam/datacore-cookbook/releases)
[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/DataCore-VietNam/datacore-cookbook/badge)](https://securityscorecards.dev/viewer/?uri=github.com/DataCore-VietNam/datacore-cookbook)
[![Python](https://img.shields.io/badge/python-3.10%2B-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-notebooks-orange.svg)](https://jupyter.org/)
[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
[![PRs welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

Real-world, runnable workflows for analysts, quants, and data scientists working with Vietnamese financial and alternative data. Every notebook runs end-to-end on a free-tier API key and cites its dataset IDs explicitly.

## Contents

- [Why this cookbook](#why-this-cookbook)
- [Quick start](#quick-start)
- [Notebooks](#notebooks)
  - [01. Getting started](#01-getting-started)
  - [02. Equity research](#02-equity-research)
  - [03. Factor investing](#03-factor-investing)
  - [04. Alternative data](#04-alternative-data)
  - [05. Macro / economic](#05-macro--economic)
  - [06. ESG](#06-esg)
  - [07. Agents & LLMs](#07-agents--llms)
- [Contributing](#contributing)
- [Citation](#citation)
- [License](#license)

## Why this cookbook

DataCore provides clean, documented APIs for Vietnamese equities (HOSE, HNX, UPCOM), fundamentals, macroeconomic series, and alternative data. This cookbook turns that data into reproducible analysis: VN30 fundamental screeners, sector rotation, Fama-French factors adapted for Vietnamese accounting standards (VAS), e-commerce nowcasting, and LLM/agent workflows via the DataCore MCP server.

## Quick start

```bash
pip install -r requirements.txt
jupyter lab
```

Set your API key:

```bash
export DATACORE_API_KEY=dc_...
```

Get a free key at [datacore.vn/keys](https://datacore.vn/keys).

## Notebooks

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
- `01-ecommerce-signals.ipynb` — Shopee transaction data to nowcast MSN/VNM/MWG

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

## Contributing

PRs welcome — see [CONTRIBUTING.md](CONTRIBUTING.md) and our [Code of Conduct](CODE_OF_CONDUCT.md). Each notebook should:

- Run end-to-end with a free-tier key
- Cite dataset IDs explicitly
- Include a short "Why this matters" intro

## Citation

If you use these notebooks or DataCore datasets in your research, please cite the repository. See [CITATION.cff](CITATION.cff) or use the **Cite this repository** button on GitHub.

## License

Released under the [MIT License](LICENSE). Copyright (c) 2026 DataCore Vietnam.
