# 🧊 Cub3D — 42 School Project

> **A first-person 3D game inspired by Wolfenstein 3D, built using raycasting and MiniLibX.**

---

## 📖 Table of Contents
- [About](#-about)
- [Features](#-features)
- [Installation](#️-installation)
- [Usage](#-usage)
- [Controls](#-controls)
- [File Format](#️-file-format)
- [Project Structure](#-project-structure)
- [Bonus Features](#-bonus-features)
- [Screenshots](#-screenshots)
- [Authors](#-authors)

---

## 🧠 About

**Cub3D** is a project from **42 School** that introduces students to **raycasting** — a rendering technique used in early 3D games like *Wolfenstein 3D*.
The goal is to create a simple 3D game engine where the player can move inside a maze made of walls, using a 2D map as reference.

It is also the first major step into **graphics programming**, **mathematical logic**, and **event handling** using the **MiniLibX** library.

---

## ✨ Features

- 🧭 3D rendering using **raycasting**
- 🧱 Walls with **textures**
- 🌈 Floor and ceiling **colors**
- 🚶‍♂️ Smooth **player movement** and **rotation**
- 📁 Parsing of `.cub` configuration files
- 🧩 Error handling (invalid maps, missing textures, etc.)
- 🔄 Memory management and clean exit handling

---

## ⚙️ Installation

Clone the repository and compile the project:

```bash
git clone https://github.com/<your-username>/cub3d.git
cd cub3d
make
```

This will compile the project and create the `cub3D` executable.

To clean object files:
```bash
make clean
```

To clean everything (binary + objects):
```bash
make fclean
```

To recompile:
```bash
make re
```

---

## 🚀 Usage

Run the program with a `.cub` map file:

```bash
./cub3D maps/example.cub
```

Example:
```bash
./cub3D maps/maze.cub
```

---

## 🎮 Controls

| Key | Action |
|-----|--------|
| `W` | Move forward |
| `S` | Move backward |
| `A` | Move left (strafe) |
| `D` | Move right (strafe) |
| ⬅️ / ➡️ | Rotate view left/right |
| `ESC` | Exit game |

---

## 🗺️ File Format

A `.cub` configuration file defines:
- Wall textures (`NO`, `SO`, `WE`, `EA`)
- Floor and ceiling colors (`F`, `C`)
- Map layout (with characters `1`, `0`, `N`, `S`, `E`, `W`)

Example:
```cub
NO ./textures/north.xpm
SO ./textures/south.xpm
WE ./textures/west.xpm
EA ./textures/east.xpm

F 220,100,0
C 225,30,0

1111111111
1000000001
1011000001
1001000001
1000000001
1000000001
1111111111
```

Legend:
- `1` → Wall
- `0` → Empty space
- `N`, `S`, `E`, `W` → Player starting direction

---

## 🧩 Project Structure

```
cub3d/
├── includes/           # Header files
│   ├── cub3d.h
│   ├── parsing.h
│   └── raycasting.h
├── srcs/
│   ├── main.c
│   ├── parsing/
│   ├── raycasting/
│   ├── movement/
│   └── utils/
├── textures/           # XPM texture files
├── maps/               # Example .cub maps
├── libmlx/             # MiniLibX library
├── Makefile
└── README.md
```

---

## 🧠 Bonus Features

> (only if you’ve implemented them — you can remove or edit this section)

- 🪞 **Mini-map** display
- 🔫 **Animated doors or sprites**
- 🌌 **Mouse rotation**
- 💡 **Lighting effects**
- 🎵 **Background music or sounds**

---

## 🖼️ Screenshots

| In-game View | Mini-map Example |
|---------------|-----------------|
| ![Gameplay](./assets/gameplay.png) | ![Minimap](./assets/minimap.png) |

---

## 👥 Authors

👤 **Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- 42 Intra: `yabounna`

---

## 🏁 Project Goals

✅ Learn fundamentals of **computer graphics**  
✅ Understand **raycasting** mathematics  
✅ Use **MiniLibX** and event hooks  
✅ Write **clean, modular, and norm-compliant** C code  

---

### 🏆 Final Note

> “Cub3D is not just a project, it’s your first window into 3D graphics and game engines.  
> Mastering it builds a strong foundation for computer graphics and engine design.”
