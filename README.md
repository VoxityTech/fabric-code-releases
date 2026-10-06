```
███████╗ █████╗ ██████╗ ██████╗ ██╗ ██████╗    ██████╗ ██████╗ ██████╗ ███████╗
██╔════╝██╔══██╗██╔══██╗██╔══██╗██║██╔════╝   ██╔════╝██╔═══██╗██╔══██╗██╔════╝
█████╗  ███████║██████╔╝██████╔╝██║██║        ██║     ██║   ██║██║  ██║█████╗
██╔══╝  ██╔══██║██╔══██╗██╔══██╗██║██║        ██║     ██║   ██║██║  ██║██╔══╝
██║     ██║  ██║██████╔╝██║  ██║██║╚██████╗   ╚██████╗╚██████╔╝██████╔╝███████╗
╚═╝     ╚═╝  ╚═╝╚═════╝ ╚═╝  ╚═╝╚═╝ ╚═════╝    ╚═════╝ ╚═════╝ ╚═════╝ ╚══════╝
                                                                 BY VOXITY TECH
```

# Fabric Code releases

Installers and release builds of **Fabric Code**, the terminal agent and desktop app for [SimFabric](https://simfabric.dev).

## Install

```bash
curl -fsSL https://simfabric.dev/install | bash
```

This adds `~/.fabric/bin` to your PATH (zsh, bash, fish). Open a new terminal, go to a project and run `fabric`. Update later with `fabric upgrade`.

The desktop app for macOS, Windows and Linux is on the [Releases](https://github.com/VoxityTech/fabric-code-releases/releases) page and updates itself from there.

### Desktop app: first launch

Fabric Code is at **v0.0.1 (beta)** and its builds are not yet code-signed, so your system asks you to confirm the first launch:

- **macOS:** right-click the app and choose **Open**, then **Open** again. (If it is blocked: System Settings → Privacy & Security → **Open Anyway**.)
- **Windows:** in the SmartScreen window choose **More info → Run anyway**.
- **Linux:** the AppImage needs to be marked executable (`chmod +x`), or install the `.deb` / `.rpm`.

The terminal installer above is not affected.

## Getting started

1. Run `fabric` in a project folder. The first run walks you through a theme, sign-in, folder trust and terminal setup.
2. Sign in with your SimFabric account: approve in the browser with the confirmation code. For CI, set `FABRIC_API_KEY=sf_live_…` (create keys on simfabric.dev under Settings → API keys).
3. Fabric Code runs on SimFabric's own models: **Yarn-1**, **Loom-1** and **Fabric-1**. `/models` lists the ones your plan is served.

Documentation: [simfabric.dev/docs/code](https://simfabric.dev/docs/code) · Plans: [simfabric.dev/plans](https://simfabric.dev/plans) · Help: [simfabric.dev/code/feedback](https://simfabric.dev/code/feedback)

## What is in this repository

- `install`: the installer that `simfabric.dev/install` serves.
- [Releases](https://github.com/VoxityTech/fabric-code-releases/releases): the CLI and desktop builds that the installer, `fabric upgrade` and the desktop app's auto-update download.

The source code is developed privately.

---

**Fabric Code** · by [Voxity Tech](https://voxity.org)
