# 💸 Spendly: Expense Tracker & Splitter

A mobile-friendly web app to log daily expenses, understand spending with simple KPIs and charts, get AI-style saving tips, and split costs with friends.

**🔗 Live demo:** https://janhvhi.github.io/spendly/

## Features

- **Add, edit and delete expenses** with amount, category, date and note
- **Monthly dashboard:** total spent, month-by-month navigation
- **Budget ring:** set a monthly budget and track % used (green / amber / red)
- **KPIs:** daily average, month-end forecast, no-spend days
- **Category donut chart:** tap a slice to filter the expense list
- **6-month trend chart:** compare spending over time
- **Members & split:** add members, choose who paid and who shares each expense
- **Settle up:** per-person paid, share and net balance, plus the simplest payments to clear everything
- **AI money coach:** short spending summary and saving tips (with a rule-based fallback)
- **Saved data:** stays after a refresh (browser localStorage)
- **Mobile first:** responsive layout, bottom-sheet form, light and dark mode

## How it works

| Feature | Logic |
|---|---|
| Daily average | Total spent ÷ days elapsed in the month |
| Month forecast | Daily average × days in the month |
| No-spend days | Days so far with no expenses |
| Net balance | Amount paid − share of split expenses |
| Settlements | Match people who owe with people owed, largest first, to minimise payments |

## Tech stack

- HTML, CSS and vanilla JavaScript (single `index.html`, no frameworks)
- SVG for all charts (no chart library)
- localStorage for data
- Hosted on GitHub Pages

## Run it

Open `index.html` in any browser, or visit the live demo. On a phone, use **Add to Home Screen** to open it like an app.

## Limitations

- Data is stored per browser and device, with no login or cloud sync
- Splits are equal only
- Forecast is a simple linear estimate
- Live AI tips work only inside claude.ai; elsewhere the built-in tips are shown

## Future improvements

- Backend database and user accounts for shared groups
- Custom split amounts
- CSV export and recurring expenses

## Author

Janhvhi Taunk