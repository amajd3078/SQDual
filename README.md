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

## 💻 Commands & Detailed Usage

### 👥 Player Commands (No Permission Required)

* **`/duel <player>`**
  * **Description:** Sends a 1v1 duel request directly to the specified target player. This action opens the Kit Selection GUI, allowing you to choose the desired kit/kit type before sending the request.

* **`/spectator <player>`**
  * **Description:** Teleports you into spectator mode for an ongoing match involving the target player. You become completely invisible to the players in the match and receive an **Inspect Player** hotbar item to check their active potion effects, armor durability, health, and hunger.

* **`/sqsettings`**
  * **Description:** Opens your personal Profile Settings GUI. From here, you can toggle:
    * Accepting or declining incoming duel requests.
    * Allowing or blocking spectators during your matches.
    * Enabling Auto-Queue mode to jump into matches faster.
    * Hiding/Showing other players in the lobby to eliminate lag.

---

### 🛡️ Admin Commands (`Permission: sqdual.admin`)

All administrative management is controlled using the main `/sqd` command branch:

* **`/sqd editmode`**
  * **Description:** Toggles administrative edit mode on or off. Enabling this grants you access to full kit creation tools, location setting commands, and inventory management options.

* **`/sqd sethub`**
  * **Description:** Sets the global duel lobby/hub spawn point at your current exact position and direction. All players returning from finished matches or typing hub commands will be sent here.

* **`/sqd savekit <kit_name>`**
  * **Description:** Saves your current inventory, armor, offhand item, and active potion effects under the specified kit name.

* **`/sqd seticon <kit_name>`**
  * **Description:** Sets the display icon item for the specified kit based on the item currently held in your main hand. This icon appears in the Kit Selection GUI.

* **`/sqd setpos1 <arena_name>`**
  * **Description:** Sets the first corner boundary (Position 1) of the block-breaking region for the specified arena.

* **`/sqd setpos2 <arena_name>`**
  * **Description:** Sets the second corner boundary (Position 2) of the block-breaking region for the specified arena.

* **`/sqd setspawn1 <arena_name>`**
  * **Description:** Sets Player 1's starting spawn point for the specified arena at your current location and viewing direction.

* **`/sqd setspawn2 <arena_name>`**
  * **Description:** Sets Player 2's starting spawn point for the specified arena at your current location and viewing direction.

* **`/sqd savearena <arena_name>`**
  * **Description:** Finalizes and registers the arena in the database after all positions (`pos1`, `pos2`, `spawn1`, `spawn2`) have been properly assigned.

* **`/sqd link <arena_name> <kit_name>`**
  * **Description:** Links a specific arena to a designated kit. Matches using this kit will automatically route to and utilize this linked arena.

* **`/sqd reload`**
  * **Description:** Safely reloads the script configuration, applies new changes, and restores active arena blocks without interrupting data integrity.

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
* **Discord Community:** [Join my Discord Server](https://discord.gg/28pTmAYCwH)
* **Browse My Other Works:** [Click here to view other scripts and projects by me (e.g., SQKoth - King of the Hill)](https://github.com/amajd3078/SQKoth---King-of-the-hill)

---
> Developed and maintained by **amajd3078**.
