# Champions League Predictor

A Jupyter notebook project to scrape match data (Champions League, Europa League, and the top 5 European leagues), build an Elo rating system, and eventually predict match results.

## Contents

- `champions_league_predictor.ipynb` — the main notebook: scraping, Elo ratings, predictions, and EDA
- `matches.csv` — cached scraped match data
- `elo.csv` — cached Elo ratings per match (before/after for both teams)
- `session_logs/` — short write-ups of what was worked on in each session

## Setup

```bash
python3 -m venv venv
source venv/bin/activate
pip install curl_cffi pandas matplotlib
```

Data comes from SofaScore's internal API via `curl_cffi` (needed to get past TLS-fingerprint bot protection — plain `requests` gets blocked).
