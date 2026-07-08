# Bedevere Desktop

**The native, local-first build of [Bedevere](https://bedeverewise.app) for Windows** — real DuckDB and the-stats-duck running on your own machine, no browser sandbox. Open SAS, SPSS, Stata, Parquet, and Excel files and query them with SQL: the same editor, table, and charts as [bedeverewise.app](https://bedeverewise.app), just running on native DuckDB.

This repository hosts the **release binaries and notes** for Bedevere Desktop. The application source is maintained privately.

## Download

Get the installer from the [**Releases**](../../releases/latest) page — currently **0.14.0-beta** (~19 MB):

→ `Bedevere-Desktop-0.14.0-win-x64-setup.exe`

## Install

1. Download and run the installer.
2. It is **not yet code-signed**, so Windows SmartScreen will warn you — click **More info → Run anyway**.
3. Bedevere Desktop uses the **WebView2 runtime**. Windows 11 already has it; on Windows 10 it arrives with any recent version of Microsoft Edge.

**System requirements:** Windows 10 or 11, 64-bit (x64). macOS and Linux are planned.

## Beta

This is a **public beta** — expect rough edges, and please report anything you run into [via Issues](../../issues) or at [kolistat.com/contact](https://kolistat.com/contact). Your files and queries stay on your device; the app does not phone home.

## Verify your download (optional)

Each release lists a SHA-256 checksum. To confirm your download is intact, run in PowerShell:

```powershell
Get-FileHash Bedevere-Desktop-0.14.0-win-x64-setup.exe -Algorithm SHA256
```

and compare the hash to the one in the release notes.

## Links

- **Web version:** [bedeverewise.app](https://bedeverewise.app) — the same app in your browser, no install.
- **Product page:** [kolistat.com/products/bedevere](https://kolistat.com/products/bedevere)

## License

Bedevere Desktop is proprietary software, free to use during the beta. See [LICENSE.txt](LICENSE.txt) for the End-User License Agreement and [THIRD-PARTY-NOTICES.txt](THIRD-PARTY-NOTICES.txt) for the open-source components it includes.

© 2026 Massimo Meneghello (KoliStat)
