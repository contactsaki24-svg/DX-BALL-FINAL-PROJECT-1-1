
# DX-BALL (Retro Arcade Game in C & Raylib)

A feature-rich, classic retro **DX-Ball / Breakout** clone built completely from scratch using the **C programming language** and the **Raylib** graphics library. This project features multiple difficulty modes, progressive levels, custom power-ups, high-score tracking with local file persistence, and immersive retro audio.

---

## ✨ Key Features

*Custom Difficulties:** Choose between *Easy*, *Medium*, and *Hard* modes that dynamically scale the ball speed.
*Level Progression:** 3 uniquely designed levels with custom brick layouts, visual backgrounds, and durability mechanics (including unbreakable bricks).
*Exciting Power-Ups: 
  W (Expand Paddle): Increases your paddle size.
  + (Extra Life): Grants an additional life (up to 5).
  S (Slow Ball): Slows down the ball speed.
  L (Laser): Equip your paddle to shoot lasers at bricks!
  X (Anti-Life): Watch out—this trap reduces your life.
  $ (Bonus Score): Instant points booster.
 (Bomb): Clears out nearby bricks instantly.
*Persistent High Scores: Automatically tracks top players and saves scores locally to `highscores.txt`.
*Audio System: Features background music tracks for menus and gameplay, alongside sound effects for brick breaks, paddle hits, and game milestones.
*Mute Control: Press `M` anytime during the game to toggle audio on/off.

---

## 🛠️ Prerequisites & Dependencies

To compile and run this game, ensure you have:
1. **A C Compiler:** GCC, Clang, or MSVC.
2. **Raylib Library:** Installed and properly linked on your system.
3. **Resources Folder:** A `resources/` directory containing all required textures (`.png`), sound effects (`.wav`), and music (`.mp3`).

---

## ⚙️ How to Build and Run

### For Linux (GCC)
Open your terminal inside the project directory and run:
```bash
gcc main.c -lraylib -lGL -lm -lpthread -ldl -lrt -lX11 -o dxball
./dxball

```

### For Windows (MinGW)

Using MinGW-w64 in your terminal:

```bash
gcc main.c -lraylib -lopengl32 -lgdi32 -lwinmm -o dxball.exe
dxball.exe

```

---

## 🕹️ Controls

| Key | Action |
| --- | --- |
| `LEFT / RIGHT Arrow` or `A / D` | Move Paddle Left / Right |
| `SPACEBAR` | Launch Ball / Fire Lasers (when powered up) |
| `ESC` | Pause Game / Go Back / Quit |
| `M` | Toggle Audio (Mute / Unmute) |

---

## 📁 Project Structure

```text
├── main.c              # Core game engine, states, physics, and rendering
├── highscores.txt      # Local high-score records storage
└── resources/          # Asset folder
    ├── menu_bg.png     # Main menu background texture
    ├── bg1.png         # Level 1 background texture
    ├── bg2.png         # Level 2 background texture
    ├── bg3.png         # Level 3 background texture
    ├── ball_r9.png     # Ball texture
    ├── *.wav           # Sound effects (break, hit, confirm, etc.)
    └── *.mp3           # Background music tracks


```
---
You can watch the gameplay in youtube also. link: https://youtu.be/bj1bZ04CGAc?si=hD3t7JlsBecunzju

## 👨‍💻 Author

Built with passion using C and Raylib.
