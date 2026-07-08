# Changelog — Bedevere Desktop

All notable changes to Bedevere Desktop. Installers are on the [Releases](../../releases) page.

## 0.14.0-beta — 2026-07-08

First public beta. Windows 10/11, 64-bit.

- Native **DuckDB** and **the-stats-duck** running locally — no browser sandbox.
- The same editor, table, and charts as [bedeverewise.app](https://bedeverewise.app), on native DuckDB.
- Native **re-export** to SAS / SPSS / Stata formats (`.xpt`, `.sav`, `.por`, `.sas7bdat`) alongside Parquet and JSON.
- Single self-contained installer (~19 MB); WebView2 runtime required (bundled on Windows 11 / recent Edge).
- Installer is not yet code-signed (SmartScreen "Run anyway").
