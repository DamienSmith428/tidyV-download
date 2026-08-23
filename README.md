# TidyV — Frontend

> **FiveM Vehicle Pack Organiser** · Made by [DS Customs](https://ds-customs.tebex.io)

This repository is the static **GitHub Pages** website for [TidyV](https://github.com/DamienSmith428/tidyV-download) — a free Windows desktop app that organises loose GTA V vehicle files into clean, ready-to-use FiveM resource folders, complete with an auto-generated `fxmanifest.lua`.

---

## What Is TidyV?

TidyV is a **Windows desktop application** for FiveM vehicle modders. Drop your vehicle folder(s) in and it:

- Scans every `.yft`, `.ytd`, and meta file inside the folder(s)
- Detects vehicle model names automatically from `vehicles.meta`, `handling.meta`, and `carcols.meta`
- Sorts base model and texture files into `stream/{model}/main/`
- Routes livery and mod variant `.yft` files (detected via `carcols.meta`) into `stream/{model}/mods/`
- Places all meta files into `data/{model}/`
- Generates a complete `fxmanifest.lua` with wildcard `files` paths and correctly typed `data_file` entries
- Supports queuing multiple folders to pack into a single resource

No subscriptions. No backend. Completely free to use.

---

## Output Structure

```
{resourceName}/
├── fxmanifest.lua
├── data/
│   └── {model}/
│       ├── vehicles.meta
│       ├── handling.meta
│       ├── carcols.meta
│       ├── carvariations.meta
│       └── vehiclelayouts.meta
└── stream/
    └── {model}/
        ├── main/
        │   ├── {model}.yft
        │   ├── {model}_hi.yft
        │   └── {model}.ytd
        └── mods/
            └── (livery / mod .yft files)
```

---

## Desktop App Requirements

| Requirement | Detail |
|---|---|
| OS | Windows 10 (1903+) or Windows 11 |
| Runtime | .NET Framework 4.8 (built into Windows 10 1903+ and Windows 11) |
| Install | None — single portable `.exe` |

---

## Links

| | |
|---|---|
| 🔗 Live Site | [damiensmith428.github.io/tidyV-download](https://damiensmith428.github.io/tidyV-download) |
| 💬 Discord | [discord.gg/HfaZHm5qJQ](https://discord.gg/HfaZHm5qJQ) |
| 🛒 DS Customs Store | [ds-customs.tebex.io](https://ds-customs.tebex.io) |
| 📦 Latest Release | [Releases](https://github.com/DamienSmith428/tidyV-download/releases/latest) |

---

## License

TidyV is free to use. Redistribution or resale of the application is not permitted without explicit permission from DS Customs.
