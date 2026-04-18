# news-sentiment-analyst

> Aggregate financial news, classify market sentiment, and surface high-impact catalysts by ticker and sector — powered by [Finskills API](https://finskills.net) news endpoints.

[![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)]()
[![Plan](https://img.shields.io/badge/API%20Plan-Free%2FPro-yellow.svg)](https://finskills.net/register)
[![Category](https://img.shields.io/badge/category-news--sentiment-blue.svg)]()

---

## What This Skill Does

1. Fetches latest financial news from multiple sources via Finskills API
2. Classifies each story as bullish, bearish, or neutral
3. Assigns an overall **Risk-On / Mixed / Risk-Off** market sentiment label
4. Maps sentiment to specific tickers and sectors
5. Identifies catalyst types (earnings, FDA, M&A, analyst action, macro data)
6. Outputs a structured report with top themes, opportunities, and risks

## Install

```bash
npx skills add https://github.com/your-org/finskills-skills --skill news-sentiment-analyst
```

## Quick Start

```
You: What's happening in the market today?
Claude: [Fetches news, builds sentiment map, outputs structured report]

You: What's the latest news on AAPL?
Claude: [Fetches symbol-specific news, classifies sentiment, surfaces key stories]
```

## Example Triggers

- `"Give me a market sentiment check"`
- `"What are the biggest stories moving markets today?"`
- `"What's the news on Tesla this week?"`
- `"Which sectors are in the news positively today?"`
- `"Why is NVDA moving?"`

## API Endpoints Used

| Endpoint | Plan | Data |
|----------|------|------|
| `GET /v1/free/news/finance` | Free | General financial news |
| `GET /v1/news/latest` | Pro | Broader, more recent news |
| `GET /v1/news/by-symbol/{symbol}` | Pro | Stock-specific news |

## Requirements

- **Finskills API Key**: [Get one free](https://finskills.net/register)
- General market news works on **free plan**; stock-specific news requires **Pro**

## License

MIT — see [LICENSE](../LICENSE)
