<div align="center">

# ArkheOS

**Best performance. No strings attached.**

A free, open-source Windows 11 AME playbook built for maximum performance — trimmed, tuned, and yours to inspect line by line.

[![Version](https://img.shields.io/badge/version-1.1-white?style=for-the-badge&labelColor=050505)](https://github.com/Fola2x/ArkheOS/releases)
[![Windows](https://img.shields.io/badge/Windows-11%2023H2%20%C2%B7%2025H2-white?style=for-the-badge&labelColor=050505)](#requirements)
[![License](https://img.shields.io/badge/license-open%20source-white?style=for-the-badge&labelColor=050505)](#license)
[![Discord](https://img.shields.io/discord/0?style=for-the-badge&label=Discord&labelColor=050505&color=white)](https://discord.gg/xRB9BkNerz)

[Download](https://github.com/Fola2x/ArkheOS/releases) · [Discord](https://discord.gg/xRB9BkNerz) · [Report an issue](https://github.com/Fola2x/ArkheOS/issues)

</div>

---

## About

ArkheOS is an [AME Wizard](https://ameliorated.info/) playbook for Windows 11 — it applies on top of a normal Windows install rather than replacing it. Prepare for maximum performance and enjoy: privacy hardened, bloat removed, and a full library of opt-in tweaks you control instead of a black box that decides for you.

Everything ArkheOS does is a plain `.yml` playbook and a folder of `.bat` scripts. Nothing is hidden in a compiled binary — open `Configuration\` and `Executables\` and read exactly what runs before you ever install it.

## What the installer actually does

ArkheOS keeps the automated install deliberately small:

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

1. Install [AME Wizard](https://ameliorated.info/) and get a clean Windows 11 ISO.
2. Only load the ArkheOS playbook from this repo's [Releases](https://github.com/Fola2x/ArkheOS/releases) or the pinned Discord link — never a random third-party copy.
3. Build your ISO with the playbook applied, or run it against an existing install.
4. Once Windows boots, use the **Arkhe Toolbox** on your desktop and the `Configuration\` playbooks to apply whatever else you want.

## Requirements

- Windows 11, build 22631, 26100, or 26200 (23H2 – 25H2)
- Internet connection during install

## Contributing

Pull requests are welcome. Read through `Configuration\` and `Executables\` before opening one — every tweak should be traceable to a real registry key or command, not guessed. Keep new categories consistent with the existing folder layout (one `.yml` per category in `Configuration\`, its script in `Executables\`).

## Contributors

- [Fola2x](https://github.com/Fola2x)

<!-- more contributors to be added here -->

## Contact

- Discord: [discord.gg/xRB9BkNerz](https://discord.gg/xRB9BkNerz)
- GitHub: [github.com/Fola2x](https://github.com/Fola2x)

## License

Open source. See [`LICENSE`](LICENSE) for details.
