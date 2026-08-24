<div align="center">

# ArkheOS

**Best performance. No strings attached.**

A free, open-source Windows 11 AME playbook built for maximum performance — trimmed, tuned, and yours to inspect line by line.

[![Version](https://img.shields.io/badge/version-1.1-white?style=for-the-badge&labelColor=050505)](https://github.com/Fola2x/ArkheOS/releases)
[![Windows](https://img.shields.io/badge/Windows-11%2025H2-white?style=for-the-badge&labelColor=050505)](#requirements)
[![License](https://img.shields.io/badge/license-MIT-white?style=for-the-badge&labelColor=050505)](#license)
[![Discord](https://img.shields.io/discord/0?style=for-the-badge&label=Discord&labelColor=050505&color=white)](https://discord.gg/xRB9BkNerz)

[Download](https://arkheos.xyz) · [Discord](https://discord.gg/xRB9BkNerz) · [Report an issue](https://github.com/Fola2x/ArkheOS/issues)

</div>

---

## About

ArkheOS is two things working together:

- **A prebuilt, already-debloated Windows 11 25H2 ISO** — download it straight from [arkheos.xyz](https://arkheos.xyz), flash it, install it. It's built by combining a clean Windows 11 image with the ArkheOS playbook via [AME Wizard](https://ameliorated.info/), so the debloating is baked in before you ever boot it.
- **The ArkheOS playbook itself** — the same `.yml` tweak library and `.bat` scripts in this repo, which you can apply on top of the ISO (or on top of any normal Windows 11 install) for performance, privacy, and gaming tweaks. Fully opt-in — a black box that decides for you this is not.

Nothing here is hidden in a compiled binary. Open `Configuration\` and `Executables\` and read exactly what runs before you ever install anything.

## What the installer actually does

Whether it's baked into the ISO build or run yourself via AME Wizard, the automated install is deliberately small:

1. Copies ArkheOS system files and drops a desktop shortcut
2. Downloads the **Arkhe Toolbox** (`Post.exe`) straight to your desktop
3. Removes Microsoft Apps / Xbox Apps — on by default, uncheck either to keep them
4. Installs your choice of browser — Brave, Chrome, Firefox, or Thorium

That's it. No wall of tweaks gets forced onto your machine during setup. Every performance, privacy, and debloat tweak below ships as its own standalone playbook in `Configuration\` — run the ones you want, skip the ones you don't.

## Tweak library

| Category | What it covers |
|---|---|
| `visual` | DWM animations, Explorer visuals, transparency |
| `performance` | Timer resolution, priority separation, HAGS, GPU scheduler |
| `privacy` | Telemetry, activity feed, CEIP, diagnostics |
| `gaming` | Game DVR/Bar, fullscreen optimizations, DirectX |
| `sound` | MMCSS audio scheduling, spatial audio |
| `mouse` | Raw 1:1 input, acceleration removed |
| `keyboard` | Input latency, sticky/toggle keys |
| `network` | NIC power saving, TCP/DNS tuning, NetBIOS |
| `file` | NTFS flags, Explorer file handling |
| `memory` | RAM-scaled paging and cache tuning |
| `onedrive` | Full removal + Cloud Files filter driver |
| `debloat` | Store apps, Edge, ads/suggestions, Windows Update nags |
| `services` | Background services, service-host grouping |
| `drivers` | AMD Radeon set, NVIDIA containers, Vulkan overlays |
| `power` | Device idle states, custom Arkhe power plans |
| `branding` | Black theme, Arkhe icon and wallpaper |
| `cleanup` | Deep clean and CompactOS |
| `security` | Defender/UAC/Core Isolation — **OS HANDLES THIS** |
| `fixes` | Taskbar/wallpaper repair, runtimes, restore mitigations |
| `misc` | Everything else that didn't fit cleanly elsewhere |


## Installing

**Option A — prebuilt ISO (recommended):**

1. Go to [arkheos.xyz](https://arkheos.xyz) and download the latest ArkheOS ISO — a debloated Windows 11 25H2 image with the playbook already applied.
2. Flash it to a USB drive using a tool like [Rufus](https://rufus.ie/).
3. Boot from the USB and install. See [INSTALL.md](INSTALL.md) for step-by-step instructions.
4. Once Windows boots, use the **Arkhe Toolbox** on your desktop and the `Configuration\` playbooks in this repo to layer on any additional tweaks.

**Option B — apply the playbook yourself:**

1. Install [AME Wizard](https://ameliorated.info/) and get a clean Windows 11 ISO.
2. Only load the ArkheOS playbook from this repo's [Releases](https://github.com/Fola2x/ArkheOS/releases) or the pinned [Discord](https://discord.gg/xRB9BkNerz) link — never a random third-party copy.
3. Build your ISO with the playbook applied, or run it against an existing install.
4. Once Windows boots, use the **Arkhe Toolbox** on your desktop and the `Configuration\` playbooks to apply whatever else you want.

## Requirements

- Windows 11, build 26200 (25H2) — other builds are not supported
- Internet connection during install
- A USB drive, 8GB or larger recommended, for flashing the ISO

## Contributing

Pull requests are welcome. Read through `Configuration\` and `Executables\` before opening one — every tweak should be traceable to a real registry key or command, not guessed. Keep new categories consistent with the existing folder layout (one `.yml` per category in `Configuration\`, its script in `Executables\`).

## Contributors

- [Fola2x](https://github.com/Fola2x)

<!-- more contributors to be added here -->

## Contact

- Discord: [discord.gg/xRB9BkNerz](https://discord.gg/xRB9BkNerz)
- GitHub: [github.com/Fola2x](https://github.com/Fola2x)

## License

MIT. See [`LICENSE`](LICENSE) for details.
