# Currency Converter BD

A live currency converter to and from Bangladeshi Taka (BDT) — with a remittance mode for money sent home, an offline fallback using the last saved rates, and a 7-day USD→BDT trend chart that builds up from your own daily visits.

**Live demo: https://nafiz-xd.github.io/currency-converter-bd/**

## Features

- Convert between 15 currencies (BDT, USD, EUR, GBP, INR, SAR, AED, MYR, SGD, KWD, QAR, CAD, AUD, JPY, CNY) using live mid-market rates and cross-rate math
- Big animated result display with a one-tap swap button (⇅)
- Remittance mode: enter an amount sent home in a foreign currency and see the BDT received, with a clear note that bank, bKash and agent rates differ from the mid-market rate
- 7-day mini trend chart of USD→BDT, drawn from daily rate snapshots saved in your browser — no data is ever fabricated
- Offline fallback: the last successful rates are cached, and if a fetch fails the app keeps working and tells you when those rates were saved
- "Last updated" timestamp taken straight from the rates API response

## Tech

Vanilla HTML, CSS and JavaScript in a single page — rates from the free keyless ExchangeRate-API open endpoint (open.er-api.com), cache and daily snapshots in localStorage, trend chart drawn on canvas. No build step, no dependencies.

---
Built by Nafiz Bin Azad
