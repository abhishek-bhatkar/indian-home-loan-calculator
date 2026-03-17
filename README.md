# 🏠 Indian Home Loan Calculator

**🔗 Live demo → [abhishek-bhatkar.github.io/indian-home-loan-calculator](https://abhishek-bhatkar.github.io/indian-home-loan-calculator/)**

A single-file, zero-dependency web app for planning and optimising your Indian home loan repayment. Runs entirely in the browser — no server, no sign-up, no data sent anywhere.

## Features

**Loan inputs**
- Outstanding balance, rate, tenure, custom EMI override
- Step-up EMI (% increase per year), extra flat monthly payment
- One-time lump sums in specific months, recurring yearly lump sum with growth

**Results**
- Live closure date, interest saved, monthly schedule, stacked bar chart
- PDF/print export of full repayment table

**Insights & Analysis**
- **Tax benefit tracker** — Sec 24(b) interest deduction + Sec 80C principal deduction, year-by-year table, by tax slab (5% / 20% / 30%)
- **Break-even vs investing** — compares interest saved from prepayments vs investing at a configurable return rate
- **Scenario comparison** — side-by-side table of current inputs vs any saved scenario

**UX**
- **Dark mode** — toggles with 🌙/☀️ button, persists across sessions
- **Collapsible sections** — click any section title to collapse / expand
- **Scenarios (bookmarks)** — save, load, and delete named snapshots of your inputs
- **Auto-save** — all inputs persist in `localStorage` and restore on revisit

## Quick Start

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or serve locally: `npx serve .` / `python3 -m http.server`

## Tech Stack

- Pure **HTML + CSS + JS** — single file, no framework, no build step
- [Chart.js 4.4.1](https://www.chartjs.org/) via CDN

## License

MIT