# MF Quant Analyzer — Data

Auto-published data for **MF Quant Analyzer**, a free, open, quantitative
ranking tool for the Indian direct-growth mutual fund universe.

- 📊 **Live workbook** (interactive, one-click refresh): see the
  [latest release](../../releases/tag/latest)
- 📄 **Snapshot workbook** (no macros, same data, view-only): also in the
  [latest release](../../releases/tag/latest)
- 🔗 **Raw data (JSON)**: [`exports/metrics_latest.json`](exports/metrics_latest.json)

This repo is auto-updated daily by a private companion repo that fetches
NAV data from AMFI/MFAPI.in, computes ranking scores, and publishes here.
The scoring engine itself is not published — only its output.

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
