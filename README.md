# SwiftX

**Encrypted local file transfer between your devices, by HALXNAO.**

Send files directly between devices on your local network: no accounts, no cloud, no telemetry.

## Download

**[Download the latest version for Windows](https://github.com/halxnao/swiftx-releases/releases/latest)**

Windows 10 or 11, 64-bit. You do not need to install Java.

## Features

- Send and receive files directly over your local network (TCP), encrypted
- Send several files at once
- Resumable transfers: rerun an interrupted transfer and it continues where it stopped
- Finds devices on your network automatically, or enter an IP address yourself
- Dark and light themes
- No accounts, no telemetry, no cloud services

## Installing

1. Download `SwiftX-Setup-x.y.z.exe` from the [latest release](https://github.com/halxnao/swiftx-releases/releases/latest).
2. Run it and follow the wizard. You choose the install folder and shortcuts.
3. On an all-users install the setup can add a Windows Firewall rule so SwiftX can receive files on private networks. If you skip it, Windows will ask the first time you receive a file.
4. Updating: run the newer installer over the old version. Your settings are kept.

### Windows SmartScreen warning

The installer is not code-signed yet, so Windows may show "Windows protected your PC". Click **More info**, then **Run anyway**. To confirm the file is genuine, compare its SHA-256 with the value in the release notes:

```powershell
Get-FileHash .\SwiftX-Setup-2.0.0.exe -Algorithm SHA256
```

## Privacy

- No accounts, no analytics, no telemetry. SwiftX never contacts any HALXNAO server.
- It connects only to the devices you choose on your network and listens for discovery broadcasts (UDP port 55555).
- Settings are stored only on your computer, in `%APPDATA%\SwiftX`. The uninstaller asks whether to remove them (default: keep).

## License

SwiftX is closed-source software, copyright (C) 2026 HALXNAO. The end-user license is shown in the installer and installed with the app. Open-source components (OpenJDK, JavaFX) are listed in `THIRD-PARTY-NOTICES.txt` in the installation folder.
