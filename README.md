# Patchlines downloads

Patchlines brings gacha game schedules, saved events, resources and pull estimates into one local app for Windows 11 x64.

## Microsoft Store — coming after certification

Microsoft Store will be the main official Windows download. The Store release is currently a draft and is not available yet. It must complete certification and be published before you can download it.

Once published, install Patchlines through Microsoft Store and open it from Start. Microsoft Store will manage app installation and updates.

## Portable ZIP — available now

Use the GitHub ZIP if you prefer to extract the app and start it yourself.

**[Download portable Beta 4.1 for Windows x64](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.4.1/Patchline-0.1.0-beta.4.1-windows-x64.zip)** · [SHA256 checksum](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.4.1/Patchline-0.1.0-beta.4.1-windows-x64.zip.sha256) · [Release notes](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.4.1)

1. Extract the entire ZIP into a normal folder on your PC.
2. Open **Start Patchline.cmd** and wait for startup to finish.
3. Patchline opens in your usual browser. Keep the extracted folder while using the app.

Node is included. The ZIP needs no account, Node installation or npm commands.

### Manual PowerShell startup

Open the extracted folder containing `launcher.mjs` and `runtime`. Type `powershell` in File Explorer's address bar and press Enter, then paste:

```powershell
& .\runtime\node.exe --use-system-ca .\launcher.mjs --no-browser
```

Wait for the ready message and open its printed address in your browser. Keep PowerShell open. **Ctrl+C** or **Quit Patchline** stops the app. The ZIP includes `Manual startup.txt` with the full instructions.

### Portable ZIP requirements and updates

The ZIP supports Windows 11 x64. Some PCs need Microsoft's [Visual C++ x64 Redistributable](https://aka.ms/vc14/vc_redist.x64.exe).

It contains signed OpenJS Node and unsigned Cloudflare workerd. Smart App Control may block the runtime with either startup method. Keep Windows protections enabled and report the blocked filename if startup fails.

Export a backup from **Settings & backups** before updating. Quit the app, extract the next ZIP into a new folder, and start the new copy. The portable profile remains in `%LOCALAPPDATA%\Patchline Beta` and is reused. ZIP app updates are installed manually.

To stop the normal launcher, use **Quit Patchline** or **Stop Patchline.cmd**. Closing the browser alone leaves it running. Before switching download routes, export a backup and restore it from the new app's settings.

## Data and source coverage

Favourites, saved events and cached schedules stay on your PC. Fresh imports, remote artwork and linked resources need internet. Failed imports keep the last successful cache. Source coverage varies; unknown dates and estimated rewards retain their labels.

Browser reminders need notification permission and an open tab. Local Discord reminders need a configured webhook, automatic checks enabled, and the app running on an awake, online PC. Webhook credentials are excluded from backups and diagnostics.

Each package includes third-party licenses and source attribution. Game names and artwork belong to their respective publishers.

## Privacy and support

Read the [privacy policy](PRIVACY.md). For help, [open a support issue](https://github.com/Keo-Reinz/patchline-downloads/issues) without including private backups or credentials.
