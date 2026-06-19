# Installation

<a href="https://ko-fi.com/kylincore"><img src="https://img.shields.io/badge/Ko--fi-Support-FF6433?style=for-the-badge&logo=kofi&logoColor=white" alt="Support Kylin Core on Ko-fi"></a>

If you find this project helpful, please consider supporting its continued development. Your support is greatly appreciated!

## Requirements

- A jailbroken PS5 with an active ELF loader
- [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager) installed

## Files

| File | Description |
|---|---|
| `kylin-core.elf` | Payload binary, loaded via PLDMGR |
| `IV0000-KYLN00003_00-KYLINCORELAUNCHR_GAME_SECTION.pkg` | System app package — installs launcher under **Game** category |
| `IV0000-KYLN00003_00-KYLINCORELAUNCHR_MEDIA_SECTION.pkg` | System app package — installs launcher under **Media** category |

> [!NOTE]
> Choose **one** PKG based on where you want the launcher to appear on the home screen.

## Steps

1. Copy `kylin-core.elf` and your chosen `.pkg` file to the root of a USB drive

2. Insert the USB drive into your PS5

3. Open **PS5 Payload Manager (PLDMGR)** and load `kylin-core.elf`

4. Go to **Settings → Debug Settings** and install the `.pkg` file

5. Launch **Kylin Core** from the home screen

> [!IMPORTANT]
> You must load `kylin-core.elf` via PLDMGR **before** launching the app. Otherwise the UI will not load properly.

## Cheat Files

Place your cheat files (`.shn`, `.mc4`, `.json`) into:

```
/data/kylin/cheats
```

- Flat directory only — no subfolders
- The tool auto-detects the running game and matches available cheats

## Uninstallation

1. Delete the app from the home screen (Options → Delete)
2. Remove `/data/kylin/cheats` if no longer needed
