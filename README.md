# A lightweight and professional 1v1 duel engine designed in pure Skript with zero external addons required!

---

## 📌 Overview
The **SQDual** project is custom-built for Minecraft servers (compatible with modern versions 1.21.1+ Paper / Purpur) to provide a fast, stable dual combat experience, complete with interactive GUIs, win-streak statistics systems, and full arena management.

---

## ✨ Features

* **Integrated Duel System (/duel):** Challenge any player directly via commands or by sneaking and right-clicking (Shift + Right Click) a player to select an appropriate kit from the menu.
* **Leaderboards:** Automatically displays the top 3 players with the highest win streaks for each kit directly inside the kit selection GUI.
* **Arena & Spawn Management:** A complete administrative system via the `/sqd` command to set spawns (Spawn 1 & 2), block-breaking regions (Pos1 & Pos2), and save/link arenas.
* **Edit Mode:** Toggle edit mode to save current kits and configure hub coordinates with ease.
* **Spectator System:** Use the `/spectator <player>` command to watch ongoing matches completely hidden, accompanied by an Inspect Player tool to check health, hunger, potion effects, and armor.
* **Profile Settings GUI:** A dedicated interface for each player to manage duel requests, allow spectators, auto-queue, and hide players to reduce lag.
* **Protection & Auto-Cleanup:** 
  * Offhand protection to prevent dropping or swapping system items.
  * Command blocker during combat.
  * Automatic rollback of broken blocks and projectile cleanup upon match completion or script reload.

---

## ⚠️ Current Limitations
> **Note to Users:** The script is **not 100% complete** at the moment, and it lacks some deep features found in large paid plugins. 
> * You may encounter limited advanced customization options.
> * The system is built to be lightweight and functional, but it is **under active development** and will receive gradual, major updates over time!

---

## 🎮 Quick Options
You easily control all script settings from the `options:` section at the top of the file:
* Customizing system message prefixes.
* Number of rounds required to win (`rounds_to_win`).
* Countdown times, delays, and max match duration (Time Out) before ending automatically.
* Toggling the command blocker and floor breaking permissions for specific kits.

---

## 🌐 Links
* **Browse My Other Works:** [Click here to view other scripts and projects by me (e.g., SQKoth - King of the Hill)](https://github.com/amajd3078/SQKoth---King-of-the-hill)

---
> Developed and maintained by **amajd3078**.
