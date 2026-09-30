# Patchline beta downloads

Patchline brings gacha game schedules, saved events, useful resources and pull estimates into one local app.

**Windows browser beta:** download the Windows x64 ZIP from [Releases](https://github.com/Keo-Reinz/patchline-downloads/releases), extract it, and open **Start Patchline.cmd**. It opens in your normal browser and needs no account.

Your favourites and saved events stay on your PC. Schedule imports refresh while you use the app. Internet is needed for fresh source data, remote artwork and linked resources; cached schedules remain available when imports fail.

## Requirements

- Windows 11 x64.
- Microsoft's Visual C++ x64 runtime, already present on many PCs. If missing, use the [official installer](https://aka.ms/vc14/vc_redist.x64.exe).

Node is included. This is an unsigned beta; use the official release assets and accompanying SHA256 checksum.

## Updating and backups

Make a backup from Patchline before updating. Quit the old app, extract the new ZIP, and open its launcher. Your data stays in `%LOCALAPPDATA%\Patchline Beta`.

To stop the app, click **Quit Patchline** below the sidebar's region and timezone, use **Settings & backups → Local app**, or open **Stop Patchline.cmd**. Closing the browser alone leaves the app running. Older downloads have **Local beta → App controls → Quit Patchline**.

This repository distributes release packages. Each package includes third-party licenses and source attribution for game schedules. Game names and artwork belong to their respective publishers.
