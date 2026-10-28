# SG Haze Watch

A single-page Singapore haze (NEA PSI) and weather (Open-Meteo) dashboard, with a regional map and an ASEAN capitals comparison, split across two tabs.

## Deploy on Vercel

This is a static site — a single `index.html` with no build step.

1. Import this repo in [Vercel](https://vercel.com/new).
2. Framework preset: **Other** (or "Static").
3. No build command, no output directory override needed — Vercel serves `index.html` from the repo root.
4. Deploy.

`vercel.json` just sets clean URLs; it isn't required for Vercel to find the site.

## Data

- Haze (PSI, PM2.5, PM10): NEA's 24-hour PSI, via data.gov.sg. Singapore only.
- Weather (temperature, humidity, wind, conditions): Open-Meteo, for Singapore and six ASEAN capitals.

Figures are currently a manually-placed snapshot, not a live API call from the browser — see the reading timestamp in the header and the caption under the map.
