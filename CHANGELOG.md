# Changelog — Bedevere Desktop

All notable changes to Bedevere Desktop. Installers are on the [Releases](../../releases) page.

## 0.16.0-beta — 2026-11-03

- **Your workspace comes back after a restart.** Open dataset tabs reopen in the same order, with their column filters and sorts, and so do your settings, environments and query tabs. This works for folders, and for files opened with the `.import` command. Files added by drag-and-drop or with Help → Import → Browse Files do not come back yet. A fix is planned for 0.17.
- **New statistics.** the-stats-duck 0.9 adds `glm_fit`, `emmeans`, `lin_hyp`, `ptukey` and `qtukey`. Native **DuckDB is updated to 1.5.6**, the same version as bedeverewise.app.
- **Excel files open however you add them.** Dropped and uploaded `.xlsx` files now work, and import finds the table when a sheet has rows above it.
- **Chart colours at 3:1 contrast** on the Paper and Night themes, and prose set in Source Sans 3. The app's fonts are now bundled.
- **Folder import runs once.** A file whose table name is taken gets a numbered name, such as `AE_2`.
- **Help opens at startup only on your first visit.** Settings → Startup turns it back on.
- **About** shows the desktop's license, release notes and third-party notices, and the status bar shows the right version.

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
