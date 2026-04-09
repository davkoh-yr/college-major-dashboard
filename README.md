# College Major Dashboard

A simple student-facing dashboard for comparing college majors using:

- Census PSEO Earnings View
- Census PSEO Flows View
- BLS CPS telework tables

The dashboard estimates a major-level in-personness index by merging major-to-industry graduate flows with industry-level telework shares, then visualizes earnings versus in-personness.

## Files

- `index.html`: dashboard layout
- `styles.css`: presentation and responsive styling
- `app.js`: interactivity and SVG scatterplot rendering
- `dashboard-data.js`: generated data snapshot used by the dashboard
- `build-dashboard-data.mjs`: rebuild script for the snapshot
- `pseo_earnings_raw.json`: raw Census earnings extract
- `pseo_flows_raw.json`: raw Census flows extract

## Run locally

Open `index.html` in a browser.

## Rebuild data

Run:

```bash
node build-dashboard-data.mjs
```

This regenerates `dashboard-data.js` from the raw Census extracts.
