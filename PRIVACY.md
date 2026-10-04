# Patchlines privacy policy

Last updated: 4 October 2026

This policy covers the local Windows Patchlines app, including its unsigned GitHub installer, portable GitHub ZIP and Microsoft Store distribution when available. The portable beta may display the name “Patchline” inside the app. The separately hosted website is outside this policy's scope.

Patchlines helps you plan game events, banners, reminders and checklists. You do not need a Patchlines product account or a game-account connection to use the local app. Microsoft Store, GitHub and other external services have their own account requirements and privacy policies.

## Data stored on your PC

Patchlines stores its local profile in a SQLite-based database and other files in your Windows user profile. This includes favourite games, timezone and region preferences, source-warning settings, saved events and progress, reminder rules, quiet hours, custom checklist items and completion history, announcement read history, and cached public source information. The app uses this data to display your plans, retain settings, refresh sources and decide which reminders are due.

Some interface preferences, such as appearance, layout, filters, translation choices and whether leak titles are revealed, are stored in your browser's local storage. The app also uses a `sidebar_state` cookie to remember whether the sidebar is open, with a seven-day lifetime. Browser permissions and notification settings are managed by your browser. Clearing browser site data can reset these choices separately from the app's local database.

Pull calculator values are temporary interface inputs rather than a persistent wallet. The local app also writes startup and error logs for troubleshooting, source-check status, reminder-delivery records and update-check caches.

The local server uses an internal profile identifier and control tokens to authorize local API operations, including quitting the app and configuring reminders. Its active-instance file holds a control token and process details and is removed after a clean shutdown. Protect access to your Windows profile and treat these files as private.

## Backups and diagnostics

Settings can export a JSON backup of your preferences, saved events, progress, reminders and checklists. The local runtime also keeps up to seven ordinary automatic backups and three backups made before an upgrade. Backups are local files; exported copies stay wherever you save them.

Discord webhook credentials are excluded from these collection backups. A requested diagnostic export contains source-check and runtime status, and excludes saved collections, local profile paths and webhook secrets. The diagnostic file downloads to your PC; using the feedback link does not automatically attach or submit it. Review any file or screenshot before sharing it.

## Connections to external sources

While you use Patchlines, the local runtime requests public game schedules, notices, guides, version information, community discussions, patch-income sheets and exchange rates from the configured sources. These include game publishers and community services linked inside the app. Refreshes can cover configured games beyond your favourites. Optional background schedule checks continue while the local app is running if you enable them.

Your browser may also request remote artwork and other resources from their hosts. Opening a source or resource link connects to that website. External services receive the requests and ordinary connection information, such as your IP address and requested resource. Browser requests may involve cookies, existing sign-in sessions or similar technologies according to your browser settings and the service's policy.

These requests use the configured public source URLs and, where needed, game identifiers. The app retains imported information in its local cache so a failed refresh can keep the last successful data available.

## Optional browser and Discord features

- **Browser notifications:** you choose whether to grant permission. Notifications can display a saved event's title and deadline on your screen. They need a running Patchlines tab and can be controlled through the app and your browser.
- **Discord reminders:** if you connect an incoming webhook, Patchlines contacts Discord to validate it and stores the connection settings locally. A test message is sent when you request one. When automatic reminders are enabled, the app sends the configured channel event titles, game/type information, deadlines, original-source links and a local app link. Discord and people with access to that channel can receive the messages. You can disconnect in Settings and revoke the webhook through Discord. [Discord privacy policy](https://discord.com/privacy)
  - The GitHub installer and portable ZIP starting at **Beta 5**, and the Microsoft Store build starting at package version **1.0.6.0**, protect the entire Discord settings file with Windows DPAPI encryption for the current Windows user. Existing unencrypted settings in that profile are replaced only after encryption succeeds. If Windows cannot protect or unlock the settings, the app reports an error and prevents new Discord deliveries. Protected files moved to another Windows user or PC may require reconnecting the channel.
  - The existing **portable Beta 4.1 ZIP** stores the webhook URL and channel information in an unencrypted local JSON settings file. That download has not been replaced by the Store build. The webhook URL is a credential; protect access to your Windows profile. Encryption also does not prevent other software running as your Windows user from accessing your settings.
- **Discord source reader:** if you connect a dedicated bot, Patchlines requests the bot's identity and messages from the approved channel registry. Collection retains public announcement text, embed/attachment links, original message identifiers, channel provenance and collection status in the local source cache. It can collect available history in the approved destination channels; original-server history requires the bot to have access there. A separate configured publisher archive can supplement older notices from public publisher sources. Supported dated activities can become schedule evidence; other posts stay in the announcement inbox. The bot token is protected with Windows secure storage for the current user and is excluded from collection backups and diagnostics. Automatic reading runs while the app is running on an awake, online PC. The reader does not send channel messages or join voice channels. Disconnect the reader in Settings and revoke the bot token through Discord if needed. [Discord privacy policy](https://discord.com/privacy)
- **X and Reddit content:** public-source imports can request X's public post information. The embedded X viewer and Reddit post previews connect your browser to those services when you choose to load them. Their content may use cookies or existing sessions under your browser settings. [X privacy policy](https://x.com/en/privacy) · [Reddit privacy policy](https://www.reddit.com/policies/privacy-policy)
- **Translation:** supported browser translation uses the browser's Translator API and may download language models after your action. Its availability and processing are managed by your browser. Choosing the external Google Translate link sends the selected title to Google in the link's query. [Google privacy policy](https://policies.google.com/privacy)

## App downloads, updates and support

Microsoft handles Microsoft Store acquisition and app updates under the [Microsoft Privacy Statement](https://www.microsoft.com/en-us/privacy/privacystatement). Patchlines' Store runtime directs you to Store updates. GitHub editions check the project's public releases for newer versions and cache release metadata locally. Starting at Beta 5, the app can download and stage a verified package when you choose **Download update**, then replace its program files when you choose **Restart to update**. Downloaded packages, staging state and an application rollback copy are stored locally. Update requests use GitHub's API and release download service without an embedded GitHub account token. Those services receive ordinary connection information, including your IP address and requested version or asset; the app does not send saved events or Discord credentials with update requests. Older ZIPs require a manual upgrade. [GitHub Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement)

Update recovery also keeps a verified local snapshot of the app profile, including its protected settings, to recover a failed migration. After a healthy update, the updater discards the downloaded ZIP and attempts to remove the prior completed recovery generation. The most recent recovery generation is retained; interrupted attempts or cleanup failures can leave additional copies. These recovery files stay on your PC and are not included in release downloads or diagnostic exports.

For support or privacy questions, contact the maintainer through [Patchlines GitHub issues](https://github.com/Keo-Reinz/patchline-downloads/issues). The issue tracker is public. Information you post, your GitHub account details and any attachments are handled by GitHub and can be visible to other people. The maintainer uses reports to respond to questions and investigate problems. Do not post private backups, webhook URLs, control tokens or other credentials.

## Your controls and deleting data

You can edit preferences, remove saved events and reminder rules, disable background reminders, disconnect Discord, and export a backup in the app. Revoking notification permission or clearing local site data is done through your browser.

Use **App controls → Quit Patchlines** to stop the local runtime. Closing the browser alone can leave the backend running. Note the data folder displayed in App controls before uninstalling. The portable beta normally uses `%LOCALAPPDATA%\Patchline Beta`; the Store version uses a separate Patchlines profile, whose physical location can depend on Windows package storage.

Deleting the portable app's extracted folder or uninstalling the GitHub desktop edition leaves its separate local profile behind. Do not assume that uninstalling a packaged app deletes every copy of your data: check for remaining profile files, browser site data and backups you exported elsewhere. To erase remaining local data, quit the app, remove its relevant data folder, clear its browser site data, and delete any exported backups, diagnostics or separately retained update downloads you no longer want. This also removes local saves and recovery copies, so export anything you wish to keep first.

Disconnecting Discord does not remove messages already delivered to a channel. Use Discord's controls for its messages and webhook. External services manage information already received under their own policies.

## Policy updates

This policy will be updated when the app's data handling changes. The date above identifies the latest version. Privacy questions can be raised through the support link above without including private data.
