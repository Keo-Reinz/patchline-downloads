# Patchlines downloads

Patchlines brings gacha game schedules, saved events, resources and pull estimates into one local Windows app. **Beta 10** adds automatic online publisher news for Honkai Impact 3rd, BrownDust2, Duet Night Abyss and upcoming Silver Palace, alongside Discord. It expands HI3's regional website coverage and BrownDust2's official notices, and shows per-game online check status in Announcements. The game hubs, optional translation and desktop tools from previous betas remain available. No Patchlines account is required.

## Choose a download

**[Open the Beta 10 download page](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.10)** and expand **Assets**.

| Download | File to choose | How to use it |
| --- | --- | --- |
| Windows installer | `Patchlines-0.1.0-beta.10-windows-x64-setup.exe` | Install for your Windows account, then open Patchlines from Start |
| Portable ZIP | `Patchline-0.1.0-beta.10-windows-x64.zip` | Extract the entire folder, then open Patchlines.exe |
| Microsoft Store | Deferred | A Store link will be added after development, certification and publication finish |

The release also includes a matching `.sha256` file for each download. The GitHub installer and ZIP remain unsigned, so Windows or security software can warn about or block them. Release installation does not require importing a test certificate.

### Installer

1. Download and open the setup EXE.
2. Use the default installation folder or choose a dedicated folder with **Browse**. The exact entered folder is used.
3. Click **Install** (or **Update** for an existing installation), then open **Patchlines** from Start.
4. Select **Patchlines** in the launcher and press **Start**.

The default folder is `%LOCALAPPDATA%\Programs\Patchlines` for the current Windows account. Existing registered installations are selected for upgrades. To move one, uninstall both the project and launcher with **Keep saved data**, then install in the new folder. Saved data stays separately in `%LOCALAPPDATA%\Patchline Beta`.

### Portable ZIP

1. Extract the entire ZIP into a normal folder on your PC.
2. Open **Patchlines.exe**.
3. Select **Patchlines** and press **Start**. Keep the extracted folder while using the app.

Node is bundled. Neither route needs a command line, a separate Node installation or a GitHub login.

## The launcher and app window

Start opens the project in its own resizable Windows window. The launcher hides and remains in the system tray. Closing the app window or choosing **Quit Patchline** stops the project and brings the launcher back. Minimise leaves it running. Patchlines is the first available project; the launcher catalog can grow as more projects are released.

The window uses Microsoft's WebView2 Evergreen Runtime. If it cannot open, choose **Retry**, **Open in browser**, or the official Microsoft runtime download page. The browser edition is also available through **Start Patchline.cmd** or manual startup below. Closing a browser tab leaves the backend running; use **Quit Patchline** to stop it.

The dedicated window and browser edition share this PC's saved project data. Browser-only appearance, cookies and permissions stay in each browser profile, so those choices may need to be selected again in the new window.

## What's in Beta 10

- **Automatic online news:** the four new games' public publisher announcements are collected on startup and every six hours while the app runs, independently of Discord. Recent collection covers the last two weeks and preserves previously stored inbox history.
- **Official regional HI3 notices:** Global and SEA website evidence supplements official Steam announcements, with regional timing and uncertainty retained.
- **Broader BrownDust2 coverage:** maintenance, events, update notes and general notices receive bounded checks. Explicit gameplay periods enter the timeline; coupons and end-only claims stay in Announcements.
- **Online source status:** Announcements shows each game's last successful check, recent notice count and coverage note. A failed provider keeps cached news and retries.
- **Silver Palace development news:** direct website checks keep its upcoming hub informed. Release timing remains unannounced; recruitment posts do not imply a confirmed test period.

This update adds no permission requests or account requirements. Unknown dates and rewards retain their labels. Check the original notice's server, platform and access conditions.

### Desktop tools retained from Beta 8

- **Announcements & review:** search and filter collected notices, browse older results, preview images and open videos at their source, mark read or hide posts, review evidence and open matching events.
- **Windows reminders and tray:** optional native alerts and shortcuts to Today, the launcher, pause reminders and quit.
- **Gameplay overlay:** a compact game-specific window with events, banners, deadlines and checklists; drag, resize, opacity, click-through lock and show/hide shortcuts.
- **Today customisation:** arrange sections, pin games, select an ending-soon window, edit recurring tasks and choose weekly reset days.
- **Launcher news:** bundled notices, cached release checks and separate installed/latest release notes.
- **Desktop window and installer:** launch in a dedicated app window and choose a folder for a fresh installation.

The [Beta 10 release page](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.10) includes the full notes and verified downloads after publication.

## Updates

Quit the running project to return to the launcher. Open its gear menu, choose **Check for updates**, then **Update**. The download is verified and staged before program files are replaced. The launcher returns afterward.

Inside Patchlines, use **Settings & backups → General → App controls → Check for updates → Download update → Restart to update**. Checks run automatically at startup and every six hours. They do not force installation. Source commits alone do not update installed apps; the maintainer publishes a packaged release first.

Saved data stays in the separate local profile. Export a collection backup from Settings & backups if you want an additional copy. The latest previous-version program and profile recovery copies are retained. If power loss interrupts replacement, quit any running copy and use **Restore Patchline.cmd** in that update workspace beside the app folder. Do not share recovery files publicly.

Beta 5 and later can use the updater once a compatible package is published. **Beta 4.1 and earlier need one manual upgrade to Beta 10 after publication.** Install the new edition or extract its ZIP into a new folder. Older direct browser sessions may reopen the browser after their first update; quit and open **Patchlines.exe** to enter the new launcher flow.

The installer and ZIP share `%LOCALAPPDATA%\Patchline Beta`. Store editions use a separate profile; transfer a collection backup when changing editions. Microsoft Store development and submissions remain deferred until the owner considers the app nearly complete and stable.

## Reminders and overlay

Windows reminders are off by default. Enable them in **Settings → Reminders**, then choose Windows delivery on saved events. The project, launcher and PC must remain running; Windows notification settings can hide an offered alert. Use Windows reminders in the dedicated window. Browser reminders are available in the browser edition with permission and an open tab. Local Discord reminders need a configured webhook, automatic checks enabled, and an awake, online PC.

Enable the optional overlay in **Settings → Gameplay overlay**. Its default shortcut is **Ctrl + Shift + O**. Lock mode passes clicks through; Settings and the tray can unlock it again. It is an ordinary Windows window for windowed and borderless games, and can be hidden by exclusive fullscreen.

The optional Discord source reader uses a dedicated bot and approved channels. It runs while the local app runs. Original-server history requires the bot to have access there. Credentials are protected for the current Windows user and excluded from collection backups and diagnostics.

## Uninstall and reinstall

The installer edition offers the same data choices in every uninstall route:

- **App controls → Open uninstall options** or **launcher gear → Uninstall project…** can remove the project and keep the launcher. Its main action becomes **Install**, which restores a verified same/newer release.
- **Windows Installed apps → Patchlines → Uninstall** or **Uninstall Patchlines.exe** beside the launcher can remove both the project and launcher.
- **Keep saved data** is selected by default. **Delete saved data** requires confirmation and removes the managed profile, protected Discord credentials, embedded browser data, internal backups and verified update recovery copies.

Download a collection backup before deleting data if you want to keep your plans; credentials and browser site data are excluded. Browser data outside Patchlines, exported files and downloaded installers remain under your control. Portable ZIPs use manual folder removal. Microsoft Store manages its own package removal.

## Manual PowerShell startup

Open the extracted folder containing `launcher.mjs` and `runtime`. Type `powershell` in File Explorer's address bar and press Enter, then paste:

```powershell
$env:PATCHLINE_LAUNCH_METHOD = 'manual'
& .\runtime\node.exe --use-system-ca .\launcher.mjs --no-browser
```

Wait for the ready message and open its printed address in your browser. Keep PowerShell open. **Ctrl+C** or **Quit Patchline** stops the app. The ZIP includes `Manual startup.txt` with the full instructions.

## Requirements and local data

Windows 11 x64 is the supported target. The launcher uses .NET Framework 4.8. Some PCs need Microsoft's [Visual C++ x64 Redistributable](https://aka.ms/vc14/vc_redist.x64.exe). The desktop window needs the [WebView2 Evergreen Runtime](https://developer.microsoft.com/microsoft-edge/webview2/#download-section). Its SDK assemblies, loader and license are bundled with Patchlines.

The package contains signed OpenJS Node and unsigned Cloudflare workerd. Manual startup uses the same runtime and may encounter the same Windows block. Report the exact blocked filename if startup fails.

Favourites, saved events and cached schedules stay on your PC. Fresh imports, remote artwork and linked resources need internet. Failed imports keep the last successful cache. Source coverage varies; unknown dates and estimated rewards retain their labels.

Packages include third-party licenses and source attribution. Game names and artwork belong to their respective publishers. Read the [privacy policy](PRIVACY.md). For help, [open a support issue](https://github.com/Keo-Reinz/patchline-downloads/issues) without including private backups or credentials.
