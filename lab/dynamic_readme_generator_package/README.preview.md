# 🎨 [The Realm]: A Color-Shattered World

Welcome to the design archive for **[The Realm]**,  
A narrative-rich, hue-fractured fantasy world where emotion, memory, and magic are bound to color.

> [!NOTE]
> **[The Realm]** is a placeholder name.

---

## 📘 Table of Contents

- [🎮 Game Design](#-game-design)
  - [🕹 Game Mechanics & Core System](#-game-mechanics--core-system)
  - [💎 Items – Catalogue](#-items--catalogue)
  - [📺 UI](#-ui)
- [🌍 World Overview](#-world-overview)
- [📜 Timeline & History](#-timeline--history)
- [🧬 Main Character – The Prismwalker](#-main-character--the-prismwalker)
- [🧠 Personality System](#-personality-system)
- [🌀 In-Game Visual Concepts](#-in-game-visual-concepts)
  - [📷 Example Scenes](#-example-scenes)
- [🪄 Myths & Omens](#-myths--omens)
- [🎭 NPC Characters](#-npc-characters)
- [👹 Enemies – Bestiary Index](#enemies--bestiary-index)
- [🎨 Color Codex](#-color-codex)
- [🌑 Endgame](#-endgame)
- [🗂️ File Structure & Visual Assets](#file-structure--visual-assets)
- [TODO List](#todo-list)

---

## 🎮 Game Design

Heavy-lore, color-themed fantasy RPG game project.

[See Game Design Document - First Draft ►][gdd_draft]

### 🕹 Game Mechanics & Core System

- [See Game Mechanics Reference ►][core_systems]
- [See Hue-Binding System ►][hue_binding]
- [See Hue-Affinity Tiers Logic ►][hue_affinity]

### 💎 Items – Catalogue

Catalog of the major artifacts, relics, consumables, powers, and tools grouped by function.

- [Check Items – Catalogue ►][items]

### 📺 UI

- [Check UI Design Concepts ►][ui]

---

## 🌍 World Overview

<div align="center">
  <h3>[The Realm]</h3>
  <img src="./assets/world-map-overview.png" alt="World Map Preview" width="300">
  <br><i>"The Prism shattered. Now the hues rule alone..."</i><br>

  <strong><a href="./docs/03-world/overview.md">Read full world breakdown ►</a></strong>
</div>

<div align="center">

|                                                 |                                  |
| ----------------------------------------------- | -------------------------------- |
| 🟢 [**Huevale**][huevale]       | Verdant growth & stealth puzzles |
| 🔴 [**Vireya**][vireya]         | Ember-forged battlefield zone    |
| 🔵 [**Iriseld**][iriseld]       | Floating sea-cliff archipelago   |
| 🟣 [**Myrrala**][myrrala]       | Twilight glades of illusion      |
| 🟡 [**Luxeran**][luxeran]       | Mirage-laced golden desert       |
| 🤎 [**Auralith**][auralith]     | Rusted ruins & fossil memory     |
| ⚫ [**Nullshade**][nullshade]   | The broken, colorless core       |

</div>

---

## 📜 Timeline & History

> "All color was once one — until we tried to own it."

[See full timeline ►][timeline]

- 🕊️ Age of Light — Unified Core
- 🔮 Age of Echoes — Color Orders rise
- ⚔️ Color War & Nullshade Plague
- 💥 The Shattering — Realms fracture
- 🌑 The Dimming Cycle — Your era begins

---

## 🧬 Main Character – The Prismwalker

<div align="center">
  <h3>The Prismwalker</h3>
  <img src="./assets/player/prismwalker-sketch.png" alt="Prismwalker Concept Art" width="200">
  <br><i>"Born without color. Bound to none. Shaped by every hue."</i><br>

  <strong><a href="./docs/02-content/characters/player/prismwalker.md">Character breakdown ►</a></strong>
</div>

### Features

- Customizable visual
- Dialogue influenced by color
- Combat system with Huebinding & Prismatic Burst

---

## 🧠 Personality System

> "Your hues don't just affect your skills — they shape your voice."

[Click to see full system ►][personality_system]

---

## 🌀 In-Game Visual Concepts

<div align="center">
  <h3>Huebound Skin Concept</h3>
  <img src="./assets/player/hue-skin-example.png" alt="Huebound Skin Concept" width="500">

  <strong><a href="./docs/06-art/in-game-visuals.md">Click to see Character Visuals Document ►</a></strong>
</div>

### Features

- Veins and aura based on hues
- Prism Core glow
- Clothing & trail effects by hue
- HUD integration suggestion

### 📷 Example Scenes

Some example in-game scene scripts for each region.

[Click to see in-game scene examples ►][scene_examples]

---

## 🪄 Myths & Omens

> "The first color was silence."  
> "When the sun weeps amber, even the blind must wear masks."

[Click to see more prophecies & cryptic sayings ►][myths_and_omens]

---

## 🎭 NPC Characters

[Click to see important NPCs list ►][npcs]

Includes:

- Character + item ideas
- Usage in worldbuilding
- Dialogue

---

## 👹 Enemies - Bestiary Index <a id="enemies--bestiary-index"></a>

Bestiary for creatures from each region, with lore and details.

Structure per entry:

- Name: Evocative and thematic, often involving color or light-based terms.
- Flavor Quote: A short, poetic line — mysterious, lore-rich, often ironic.
- Visual Design: Concise description of physical appearance.
- Behavior: Specific, interesting mechanic that ties into the world/lore.
- Weakness/Counterplay: Each has at least one specific counter or condition.

[Click to see Bestiary Index by Region ►][bestiary]

---

## 🎨 Color Codex

> [!IMPORTANT]
> This list is the origin of this whole thing.

[Click to see complete color/style list ►][colors]

---

## 🌑 Endgame

> [!WARNING]
> Spoilers.

[Click to see what happens in the final moments (WIP) ►][endgame]

---

## 🗂️ File Structure & Visual Assets <a id="file-structure--visual-assets"></a>

Generated README links are managed through:

```text
readme.config.toml
README.template.md
tools/generate_readme.py
```

When docs or assets move, update `readme.config.toml` and regenerate the README.

---

## TODO List <a id="todo-list"></a>

### Todo - Enemies

- Counter coverage audit: every enemy lists a counter; verify each counter is:
  1. in `items/index.md`
  2. introduced before the fight
  3. optionally has at least one alternative: skill-based or environment-based

### Tools & Misc

- [Engineering tooling notes ►][tooling]

<!-- AUTO-GENERATED-REFERENCE-LINKS:START -->
<!-- Generated by tools/generate_readme.py. Edit readme.config.toml, not this block. -->

<!-- Docs -->
[auralith]: ./docs/03-world/regions/auralith.md
[bestiary]: ./docs/02-content/bestiary/index.md
[colors]: ./docs/06-art/palette.md
[core_systems]: ./docs/01-design/systems/overview.md
[endgame]: ./docs/04-narrative/scenes/endgame.md
[gdd_draft]: ./docs/01-design/gdd-draft.md
[glossary]: ./docs/_shared/meta/glossary.md
[hue_affinity]: ./docs/01-design/systems/hue-affinity.md
[hue_binding]: ./docs/01-design/systems/hue-binding.md
[huevale]: ./docs/03-world/regions/huevale.md
[in_game_visuals]: ./docs/06-art/in-game-visuals.md
[iriseld]: ./docs/03-world/regions/iriseld.md
[items]: ./docs/02-content/items/index.md
[luxeran]: ./docs/03-world/regions/luxeran.md
[main_character]: ./docs/02-content/characters/player/prismwalker.md
[myrrala]: ./docs/03-world/regions/myrrala.md
[myths_and_omens]: ./docs/03-world/myths-and-omens.md
[naming_conventions]: ./docs/_shared/meta/naming-conventions.md
[npcs]: ./docs/02-content/characters/npcs/index.md
[nullshade]: ./docs/03-world/regions/nullshade.md
[personality_system]: ./docs/01-design/systems/personality-system.md
[scene_examples]: ./docs/04-narrative/scenes/scene-examples.md
[timeline]: ./docs/03-world/timeline.md
[tooling]: ./docs/08-engineering/tooling.md
[ui]: ./docs/05-ux/ui.md
[vireya]: ./docs/03-world/regions/vireya.md
[world]: ./docs/03-world/overview.md

<!-- Assets -->
[hue_skin_example]: ./assets/player/hue-skin-example.png
[meeting_thalera]: ./assets/in-game-visuals/meeting-thalera.png
[prismwalker_sketch]: ./assets/player/prismwalker-sketch.png
[world_map]: ./assets/world-map-overview.png

<!-- AUTO-GENERATED-REFERENCE-LINKS:END -->
