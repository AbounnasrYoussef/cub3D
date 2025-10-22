# cub3D

from pathlib import Path

# Contenu du README.md
readme_content = """# 🧊 Cub3D — 42 School Project

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
