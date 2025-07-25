# Reforger Persistent Framework (RPF)

**RPF** is a modular, developer-friendly persistence system for *Arma Reforger*, designed to allow servers to **save and restore game state across restarts**. Whether you're running large-scale monthly campaigns or immersive roleplay scenarios, RPF provides a stable and extensible backend for world persistence.

---

## ✅ Core Goals

- **Modular Design** – Enable only what your server needs: player data, vehicles, zones, etc.
- **Community Friendly** – Open source (MIT), well-documented, and built for collaboration.
- **Minimal Dependencies** – Server-side only, lightweight by design.
- **Open Source** – Public repo with versioned commits and release tags.
- **Future Proof** – Built on a versioned format to support upgrades and extensions.

---

## 📦 Core Modules

| Module            | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| `RPF_Core`        | JSON save/load engine, mission event hooks, and auto-backup system          |
| `RPF_PlayerData`  | Persists UID, faction, role, kills, deaths, and rank                        |
| `RPF_Zones`       | Captures territory ownership, control states, and capture progress          |
| `RPF_Vehicles`    | Saves location, damage state, fuel level, and ownership                     |
| `RPF_Structures`  | Restores player-built FOBs, fortifications, static structures               |
| `RPF_Campaign`    | Tracks global war status (weeks, victory points, strategic shifts)          |

Each module supports interval-based saving and consistent JSON formatting. Designed for standalone use or seamless integration into larger frameworks.

---

## 🔧 Technical Stack

- **Language**: Enfusion Script (Bohemia’s C++-like scripting language)
- **Persistence**: JSON-based (future support for binary or remote backends)
- **Framework**: Built on [Enfusion Database Framework (EDF)](https://github.com/Arkensor/EnfusionDatabaseFramework) by [Arkensor](https://github.com/Arkensor)
- **Configurable**: Fully tunable via `.json` and script-side parameters

---

## 📌 Use Cases

- **WCS/ACE-style Campaigns** – Persistent zones, battles, and supply lines across weeks
- **RP Servers** – Character stats, factions, progression retained between sessions
- **Survival Modes** – Loot, structures, and base-building that persists across restarts
- **Mod-Integrated Persistence** – Easily extendable for any mod needing save/load functionality

---

## 🛠️ Milestones

- ✅ Design architecture & MIT licensing  
- 🔄 RPF_Core + RPF_Zones MVP in progress  
- 🔄 Test mission with save/load capability  
- 🔄 Player role + faction persistence  
- 🔄 Full repo documentation and mod.io integration  
- 🔄 Vehicle, structure, and campaign state persistence  
- 🔄 Support for forks, extensions, and modular contributions  

---

## 🤝 Why This Matters

> *Arma Reforger currently lacks native persistence support.* RPF aims to solve that—providing an open, well-documented, and flexible foundation for long-form gameplay, just as **CBA** and **ACE** did for Arma 3.

This framework empowers developers and server admins to:
- Reduce setup time for persistent game modes
- Eliminate progress loss and player frustration
- Unlock dynamic, evolving campaigns
- Collaborate on a shared technical standard

---

## ⚖️ License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute the framework in both personal and commercial Reforger servers and mods. Attribution to the base project is appreciated but not required.

---

## 📂 Acknowledgements

- [Enfusion Database Framework (EDF)](https://github.com/Arkensor/EnfusionDatabaseFramework) – foundational backend layer
- Bohemia Interactive – creators of the Enfusion engine and Arma Reforger

---

## 📬 Contributions Welcome

Want to help expand RPF? Fork the repo, submit a pull request, or open an issue. Modular sub-systems and external save backends are especially welcome.

---

> ⚠️ This is an active work-in-progress. Expect commits and refactors as we build toward a stable 1.0.
