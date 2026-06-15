# Kylin Core
<img align='right' src='assets/logo.png' width='120' style='border-radius: 28px;' alt="kylin core logo">

**English** | [简体中文](./zh/README.md)

A homebrew cheat loader and real-time game modifier for PS5, built for the PlayStation 5 homebrew ecosystem.

[![Latest release](https://img.shields.io/github/v/release/aydencharles/kylin-core-release?label=Release&logo=github&color=blue)](https://github.com/aydencharles/kylin-core-release/releases/latest)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](./LICENSE)
[![GitHub License](https://img.shields.io/github/license/aydencharles/kylin-core-release)](./LICENSE)
[![Platform](https://img.shields.io/badge/platform-PS5_(4.xx_–_12.xx)-brightgreen)]()

## Features

1. **Real-time cheat toggle** — enable or disable cheats anytime during gameplay, changes apply instantly
2. **Multi-format support** — supports `.shn` / `.mc4` / `.json` cheat files, all from a single flat directory
3. **Automatic game detection** — no manual title ID needed; the tool auto-detects the running game
4. **Single-tool solution** — no extra modules, no `ps5debug-NG`, no additional dependencies
5. **Stable in-game operation** — no freeze on APR games
6. **Simple directory layout** — drop cheat files into `/data/kylin/cheats` and you're done

## Compatibility Status

- PS4 games (running on PS5): ✅ Supported
- PS5 native games: ✅ Supported
- PS5 games with APR: ✅ Supported
- Firmware: Compatible with jailbroken PS5 consoles running **4.xx through 12.xx**
- Cheat formats: `.shn` · `.mc4` · `.json`

## Installation

See [`guide/installation.md`](guide/installation.md)

### Quick Start

1. Copy `kylin-core.elf` and `IV0000-KYLN00003_00-KYLINCORELAUNCHR.pkg` to a USB drive
2. Load `kylin-core.elf` via [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager)
3. Install `.pkg` via **Settings → Debug Settings**
4. Launch **Kylin Core** from the home screen

> [!IMPORTANT]
> Must be loaded via PLDMGR first, otherwise the UI may not display properly.

## Usage

```
1. Launch your game
2. Open Kylin Core from the PS5 home screen
3. The tool auto-detects the running game
4. Toggle cheats on/off as needed
5. Return to game — changes apply instantly
```

## Cheat Directory

All cheat files are stored at `/data/kylin/cheats`.

- Place all cheat files directly in this directory
- No subfolders allowed — flat structure only

## Known Issues

- Some cheats depend on specific firmware versions
- Cheat behavior depends on the quality of its implementation
- Must be loaded via PLDMGR before launching the UI

## Sponsor

- [Ko-fi](https://ko-fi.com/kylincore): support the development of Kylin Core

## Credit

- [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager): PS5 ELF loader
- [PS5 Payload SDK](https://github.com/ps5-payload-dev/sdk): open-source SDK for PS5 payload development
- The PS5 homebrew community — exploit researchers, SDK maintainers, and payload loader authors

## License

This project is licensed under the [MIT License](LICENSE).
