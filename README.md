# FOB Ocean Rates Dashboard 2026

Interactive dashboard for monitoring ocean freight rates across all active lanes for **Transnational Foods LLC** and **Pampa Beverages**.

---

## What it shows

- Monthly FOB ocean rates (USD) by route and container type
- Month-over-month % variation with color coding
- % variation vs January baseline (full-year trend view)
- Top movers — biggest rate increases and drops
- Average rate trend chart by month
- Regional summary cards (Asia, South America, Europe)

## Filters

| Filter | Description |
|---|---|
| Company | Transnational Foods / Pampa Beverages / Combined |
| Region | Filter by shipping region (Asia, South America, Europe) |
| Destination | Norfolk or LA / Long Beach |
| Country of Origin | Filter routes by origin country |
| Search | Free-text search by route name |

## Table views

| View | Description |
|---|---|
| Solo USD | Raw booked rates in USD |
| USD + Var% | Rates with month-over-month % change |
| Var% vs ENE | % variation compared to January baseline |

## Data source

Consolidated from regional booking files:
- Asia (China, Korea, Vietnam, India)
- South America (Brazil, Chile, Peru, Argentina)
- Europe (Spain, Germany, Netherlands)

Updated monthly. Source files managed in the internal logistics SharePoint.

## How to update

1. Run `standardize_and_consolidate.py` to refresh the source CSV
2. Run the main report script to regenerate `FOB_Ocean_Dashboard.html`
3. Upload the new file to this repo (replacing `index.html`)

The dashboard auto-deploys via GitHub Pages within ~30 seconds of upload.

---

*Maintained by the Logistics & Transportation team — Transnational Foods LLC*
