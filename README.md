# Patchline beta downloads

Patchline brings gacha game schedules, saved events, resources and pull estimates into one local app.

**[Download Beta 4.1 for Windows x64](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.4.1).** Extract the entire ZIP and open **Start Patchline.cmd**. It opens in your normal browser and needs no account. Node is included.

Your favourites, saved events and cached schedules stay on your PC. Fresh imports, remote artwork and linked resources need internet; failed imports retain the last successful schedules.

## Beta 4.1

- Rotating gallery is the default background for new browsers and profiles. Existing appearance choices stay saved; **Reset appearance** selects the new default. Reduced motion keeps the background still.

This release also includes the Beta 4 features:

- Fourteen games, including Genshin Impact and hololive Dreams, with additional official and community source coverage.
- Schedule binders for earlier running events, compact/comfortable cards, supported featured portraits and reward icons, clearer date headers and scrolling titles.
- Event Clock with larger artwork, urgency counters, aligned deadlines and live time remaining bars.
- Full scrollable announcement history, individual read receipts and a compact list view.
- Today checklists, clearer deadline durations, browser reminders and local Discord reminders using your own channel webhook.
- Reorderable favourites, rotating game backgrounds, adjustable glass effects and event artwork zoom/pan.
- Supported version updates, translation controls, source health, automatic local backups and private diagnostic exports.

Source coverage and translation availability vary. Unknown dates and estimated rewards retain their caveats. The release notes explain the supported behavior and limits.

## Manual PowerShell startup

Open the extracted folder containing `launcher.mjs` and `runtime`. In File Explorer's address bar, type `powershell` and press Enter. Paste:

```powershell
& .\runtime\node.exe --use-system-ca .\launcher.mjs --no-browser
```

Wait for the ready message and open its printed local address in your browser. Keep PowerShell open; **Ctrl+C** or **Quit Patchline** stops the app. The ZIP includes `Manual startup.txt` with the full instructions.

## Requirements

- Windows 11 x64.
- Microsoft's Visual C++ x64 runtime, already present on many PCs. If missing, use the [official installer](https://aka.ms/vc14/vc_redist.x64.exe).

Use the official release assets and accompanying SHA256 checksum. The beta contains signed OpenJS Node and unsigned Cloudflare workerd. Windows Smart App Control may block the runtime even with manual startup. The command option does not establish trust for workerd; keep Windows protections enabled and report the blocked filename if startup fails.

## Updating, backups and reminders

Export a backup from **Settings & backups**, quit the old app, extract Beta 4.1 into a new folder and start it. Your local profile stays in `%LOCALAPPDATA%\Patchline Beta` and is reused by the new version. Local automatic backups retain seven normal and three pre-upgrade copies.

To stop the app, click **Quit Patchline**, use **Settings & backups → Local app**, or open **Stop Patchline.cmd**. Closing the browser alone leaves the normal launcher running.

Browser reminders need notification permission and an open tab. Local Discord reminders need a connected incoming webhook, automatic checks enabled, the app running and the PC awake and online. Nothing refreshes or sends while the runtime is stopped. Webhook credentials are excluded from exported backups and diagnostics.

This repository distributes release packages. A ZIP update does not update the separately hosted website. Each package includes third-party licenses and source attribution. Game names and artwork belong to their respective publishers.
