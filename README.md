# Patchlines downloads

Patchlines brings gacha game schedules, saved events, resources and pull estimates into one local Windows app. **Beta 11.16** preserves matching event artwork, keeps dated announcements linked, expands verified featured details and adds animated launcher transitions. Saved progress and reminder IDs remain attached. Compatible updates retain changed-file downloads and lighter background processing. Today, sourced reset times, dated announcements, download progress, update size details and rotating launcher artwork remain available. The shared announcement feed supplies supported game information without configuring a Discord bot. All eighteen game hubs remain available. No Patchlines account is required.

## Choose a download

**[Open the Beta 11.16 download page](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.11.16)** and expand **Assets**.

| Download | File to choose | How to use it |
| --- | --- | --- |
| Windows installer | `Patchlines-0.1.0-beta.11.16-windows-x64-setup.exe` | Install for your Windows account, then open Patchlines from Start |
| Portable ZIP | `Patchline-0.1.0-beta.11.16-windows-x64.zip` | Extract the entire folder, then open Patchlines.exe |
| Microsoft Store | Deferred | A Store link will be added after development, certification and publication finish |

The release also includes a matching `.sha256` file for each download and a small `.size.json` metadata file used by update details, an update manifest and any available patch ZIPs with their checksums. Patch files are used automatically by compatible updaters. Choose the installer or ZIP to install the app. The GitHub installer and ZIP remain unsigned, so Windows or security software can warn about or block them. Release installation does not require importing a test certificate.

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

## What's in Beta 11.16

- **Richer schedule artwork:** matching reports can share their specific event or banner image independently of which source supplies dates. Sparse refreshes keep proven media for the same activity.
- **Reliable announcement links:** dated activities resolve through canonical identities; unresolved dated matches show their periods and a clear review label.
- **Verified featured details:** supported Endfield, GFL2 and NTE records retain exact named character or weapon details. Reverse: 1999, CZN Combatants and HI3 battlesuits gain exact named portraits; PGR retains typed featured names. Unsupported variants and lineups remain unfilled.
- **Animated launch and quit:** short transitions follow actual runtime readiness and shutdown, with reduced motion and failure recovery.
- **Smaller compatible downloads:** Beta 11.15 reuses unchanged verified runtime files through the published patch; the native launcher is updated for transitions.

### Schedule features retained from Beta 11.15

- **One corroborated activity:** matching calendar, guide and publisher reports share one card, retaining source evidence and uncertainty. Conflicting regions, versions and repeated cycles stay distinct.
- **Correct patch sections:** CZN notices keep named activity periods instead of repeating the patch title as a costume. NIKKE enemy lists remain supporting raid information.
- **Existing plans preserved:** cached identity repair retains saved progress and original reminder keys, including when a reporting source disappears.
- **Smaller compatible download:** Beta 11.14 can reuse unchanged verified launcher and runtime files through the published patch.

### Launcher features retained from Beta 11.14

- **Cleaner launcher:** the outer frame subtly reveals the desktop, while artwork and controls stay solid. Start sits directly on the artwork and sidebar icons share one centre line.
- **Visible gentle motion:** wallpapers slowly pan and zoom throughout their display, with short crossfades. Cached images and four slow-motion redraws per second keep the effect light; motion pauses while inactive or the project is open.
- **Compact release browsing:** single-line version entries fit more releases; full titles and dates remain in hover descriptions and release details. Each mouse-wheel notch moves one entry.

### Today and schedule features retained from Beta 11.13

- **Horizontal Today rows:** deadlines, today's banners and daily checkpoints each get a full-width section. Expand longer lists and keep the nearest deadlines and resets easy to reach.
- **Readable checkpoints:** controls wrap to fit each card; daily completion, undo, weekly work, server choices and uncertainty stay available.
- **Clearer schedule browsing:** affected games and sources are highlighted; still-running and early announcements are grouped by game with an All games view. Known opening and closing times have relative labels.
- **Gentle launcher motion:** the existing artwork can pan and zoom slowly and crossfade. Choose Static, Crossfade or Gentle motion; animation pauses while the launcher is inactive or the app is open.
- **Previous release notes:** older published Windows updates sit in a separate collapsed archive, with dates, source links and cached offline reading.

### Update features retained from Beta 11.12

- **Smaller compatible updates:** new and changed files are downloaded; unchanged files are verified and reused in a complete staged installation. Missing patches or modified baselines fall back to the full download. Installing this updater takes one full update; later compatible releases can use patches.
- **Clear download details:** patch sizes and actual received/total bytes are shown. Full fallback, complete installation sizes and staging/recovery space stay explicit.

- **Less repeated processing:** unchanged feed validation and schedule reconciliation are reused within bounded caches. Source corrections, health and uncertainty stay current.
- **Lighter desktop polling:** the launcher reuses one status helper; disabled overlays and paused reminders skip schedule work. Update and quit actions release the helper safely.
- **Incremental announcements:** quiet Discord checks update health, and changed games share one identity-maintenance pass.
- **Reliable navigation:** workspace menus, game hubs and Today shortcuts open through ordinary page navigation, avoiding the production router error. Unchanged schedule processing remains cached, automatic refreshes are coalesced and manual checks remain available.

### Announcement features retained from Beta 11.9

- **Dated announcements:** supported event, login, claim, costume, pass and shop notices become schedule activities while retaining their original source clocks and purchase conditions.
- **Repeated reports and corrections:** matching notices attach evidence to the same activity; ambiguous matches and different games, servers, versions or draw pools stay separate for review.
- **Saved-plan continuity:** provider and date changes keep saved activities and configured reminders linked. Bounded history and background reprocessing keep normal page reads efficient.
- **Reliable shared collection:** both new and older app versions receive their supported feed. Edits during collection no longer prevent publication, and save conflicts show the correct explanation.
- **Coverage stays explicit:** inaccessible text, unsupported wording and uncertain periods still need review. Unknown hours and rewards remain unknown.

### Today features retained from Beta 11.8

- **Today workspace:** immediate notices, saved deadlines and today's banners stay prominent. Customisation preserves section order, followed-game pins and the ending-soon window.
- **Daily checkpoint:** tasks are grouped by game, with one-tap daily completion, undo and local reset countdowns. Weekly work stays visible after dailies are done, and All clear means every task is finished for its current reset.
- **Sourced resets:** curated publisher/community references and Game Time Master checks supply server reset times. Choose a server or publisher when needed; personal overrides take priority. Fixed server clocks convert to your timezone, including daylight saving. Sources, conflicts and unsourced weekly days remain labelled. Reset research ships with the app.
- **Grouped catch-up:** unread changes appear by game and type with bounded previews and detail on demand. Repeated date notices collapse into one item, while genuine recurring cycles remain separate. Older unread history stays reachable, reading does not skip later pages, and historical details retain full source evidence.

### Update features retained from Beta 11.7

- **Download progress:** a progress bar, percentage and received/total bytes appear on the main update action when a verified total is available. Verification and installation keep their own status.
- **Update sizes:** open **Update details · sizes & space** below the main action, or **launcher gear → Update details…**. App controls also offers update details. These show download size, **Installed now → After update**, available drive space and an additional space estimate. Checks run when requested; older releases and incomplete scans keep unknown or partial labels.
- **Temporary space:** the estimate covers the download, extracted copy, update helper and safety margin. Saved-data backups need extra space on their own drive; the old app is kept for recovery.
- **Recovery preserved:** verified downloads, explicit update actions, saved profile data and previous-version recovery continue to use the existing process.

### Launcher features retained from Beta 11.6

- **Installation storage:** open **launcher gear → Installation storage…**, or use **Storage → Check storage** beside App updates in **App controls**. User-triggered checks show installation size and space available on the drive; the launcher also shows drive capacity. Partial scans say **At least** and explain skipped entries or limits. Checks read file metadata only, with the separate saved profile outside the measured app folder.
- **Rotating launcher artwork:** bundled images for all eighteen games, with matching game, publisher/artist credits and original source links. Archive and fan-art credits are retained. Rotation pauses while hidden, minimised or running the project; at most two images are decoded at once.
- **Manual update button:** a square refresh button beside the smaller Start button checks for packaged releases. An available update changes the main action to **Update**.
- **Clearer launcher UI:** vector action icons, rounded panels, clearer fonts, dark minimal scrollbars and native release-note headings, bullets and emphasis. Installed and latest release notes remain separate, with original text preserved.

### Schedule history and source improvements retained

- **Schedule loading:** current pages receive current records and archive counts. Historical records are excluded from the ordinary schedule payload and article overlay.
- **Archived history:** optional GachaTracker history for 11 game hubs loads the selected games and a month or bounded week window, with a date jump, recent-history shortcut and separate loading status. Public history checks run at most daily while browsing the archive. Only safely dated completed activities are retained; coverage and server applicability remain limited.
- **Saved history:** original dates, evidence and progress remain available. Historical saves and direct event links load their requested cached records.
- **Dates unconfirmed:** collected official activity notices appear separately until matching evidence supplies dates. Character-only links remain possible matches.
- **Resources:** additional Game8 news/version links and Enikk NIKKE character, team-usage and raid references.

- **Schedule imports:** Endfield's official version briefing supplies individual banners and event periods. Approved official linked posts and cached announcements receive current parsing. Unknown dates remain unknown.
- **Activity artwork:** BrownDust2 and Duet Night Abyss use images from each notice section rather than borrowing a sibling activity's image. Missing source artwork keeps its fallback.
- **Game backgrounds:** fifteen new 1440p or 4K images cover HI3, BrownDust2, Duet Night Abyss, Silver Palace, Limbus Company and Chaos Zero Nightmare, with source credits.
- **Settings and updates:** categories stay at the same height. App controls shows successful and failed checks and when the next automatic update check is due.

- **Shared announcement feed:** central collection every six hours; the app checks for published information on startup and every thirty minutes. No friend bot setup is needed. Original sources, images and uncertainty remain attached; personal plans stay local.
- **Reward claim periods:** supported in-game gift and claim windows enter the schedule. Paid offers, codes and unclear timing stay in Announcements.

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

BrownDust2's publisher currently refuses GitHub runner requests with HTTP 403. Its recovered schedule and artwork remain available in the shared feed; failed checks preserve prior information and freshness. Source coverage and artwork vary by activity.

The [Beta 11.16 release page](https://github.com/Keo-Reinz/patchline-downloads/releases/tag/v0.1.0-beta.11.16) includes the full notes and verified downloads after publication.

## Updates

Quit the running project to return to the launcher. Choose the square **Check for updates** refresh button beside **Start**, then **Update** when offered. The gear menu retains the same check. The download is verified and staged before program files are replaced. The launcher returns afterward.

Inside Patchlines, use **Settings & backups → General → App controls → Check for updates → Download update → Restart to update**. Checks run automatically at startup and every six hours. They do not force installation. Source commits alone do not update installed apps; the maintainer publishes a packaged release first.

Installing Beta 11.12 takes one full update to add the new updater. Later releases can download a smaller changed-file patch when one supports your installed version. Installed files are verified before reuse; missing patches or modified files use the full download. Progress and size details show the actual chosen download. Complete staging and recovery copies still require free disk space.

Saved data stays in the separate local profile. Export a collection backup from Settings & backups if you want an additional copy. The latest previous-version program and profile recovery copies are retained. If power loss interrupts replacement, quit any running copy and use **Restore Patchline.cmd** in that update workspace beside the app folder. Do not share recovery files publicly.

Beta 5 and later can use the updater once a compatible package is published. **Beta 4.1 and earlier need one manual upgrade to the current beta.** Install the new edition or extract its ZIP into a new folder. Older direct browser sessions may reopen the browser after their first update; quit and open **Patchlines.exe** to enter the new launcher flow.

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
