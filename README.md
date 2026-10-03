<p align="center"><img src="assets/linktofile-logo.png" alt="LinkToFile logo" width="112"></p>

# LinkToFile

**Save an authorised video link as a file on your Windows PC.** Pick a quality yourself, or let Smart Download choose for your device.

**English** · [Русский](README.ru.md)

### [Download for Windows — Setup](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/LinkToFile-0.1.3-Setup-x64.exe)

[Setup (.exe)](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/LinkToFile-0.1.3-Setup-x64.exe) · [Portable (.zip)](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/LinkToFile-0.1.3-windows-x64-portable.zip) · [All releases](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases)

**Available release: 0.1.3 Beta**, published 18 September 2026. Free beta with a Russian and English interface. This is an early release: source websites can change and some links may fail. These download links point to the published version, not a draft.

## What the published beta includes

- Link analysis with video format and quality selection.
- Smart Download profiles for a TV, computer, phone and archive.
- Video downloads with audio-track merging through bundled FFmpeg.
- Playlists, a download queue, pause, resume, cancel and retry.
- Download history, opening completed media and saved settings.
- Russian and English interface, local diagnostics and third-party notices.
- Signed update verification for the installed version; Portable updates manually.

All current features are free. Download only your own content or material you are authorised to save. Follow the source service's terms. A public link does not grant permission; LinkToFile does not bypass DRM or paywalls.

## Requirements and installation

Windows 10 or 11, **64-bit x64**, with Microsoft Edge WebView2 Runtime. Internet access is needed for link analysis and downloads. Leave enough free space for the media and temporary separate tracks. Python, Node.js, yt-dlp and FFmpeg do not need to be installed separately.

1. Download **Setup** for a regular installation, or **Portable** to use an extracted folder.
2. Compare the file's SHA-256 with this release's [SHA256SUMS.txt](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/SHA256SUMS.txt).
3. Setup checks for WebView2 and can download its bootstrapper. For Portable, extract the **whole ZIP**, keep its toolchain and license folders together, then run `LinkToFile.exe`. WebView2 must already be available.
4. Paste an authorised link, review the formats, select a destination and download.

Clean Windows installation and operation without a developer environment remain separate acceptance checks; this page does not claim they have been independently certified.

## File verification and Windows warnings

The published 0.1.3 **installer and application have no Windows Authenticode publisher signature**. SmartScreen can show **Unknown Publisher / Unknown app**. Tauri's update signature verifies an update package; it does not identify a trusted Windows publisher or guarantee the absence of Windows warnings. Keep Windows protection enabled.

In PowerShell, replace the path with your downloaded file:

```powershell
Get-FileHash -LiteralPath '.\LinkToFile-0.1.3-Setup-x64.exe' -Algorithm SHA256
```

Compare the result with `SHA256SUMS.txt` from the **same release**. A matching hash confirms that the bytes match the reference; it does not prove that a file is safe. Scan the file with your local antivirus before running it. No claim of verification by every antivirus is made.

Installed builds use the configured beta update channel and verify update signatures. Finish or pause active downloads before updating. For Portable, get a newer published ZIP and extract it into a new folder; retain the old folder until you have checked your settings and files.

## Preview 0.1.4 — not yet released

These are real screenshots of a local **0.1.4 preview**, captured with an empty demonstration profile. They show the interface in development; **the downloads above are still 0.1.3 Beta**. No release date is promised.

<p><img src="assets/screenshots/preview-0.1.4-home-en.jpg" alt="Unreleased LinkToFile 0.1.4 preview: empty English home screen" width="700"></p>
<p><img src="assets/screenshots/preview-0.1.4-settings-en.jpg" alt="Unreleased LinkToFile 0.1.4 preview: English settings and version" width="700"></p>
<p><img src="assets/screenshots/preview-0.1.4-settings-ru.jpg" alt="Unreleased LinkToFile 0.1.4 preview: Russian settings and version" width="700"></p>

## Support and documents

[Website](https://linktofile.ru) · [Beta website](https://linktofile-beta.nikitacreator.chatgpt.site/) · [Release notes](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/tag/v0.1.3-beta) · [Beta terms](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/BETA-TERMS.txt) · [Third-party notices](https://github.com/NikitaCreatorDeveloper/linktofile-releases/releases/download/v0.1.3-beta/THIRD-PARTY-NOTICES.md)

Feedback and private security reports: [nikitacreatordeveloper@gmail.com](mailto:nikitacreatordeveloper@gmail.com). Include your app version, Windows version and short reproduction steps. Review diagnostics first and remove personal URLs, paths, account information and secrets. Send security details privately. Development is paused while demand is assessed from downloads and feedback; future features and guaranteed support are not promised.

Usage, privacy and license documents in Russian and English are also bundled in the application's `licenses` folder and available in Settings. Queue, history and settings are stored locally; source sites and image servers receive network requests. See the bundled privacy document for clipboard and update behaviour.

This public repository hosts user documentation and release downloads. The original LinkToFile source remains private. The free beta license and separate third-party licenses apply; no open-source license for the original application is granted here.
