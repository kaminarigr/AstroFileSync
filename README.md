# AstroFileSync

A lightweight Windows background service and tray application for safe astrophotography file synchronization.

Created by **YoruHikari** — [yoruhikari.gr](https://www.yoruhikari.gr/)

## Download

[Download the latest Windows installer](https://github.com/kaminarigr/AstroFileSync/releases/latest/download/AstroFileSyncSetup-x64.exe)

The installer is self-contained for Windows x64. The destination computer does not need the .NET SDK.

## Highlights

- Monitors an astrophotography source folder and copies completed files automatically
- Stable-file detection to avoid copying files while NINA or another capture application is still writing them
- Optional SHA-256 verification after each copy
- Windows Service for continuous background operation
- Tray dashboard with queue, progress, speed and live Matrix-style activity log
- Pause, resume and manual rescan controls
- Configurable source and destination folders
- Test copy, settings import/export and log viewer
- First-run configuration wizard
- Automatic recovery after destination drive reconnection

## Installation

1. Download `AstroFileSyncSetup-x64.exe` from the latest release.
2. Run the installer as Administrator.
3. Select the source folder used by your capture application.
4. Select the destination or backup folder.
5. Open AstroFileSync from the tray icon to view status or change settings.

Settings and logs are stored under:

```text
C:\ProgramData\AstroFileSync
```

## Verify the download

Each release includes a `.sha256` file. In PowerShell:

```powershell
Get-FileHash .\AstroFileSyncSetup-x64.exe -Algorithm SHA256
```

Compare the result with `AstroFileSyncSetup-x64.exe.sha256` from the same release.

## Current version

**4.2.1**

## Support

Website: [https://www.yoruhikari.gr/](https://www.yoruhikari.gr/)
