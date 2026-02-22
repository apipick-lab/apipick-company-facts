# apipick-company-facts

A [Claude Code](https://claude.ai/claude-code) skill that retrieves public company information by stock ticker or SEC CIK number using the [apipick](https://www.apipick.com) Company Facts API.

## What it does

Given a stock ticker symbol (e.g. `AAPL`) or SEC CIK number, this skill returns:

- **Company name** — official legal name
- **Industry & sector** — business classification
- **Exchange** — trading exchange (NASDAQ, NYSE, etc.)
- **Market cap** — market capitalization in USD
- **Employees** — total headcount
- **Website** — official company URL
- **SEC filings** — link to EDGAR filings page

## Requirements

An apipick API key is required. Get 100 free credits at [apipick.com](https://www.apipick.com).

## Installation

Install via Claude Code:

```bash
claude skills install https://github.com/apipick-lab/apipick-company-facts
```

## Usage

Once installed, just ask Claude naturally:

- *"Look up company info for Apple"*
- *"What's the market cap of TSLA?"*
- *"How many employees does Microsoft have?"*
- *"Get SEC filings for NVIDIA"*

Claude will resolve company names to tickers automatically and call the apipick API.

## API Reference

| Field | Value |
|-------|-------|
| Endpoint | `GET https://www.apipick.com/api/company/facts` |
| Auth | `x-api-key` header |
| Cost | 1 credit per request |

See [`references/api_reference.md`](references/api_reference.md) for full documentation.

## Links

- [apipick.com](https://www.apipick.com) — API platform
- [Company Facts](https://www.apipick.com/company-facts) — product page
- [Get API Key](https://www.apipick.com/dashboard/api-keys)
