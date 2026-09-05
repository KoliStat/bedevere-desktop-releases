# Changelog — Bedevere Desktop

All notable changes to Bedevere Desktop. Installers are on the [Releases](../../releases) page.

## 0.15.0-beta — 2026-09-05

- **Saved queries no longer vanish or revert.** Three data-loss paths closed, including the desktop store split that caused "saved a query, got a different one back, then it vanished". Queries that seemed lost in 0.14 may reappear after upgrading — they were saved all along.
- **Charts fixed across the board.** 64-bit integer columns (`count(*)`, IDs) no longer crash the renderer; bar / boxplot / violin over text columns draw instead of rendering empty; violin's `x:nominal` page-wide-ribbon bug is gone (the-stats-duck v0.8.0); axis labels are larger and facet headers legible in dark mode.
- **Stat-format re-export restored.** `.export` offers `.xpt` / `.sav` / `.por` / `.sas7bdat` again.
- Native **DuckDB updated to 1.5.1**, now statically linked (no loose DLL); bundled extensions load by path, so extension updates take effect on upgrade.

## 0.14.0-beta — 2026-07-08

First public beta. Windows 10/11, 64-bit.

- Native **DuckDB** and **the-stats-duck** running locally — no browser sandbox.
- The same editor, table, and charts as [bedeverewise.app](https://bedeverewise.app), on native DuckDB.
- Native **re-export** to SAS / SPSS / Stata formats (`.xpt`, `.sav`, `.por`, `.sas7bdat`) alongside Parquet and JSON.
- Single self-contained installer (~19 MB); WebView2 runtime required (bundled on Windows 11 / recent Edge).
- Installer is not yet code-signed (SmartScreen "Run anyway").
