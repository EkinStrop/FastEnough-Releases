# Fast Enough? - Android File Explorer

A Windows desktop file explorer for managing files on Android devices. Built for speed and reliability with a custom TCP server that runs on your Android device, bypassing the limitations of standard ADB file transfer.

## Download

Download the latest release from the [Releases](https://github.com/EkinStrop/FastEnough-Releases/releases) page.

The release ZIP contains:
- **Fast Enough - Android File Explorer.exe** (the app)
- **dokan2.dll** (required, must be in the same folder as the exe)
- **Dokan_x64.msi** (optional driver for virtual drive features, see below)
- **readme.txt** (setup instructions)
- **projfs_enable.png** (screenshot of the Windows Feature that needs to be enabled)
## Features

- **Dual-channel accelerated transfers** using USB and WiFi simultaneously for up to 2x faster speeds
- **WiFi ADB support** with setup wizard, auto-connect, and Android 11+ wireless debugging pairing
- **Dual-panel file explorer** with Windows and Android side by side
- **High-speed file transfers** via custom TCP protocol, significantly faster than standard ADB
- **Resume-capable transfers** that pick up where they left off after disconnection
- **CRC32 integrity verification** computed inline during transfer with ARM hardware acceleration
- **Virtual drive mount** (Dokan) to browse device files directly in Windows Explorer
- **Dual-device support** for transferring files between two Android devices
- **Windows Explorer drag-and-drop** in both directions
- **Rubber-band selection**, column sorting, search/filter, breadcrumb navigation
- **Appearance settings** with adjustable UI scale and full color theming
- **MCRAW container support** with ProjFS virtual mount for RAW video files
- **Single executable** with the Android server binary embedded inside

## Dokan Virtual Drive (Optional)

To mount your Android device as a virtual Windows drive (browse files in Explorer, stream data on demand), install the included Dokan driver:

1. Run **Dokan_x64.msi** from the release ZIP
2. **Restart your PC** after installation
3. In the app, go to Connection > Mount as Virtual Drive

Without Dokan installed, all other features work normally. Only the virtual drive mount requires the Dokan driver.

## Requirements

- Windows 10/11 (x64)
- Android device with USB Debugging enabled
- ADB (Android SDK Platform Tools) is bundled with the app

## Made by JohnTheFarmer
