# StockSimulator

Flask + SQLite Bursa Malaysia paper-trading system with user accounts, buy/sell trading, portfolio valuation, delayed Yahoo Finance market data, Chart.js charts, Malaysia finance news, AI Chinese summaries, leaderboard, sortable tables, and a responsive UI.

Run: create and activate a virtual environment, install `requirements.txt`, then run `app.py`. Open http://127.0.0.1:5000. Add `NEWS_API_KEY` and `OPENAI_API_KEY` in `.env` when available.

## Delayed Bursa Malaysia Data

Quotes and charts are retrieved from Yahoo Finance through `yfinance` for the supported Bursa Malaysia symbols (for example, `1155.KL`). This is for personal coursework only: it is not an official Bursa feed, its timing and availability are not guaranteed, and it must not be used for live trading or redistributed commercially. The free feed does not reliably provide bid/ask values.

## Paper Trading UI

The app remains a paper-trading simulator and does not place real brokerage orders. The displayed order price is the latest available delayed quote.
