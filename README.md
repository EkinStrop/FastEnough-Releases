# Fast Enough? - Android File Explorer

A Windows desktop file explorer for managing files on Android devices. Built for speed and reliability with a custom TCP server that runs on your Android device, bypassing the limitations of standard ADB file transfer.

## Features

- **Dual-panel file explorer** with Windows on the left and Android on the right
- **High-speed file transfers** via custom TCP protocol, significantly faster than standard ADB pull/push
- **Two connection modes**: ADB Forward (default, reliable) and Direct TCP via USB tethering (faster)
- **Resume-capable transfers** that pick up where they left off after disconnection
- **CRC32 integrity verification** computed inline during transfer (no re-reads needed)
- **Batch file transfers** with automatic disconnect recovery and reconnection
- **Real-time device detection** via ADB track-devices (instant connect/disconnect notification)
- **Breadcrumb navigation** with back/forward history and clickable path segments
- **Column sorting** by name, size, or date with search/filter
- **Drag and drop** files between panels
- **Windows taskbar progress** bar during transfers
- **System tray support** with minimize-to-tray on close
- **Debug log window** (F12) for troubleshooting connection issues
- **Preferences** for ADB restart behavior and CRC verification toggle
- **Single executable** with the Android server binary embedded inside
- **OLED true-black theme** with light blue accents
- **Window state persistence** across sessions
- **Multi-device support** with device selector dropdown
- **Double-click to open** Android files (pulls to temp and opens locally)
- **Live window resize** rendering

## Download

Download the latest release from the [Releases](https://github.com/EkinStrop/FastEnough-Releases/releases) page.

## Requirements

- Windows 10/11 (x64)
- Android device with USB debugging enabled
- ADB (Android SDK Platform Tools) installed

## Made by JohnTheFarmer
