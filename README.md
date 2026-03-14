# 🏠 Indian Home Loan Calculator

A single-file, zero-dependency web app for planning and optimising your Indian home loan repayment. Works entirely in the browser — no server, no sign-up, no data sent anywhere.

## Features

| Feature | Description |
|---|---|
| **Outstanding balance mode** | Enter your current outstanding balance (not just original loan) for mid-loan planning |
| **Auto / override EMI** | Auto-calculates EMI from balance + rate + tenure, or let you override it |
| **Step-up EMI** | Increase your EMI by a fixed % every year to match salary growth |
| **Extra monthly payment** | Add a flat extra amount on top of EMI every month |
| **One-time lump sums** | Schedule multiple one-off prepayments in specific months (e.g. bonus payouts) |
| **Recurring yearly lump sum** | Set an annual prepayment with a configurable month, start year, and yearly growth rate |
| **Loan closure date** | See exactly which month the loan closes under your chosen strategy |
| **Interest saved** | Compares total interest paid vs the original schedule |
| **Yearly stacked bar chart** | Visualises principal, interest, and prepayments year by year (Chart.js) |
| **Repayment schedule table** | Month-by-month breakdown — show first 24 or all months |
| **PDF / print export** | Downloads a self-contained HTML file that auto-prints as a formatted schedule |

## Quick Start

No build step needed. Just open `index.html` in any modern browser:

```bash
open index.html        # macOS
start index.html       # Windows
xdg-open index.html    # Linux
```

Or serve it locally:

```bash
npx serve .
# or
python3 -m http.server
```

## Usage

1. **Loan details** — Enter your outstanding balance, annual interest rate, and original tenure.
2. **EMI & step-up** — Leave EMI blank to auto-calculate, or enter a custom EMI. Set a step-up % to increase EMI annually.
3. **Extra monthly payment** — Optional flat top-up applied every month.
4. **One-time lump sums** — Click *+ Add lump sum* to schedule prepayments in specific months.
5. **Yearly lump sum** — Set a recurring annual prepayment (e.g. annual bonus), the month to pay it, starting year, and optional yearly growth.
6. Results update **live** as you type.
7. Click **Download PDF schedule** to export a printable repayment table.

## Tech Stack

- Pure **HTML + CSS + JavaScript** — single file, no framework
- [**Chart.js 4.4.1**](https://www.chartjs.org/) (CDN) — for the yearly breakdown chart
- No build tools, no Node.js, no dependencies to install

## File Structure

```
indian-home-loan-calculator/
└── index.html   # The entire app
```

## License

MIT