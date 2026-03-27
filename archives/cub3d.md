# cub3D

## Description
**cub3D** is a **team project** at [42](https://42.fr), implementing a **Wolfenstein-like** game using the **MLX42** library ([MLX42 GitHub](https://github.com/codam-coding-college/MLX42)). It features a **raycasting engine**, **map parsing**, and **player interactions** with extended **gameplay features** beyond the base project requirements.

## Project PDFs
- [📄 Project PDF (EN)](link_to_pdf_eng)
- [📄 Projet PDF (FR)](link_to_pdf_fra)

## Team Contributions

| Contributor | Responsibilities                                                                                                                                              |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **oroy**    | - Raycaster engine<br>- Elevator & segworld logic<br>- Door & sprite animations<br>- In-game controls menu<br>- Texture choice & design                       |
| **cdumais** | - Cubfile parsing & validation<br>- Multi-map logic<br>- Player controls & event system<br>- Minimap<br>- Pixel drawing functions<br>- VXF (shadow rendering) |

---

# Requirements

## 🔹 **Base Requirements**
cub3D must include:
- A **raycasting engine** that simulates a 3D environment.
- **Texture loading** for walls from a `.cub` file.
- **Movement & rotation mechanics** for the player.
- **Wall collisions** to prevent walking through obstacles.
- **Custom map parsing** with `.cub` files defining world structure.
- **Minimap rendering**.

## 🔹 **Bonus Features**
Additional features implemented beyond the base requirements:
- **Multi-map support** (transitioning between different `.cub` files).
- **Elevator system** (functional moving platforms).
- **Optional floor and ceiling textures** in `.cub` files.
- **Texture rendering toggle** (switch between wireframe & textures).
- **Interactive mode** (cursor activation for object interactions).
- **Improved minimap with dynamic colors & radar mode**.

## 🔹 **Extra Features**
Additional gameplay and visual improvements:
- **Player sprint mechanic** (`Left Shift` for speed boost).
- **Secondary raycasting for minimap field of view simulation**.
- **Glitch effect rendering toggle** (disabling floor & ceiling updates).
- **Procedural animated sprites** (randomly placed, blue flames effect).
- **Student extraction system** (fetches 42 profile images during compilation).
- **Interference effect in elevators** (pixel noise simulating radio disruption).

---

# 📜 Cubfile Details

## **Valid `.cub` File Structure**
- **Must have a `.cub` suffix**.
- **Can include the following elements in any order** (except the map, which must be last):
  - **Wall textures** (one per direction).
  - **Optional floor & ceiling textures** (`FL`, `CE`).
  - **Floor & ceiling colors** (`F`, `C`).
  - **Map layout** defining walls, floors, and elevator positions.

## **Map Rules & Symbols**
| Symbol             | Meaning                         |
| ------------------ | ------------------------------- |
| `0`                | Walkable space                  |
| `1`                | Wall                            |
| `N`, `S`, `E`, `W` | Player spawn (facing direction) |
| `3`                | Elevator                        |

### **🚪 Elevator Constraints**
- Must be **bordered by three `1`s** and **one `0`**.
- Must have **at least one valid path leading to it**.
- Example of valid elevator placement:

```plaintext
  1111111111
  10000000E1
  1000001111
  1000000001
  1000111111
  100011  31
  1000111111
  1000000001
  1111011111

Example of a Valid .cub File

NO ./textures/wall_north.xpm
SO ./textures/wall_south.xpm
WE ./textures/wall_west.xpm
EA ./textures/wall_east.xpm

FL ./textures/floor.xpm
CE ./textures/ceiling.xpm

F 50,116,167
C 200,206,235

1111111111
10000000E1
1000001111
1000000001
1000111111
100011  31
1000111111
1000000001
1111011111

Invalid .cub Examples

🔗 Invalid Cubfiles Directory


---

🎯 Bonus Features

🏗️ Elevator System

Replaces doors with automated elevators.

Opens/closes based on proximity.

Interactive buttons inside the elevator:

Green buttons appear when inside.

Click to move up/down.

Doors close before movement and open upon arrival.



🚀 Multi-Map Support

Allows launching multiple .cub files.

Elevator required in .cub file to transition between levels.

Command Example:

./cub3D maps/level1.cub maps/level2.cub maps/level3.cub

Rules for valid elevators:

One per level.

3 walls, 1 open side.

Correct .cub file syntax.



🌌 Segworld Mechanic

Edge case handling for levels without an elevator:

A hidden "segworld" level is created as the next destination.

Blocks following levels from loading.



🖼️ Student Extraction Mechanic

Extracts the evaluating student's picture from a 42 Mac path.

Fallback default image if extraction fails.

Handled via the Makefile during compilation.



---

🗺️ Minimap System

Two Minimap Modes

1️⃣ Centered Tile-Based Minimap

Fixed grid showing entire map.

Player tile highlighted (optional).


2️⃣ Radar-Style Minimap (Top-Right)

Round minimap with a colored border.

Player icon is a triangle, pointing in the facing direction.

Dynamic minimap colors:

Walkable areas: Average floor texture color (if available).

Walls: Average color of corresponding wall textures.

Player icon: Inverted color of walkable tile.


Field of view simulation:

Secondary raycaster displays colored rays from the player.

Approximate values, tweakable via macros.



Radar-Mode Extras

Interference Effect inside elevators.

Simulated using random pixel noise.




---

🎮 UI & Controls
(tableau here)


---

📦 Installation & Compilation

Dependencies

MLX42 (Installation Guide)

CMake (Required for MLX42)

GNU Make


Build Instructions

git clone https://github.com/SaydRomey/cub3D.git
cd cub3D
make
./cub3D maps/example.cub


---

🖥️ Showcase



🔗 Demo Video


---

📝 Credits

Authors: @oroy & @cdumais

42 School Project

Inspired by Wolfenstein 3D

