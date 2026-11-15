# ⚒️ ForeverCraft – Profession Leveling Planner

[![WoW Versions](https://img.shields.io/badge/WoW-Forever%20%7C%20Classic%20%7C%20TBC%20%7C%20WotLK-00ccff.svg)](#)
[![Dependencies](https://img.shields.io/badge/Dependencies-None%20(Standalone)-brightgreen.svg)](#)
[![Optional](https://img.shields.io/badge/Optional-Auctionator-orange.svg)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](#)

*[🇩🇪 Deutsche Beschreibung weiter unten](#-forevercraft--berufe-leveling-planer-deutsch)*

---

## 🌐 English Description

**ForeverCraft** is a lightweight, standalone in-game profession leveling planner and shopping list calculator inspired by *wowcraft.io*, specifically tailored for **WoW: Forever** and Classic progression clients. 

Instead of alt-tabbing to external websites, ForeverCraft calculates your optimal crafting path, aggregates all required raw materials, deducts items you already own in your bags or bank, and calculates live Auction House costs directly inside the game.

### ✨ Key Features

* **🎨 Modern Dark-Theme UI:** Clean, compact, and movable two-column interface in the style of *wowcraft.io*.
* **🌍 100% International (i18n Ready):** All recipes, reagents, and profession detections work strictly via `ItemID` and `SpellID`. Item names, icons, and links automatically resolve in your client's native language (**EN, DE, FR, ES, RU, PT, KO, ZH**) without localization errors.
* **🔄 Automatic Skill Detection:** Automatically detects your character's current skill rank when opening the window or switching professions, and updates live as you gain skill points (`SKILL_LINES_CHANGED`).
* **🎒 Smart Inventory & Bank Deduction:** Optional checkbox to automatically subtract materials you already own in your bags or bank (`GetItemCount`). Owned materials are visually marked and excluded from the remaining cost calculation.
* **💰 Live Auctionator Integration:** 
  * Queries live Auction House prices via the official Auctionator API (`GetAuctionPriceByItemID`).
  * Safe fallback to vendor prices if Auctionator is not installed or no scan data is available.
  * **One-Click AH Search:** Send all remaining missing materials directly to Auctionator's shopping tab (`MultiSearchExact`) with a single click.
* **⚡ Zero Bloat:** 100% standalone Lua code. No heavy external libraries (Ace3, LibStub, etc.) required.

### 🛠️ Supported Professions

* 🧪 **Alchemy**
* 🔨 **Blacksmithing**
* 🍖 **Cooking**
* ✨ **Enchanting**
* ⚙️ **Engineering**
* 💎 **Jewelcrafting**
*  leather **Leatherworking**
* 🧵 **Tailoring**

### 💬 Slash Commands & Controls

* `/wfc` or `/forevercraft` — Toggles the ForeverCraft planner window.
* **Minimap Button:** Left-click to toggle the window, drag with left-click to reposition around the minimap.
* **Shift-Click on Items:** Links any recipe or material from the planner directly into your active chat input.

### 📦 Installation

1. Download the latest release from **CurseForge** or **GitHub Releases**.
2. Extract the `ForeverCraft` folder into your World of Warcraft `Interface/AddOns/` directory.
3. *(Optional)* Install **Auctionator** to enable live Auction House pricing and one-click shopping searches.

---

## 🇩🇪 ForeverCraft – Berufe-Leveling-Planer (Deutsch)

**ForeverCraft** ist ein kompakter, eigenständiger Ingame-Berufe-Planer und Einkaufslisten-Rechner im Stil von *wowcraft.io*, entwickelt für **WoW: Forever** sowie Classic-Clients.

Kein lästiges Alt-Tabben mehr auf externe Webseiten: ForeverCraft berechnet deinen optimalen Leveling-Pfad von deinem aktuellen Skill bis zum Wunsch-Ziel, fasst alle benötigten Rohstoffe zusammen, zieht deinen Taschen- und Bankbestand automatisch ab und zeigt dir die Live-Auktionshaus-Preise direkt im Spiel an.

### ✨ Highlights & Funktionen

* **🎨 Modernes Dark-Theme UI:** Übersichtlich, kompakt und frei verschiebbar – zweispaltiges Layout mit Leveling-Schritten links und einer interaktiven Einkaufsliste rechts.
* **🌍 100 % Sprachunabhängig (i18n):** Alle Rezepte, Rohstoffe und Berufsabfragen basieren intern strikt auf `ItemID`s und `SpellID`s. Dadurch funktioniert das Addon fehlerfrei auf jedem Sprachclient (**DE, EN, FR, ES, RU** etc.) und lädt Icons, Namen sowie Tooltips dynamisch über den Spiel-Cache nach.
* **🔄 Automatische Skill-Erkennung:** Liest beim Öffnen oder beim Wechsel des Berufs automatisch deinen aktuellen Charakter-Skill aus (inklusive Live-Aktualisierung beim Craften und `↻`-Sync-Button).
* **🎒 Taschen- & Bank-Abzug:** Zieht per Checkbox alle Materialien, die du bereits im Inventar oder auf der Bank besitzt, automatisch von der Einkaufsliste und den Restkosten ab.
* **💰 Volle Auctionator-Integration:**
  * Live-Preise für alle Rohstoffe über die offizielle Auctionator-API (`GetAuctionPriceByItemID`).
  * Stabiler Fallback auf Händlerpreise, falls Auctionator nicht installiert ist.
  * **1-Klick AH-Suche:** Übergibt alle noch fehlenden Materialien mit einem Klick direkt an das geöffnete Auktionshaus (`MultiSearchExact`).
* **⚡ Leichtgewichtig & Schnell:** Reiner, sauberer Lua-Code ohne externe Zusatzbibliotheken.

### 💬 Slash-Befehle & Bedienung

* `/wfc` oder `/forevercraft` — Öffnet oder schließt das Planer-Fenster.
* **Minimap-Button:** Linksklick zum Öffnen/Schließen, gedrückte linke Maustaste zum Verschieben am Minimap-Rand.
* **Shift-Klick auf Gegenstände:** Postet den Item-Link eines Schritts oder Rohstoffs direkt in den Chat.

### 📦 Installation

1. Lade die neueste Version über **CurseForge** oder **GitHub Releases** herunter.
2. Entpacke den Ordner `ForeverCraft` in dein Verzeichnis `Interface/AddOns/`.
3. *(Optional)* Installiere **Auctionator**, um Live-Auktionshauspreise und die direkte Einkaufssuche zu nutzen.
