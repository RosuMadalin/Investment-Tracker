# Investment Tracker

A stock watchlist and charting web app. Add stock symbols to a personal watchlist, see live prices, browse candlestick charts across multiple time ranges, and read the latest news for the stocks you're tracking.

🔗 **Live demo:** https://rosumadalin.github.io/Investment-Tracker/ — fully interactive, no login required: add a stock symbol and see it appear on the watchlist and charts right away.

## Features

- **Watchlist** — add/remove stock symbols, validated against a live market-data API before being saved
- **Live prices** — fetched and cached in Firestore, refreshed automatically when stale
- **Candlestick charts** — rendered with [Lightweight Charts](https://github.com/tradingview/lightweight-charts), with a range selector (1D, 5D, 1W, 1M, 6M, 1Y)
- **Market news** — latest headlines for the symbols currently on the watchlist

## Tech Stack

- Vanilla JavaScript, HTML, CSS (no build step, no framework)
- [jQuery](https://jquery.com/) (slim build)
- [Firebase](https://firebase.google.com/) — Firestore (data) and Storage
- [Lightweight Charts](https://github.com/tradingview/lightweight-charts) — candlestick charts
- [Yahoo Finance API via RapidAPI](https://rapidapi.com/) — stock prices, historical data, and news
- Hosted on GitHub Pages

## Running Locally

This is a static site with no build step — clone the repo and open `index.html` directly in a browser, or serve the folder with any static file server, for example:

```bash
npx serve .
```

## Related Project

Manual QA test plan, test cases, execution results, and bug reports written against this app: [Investment-Tracker-QA](https://github.com/RosuMadalin/Investment-Tracker-QA)
