# Portfolio Dashboard

Interactive single-page dashboard for managing and analysing a Norwegian Aksjesparekonto (ASK) portfolio. Built as a standalone HTML file with no backend or dependencies beyond Chart.js.

**[Live Demo →](https://jackbrenn.github.io/norwegian-fund-visualizer/)**

## Features

- **Fund allocation table** — adjust weights per fund with live recalculation of portfolio value and monthly purchase amounts
- **Regional diversity analysis** — compare your portfolio's geographic exposure against the MSCI ACWI IMI benchmark with overweight/underweight indicators
- **Cost tracking** — blended TER calculation, per-fund cost estimates, annual and monthly cost breakdowns
- **Cost impact simulator** — swap in hypothetical TERs to see annual savings and compounding impact over 10/20 years
- **Growth projections** — configurable return rate with 5/10/20-year projections and interactive chart
- **Export/Import** — shareable URL encoding of your full configuration, or copy a plain-text summary to clipboard

## Usage

Open the [live demo](https://jackbrenn.github.io/norwegian-fund-visualizer/) or run `index.html` locally in a browser. Everything runs client-side.

To share a specific allocation scenario, click **Copy shareable link** and send the URL. The recipient's dashboard will load with your exact configuration.

## Customisation

Fund data is defined in the `FUNDS` and `FUND_REGIONS` objects near the top of the `<script>` block. To add or change funds, update these arrays with the fund's name, TER, and regional exposure breakdown from its factsheet.

The ACWI IMI benchmark weights are in the `ACWI` object and should be updated periodically from the latest index factsheet.

## Stack

- Vanilla HTML/CSS/JS
- [Chart.js](https://www.chartjs.org/) for donut, bar, and line charts
- [DM Sans / DM Mono](https://fonts.google.com/specimen/DM+Sans) via Google Fonts

## License

MIT

---

Built with [Claude](https://claude.ai) ✌️
