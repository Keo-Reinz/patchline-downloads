# Patchlines downloads

Patchlines brings gacha game schedules, saved events, resources and pull estimates into one local app for Windows 11 x64. Beta 6 adds a native project launcher with Patchline as its first project. The local app works without a Patchlines account.

## Choose a download

| Download | Who it is for | Updates |
| --- | --- | --- |
| Microsoft Store | The main official Windows route, once certification and publication finish | Microsoft Store |
| Unsigned installer | Install from an EXE and open the project launcher from Start | Launcher and App controls check GitHub Releases |
| Portable ZIP | Extract a folder and open the included project launcher | Launcher and App controls check GitHub Releases |

**The Microsoft Store download link will be added after publication is confirmed.** Store certification and publication are separate from these GitHub releases.

**[Download the Beta 6 installer](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.6/Patchlines-0.1.0-beta.6-windows-x64-setup.exe)** · [Installer SHA256](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.6/Patchlines-0.1.0-beta.6-windows-x64-setup.exe.sha256)

Run the installer and follow its prompts, then open **Patchlines** from Start. Select **Patchline** and press **Start**. Node is bundled; no command line, Node installation or GitHub login is needed.

**[Download the portable Beta 6 ZIP](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.6/Patchline-0.1.0-beta.6-windows-x64.zip)** · [ZIP SHA256](https://github.com/Keo-Reinz/patchline-downloads/releases/download/v0.1.0-beta.6/Patchline-0.1.0-beta.6-windows-x64.zip.sha256) · [Release notes](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.6)

1. Extract the entire ZIP into a normal folder on your PC.
2. Open **Patchlines.exe** to enter the project launcher.
3. Select **Patchline** and press **Start**. The launcher hides while the project opens in your usual browser. Keep the extracted folder while using the app.

Choosing **Quit Patchline** stops the project and brings the launcher back, with Start ready to reopen it. The launcher shows project artwork, information and release news, with a catalog that can grow as new projects are added. Patchline is the first available project.

**Start Patchline.cmd** remains available to start the app directly in your browser. Manual PowerShell instructions are below. Direct startup keeps its own restart instructions after quitting.

The installer and ZIP are unsigned beta downloads. Windows or security software can still warn about or block them. Do not import a test certificate to install these editions.

## Updates

When a compatible published release is available, the project launcher's main action offers an **Update**. It verifies and stages the download before replacing program files, then returns to the launcher. Saved data stays in the separate local profile.

Beta 5 and later also support updates inside the app and check at startup and every six hours while running. Open **Settings & backups → General → App controls**, choose **Check for updates**, see release information, choose **Download update**, then **Restart to update**. In Beta 5, App controls is under Local app in the settings drawer. Export a collection backup from Settings & backups before an update if you want an additional copy.

After the first update from an older edition to Beta 6, the older updater may reopen the browser. Choose **Quit Patchline**, then open your **Patchlines** shortcut or the new **Patchlines.exe** once to enter the project launcher. Subsequent updates started from the launcher return there when installation finishes.

The latest previous-version app and profile recovery copies are kept; older completed recovery copies are removed after a healthy update where cleanup succeeds. If power loss interrupts replacement, quit any running app and use that update workspace's **Restore Patchline.cmd** beside the application folder to restore the previous version. Do not share recovery files publicly.

The ZIP and installer edition share `%LOCALAPPDATA%\Patchline Beta` and reuse an existing portable profile. Store editions use a separate profile; export and restore a collection backup when changing between Store and GitHub editions. Browser appearance and permissions may need to be selected again.

**Beta 4.1 and earlier need one manual upgrade to Beta 6.** Quit the old app, install Beta 6 or extract its ZIP into a new folder, then open the new copy. Beta 5 and later can use the App controls update flow. A GitHub source commit alone does not produce an app update; the maintainer publishes a packaged release first.

## Manual PowerShell startup

Open the extracted folder containing `launcher.mjs` and `runtime`. Type `powershell` in File Explorer's address bar and press Enter, then paste:

```powershell
$env:PATCHLINE_LAUNCH_METHOD = 'manual'
& .\runtime\node.exe --use-system-ca .\launcher.mjs --no-browser
```

Wait for the ready message and open its printed address in your browser. Keep PowerShell open. **Ctrl+C** or **Quit Patchline** stops the app. The ZIP includes `Manual startup.txt` with the full instructions.

## Requirements and local data

Windows 11 x64 is the supported target. Some PCs need Microsoft's [Visual C++ x64 Redistributable](https://aka.ms/vc14/vc_redist.x64.exe). The package contains signed OpenJS Node and unsigned Cloudflare workerd. Manual startup uses the same runtime and may encounter the same Windows block. Report the exact blocked filename if startup fails.

Favourites, saved events and cached schedules stay on your PC. Fresh imports, remote artwork and linked resources need internet. Failed imports keep the last successful cache. Source coverage varies; unknown dates and estimated rewards retain their labels.

Browser reminders need notification permission and an open tab. Local Discord reminders need a configured webhook, automatic checks enabled, and the app running on an awake, online PC. The optional Discord source reader uses a dedicated bot and approved channels; it runs only while the local app runs. Discord credentials are protected for the current Windows user and excluded from collection backups and diagnostics.

Closing the browser alone leaves the app running. Use **Quit Patchline** or **Stop Patchline.cmd**. After quitting, the stopped screen reflects your launch method; native project sessions return to the launcher. Uninstalling/removing the program does not automatically erase separate portable data, browser data or exported backups; the privacy policy explains deletion.

Each package includes third-party licenses and source attribution. Game names and artwork belong to their respective publishers.

Read the [privacy policy](PRIVACY.md). For help, [open a support issue](https://github.com/Keo-Reinz/patchline-downloads/issues) without including private backups or credentials.
