# MF Quant Analyzer — Data

Auto-published data for **MF Quant Analyzer**, a free, open, quantitative
ranking tool for the Indian direct-growth mutual fund universe.

- 📊 **Live workbook** (interactive, one-click refresh): see the
  [latest release](../../releases/tag/latest)
- 📄 **Snapshot workbook** (no macros, same data, view-only): also in the
  [latest release](../../releases/tag/latest)
- 🔗 **Raw data (JSON)**: [`exports/metrics_latest.json`](exports/metrics_latest.json)
  — `data_health.nav_as_of` shows how current the NAVs are, and
  `data_health.recoveries` lists anything the pipeline had to work around
  on that run (empty means everything came from primary sources).

This repo is auto-updated daily by a private companion repo that fetches
NAV data from AMFI/MFAPI.in, computes ranking scores, and publishes here.
The scoring engine itself is not published — only its output.

## Data notes

- Updated every Tuesday and Thursday.
- Between 2026-08-18 and 2026-10-01, published rankings were computed on
  NAVs frozen at 2026-08-17, after an upstream AMFI file-format change.
  This was fixed and fully backfilled on 2026-10-02. The pipeline now
  adapts to such format changes automatically, and won't publish stale
  data.
- October 2026: the recommended ranking weights were updated based on a
  2016–2025 backtest. Download the latest workbook to get them; your own
  Weight Config edits are never changed by Refresh.

## Disclaimer

This tool is for informational and educational purposes only and does
**not** constitute investment advice. Mutual fund investments are subject
to market risks. Read all scheme-related documents carefully before
investing. Past performance is not indicative of future returns. This
project has no affiliation with any AMC, SEBI, or AMFI.

## License

Code in this repo (any scripts, if present) is MIT licensed — see
[`LICENSE`](LICENSE). This does not extend any license over the underlying
NAV data itself, which is sourced from AMFI/MFAPI.in.
