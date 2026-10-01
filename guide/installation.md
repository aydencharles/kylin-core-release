# Installation

<a href="https://ko-fi.com/0xp0co"><img src="https://img.shields.io/badge/Ko--fi-Support-FF6433?style=for-the-badge&logo=kofi&logoColor=white" alt="Support Kylin Core on Ko-fi"></a>

If you find this project helpful, please consider supporting its continued development. Your support is greatly appreciated!

## Requirements

- A jailbroken PS5 with an active ELF loader
- [PS5 Payload Manager (PLDMGR)](https://github.com/itsPLK/ps5-payload-manager) installed

## Files

| File | Description |
|---|---|
| `kylin-core.elf` | The payload. It contains the daemon, the cheat engine, and the web UI |

## Steps

1. Load `kylin-core.elf` with **PS5 Payload Manager (PLDMGR)**

2. Wait for the ready notification. The **Kylin Core** tile is under **Media** on the home screen

3. Launch **Kylin Core** from the home screen

> [!IMPORTANT]
> You must load `kylin-core.elf` via PLDMGR **before** launching the app. Otherwise the UI will not load properly.

If the tile does not show up, check `/data/kylin/logs/kylin-core.log`.

## Cheat Files

Place your cheat files (`.json`, `.shn`, `.mc4`, `.ShnExt`) into:

```
/data/kylin/cheats
```

- Flat directory only — no subfolders
- The tool auto-detects the running game and matches available cheats
- `.ShnExt` is Alpha and not fully supported yet; `.json`, `.shn` and `.mc4` are the fully supported formats

## Uninstallation

1. Stop the payload (reboot the console, or end the daemon from the UI)
2. Delete the **Kylin Core** tile from the home screen (Options → Delete)
3. Remove `/data/kylin` if no longer needed
