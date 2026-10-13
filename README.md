# Manifold releases

Installers and update files for **Manifold**, a local-first terminal for running many shell and
AI-agent sessions side by side. Website: <https://manifold.rahnlab.de>

This repository holds release files only. The application's source code is in a private repository.

## Install

Open the [latest release](https://github.com/LukasRahn/manifold-releases/releases/latest) and download the file for your system:

| System | File |
|---|---|
| Windows 10/11 (x64) | `Manifold-<version>-setup.exe` |
| macOS (Apple Silicon) | `Manifold-<version>-arm64.dmg` |
| Debian / Ubuntu (x64) | `manifold_<version>_amd64.deb` |
| Other Linux (x64) | `Manifold-<version>.AppImage` |

The `.yml` and `.blockmap` files belong to the in-app updater. You do not need them.

**Windows.** The installer is not code-signed yet, so SmartScreen shows "Windows protected your
PC". Choose **More info**, then **Run anyway**.

**macOS.** The app is not notarized yet. Open the DMG, drag Manifold into Applications, then
right-click the app and choose **Open** the first time.

**Linux.** Install the package with `sudo apt install ./manifold_<version>_amd64.deb`. Ubuntu
24.04 and later should prefer the `.deb` over the AppImage.

## Updates

Manifold updates itself. On Windows and with the AppImage, updates download and install from
inside the app. On macOS and with the `.deb`, the app tells you when a new version is out.

Every update is checked against a signing key that is built into the app before anything is
installed. A release that fails that check is refused.
