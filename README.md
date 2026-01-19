# Trials of Tempo
> **An endless rhythm runner where music controls the chaos.**

[![Play Now](https://img.shields.io/badge/▶️_Play_Now-GitHub_Pages-success?style=for-the-badge)](https://saturn-amarbat.github.io/Trials-Of-Tempo-The-Game/)
[![View Code](https://img.shields.io/badge/📦_View_Code-Repository-blue?style=for-the-badge)](https://github.com/saturn-amarbat/Trials-Of-Tempo-The-Game)

Fly through beat-synced obstacle courses where difficulty scales with BPM. Built entirely in **pure JavaScript + p5.js** — no build tools, just open and play.

**Perfect for:**
- 🎯 Portfolio reviewers looking for interactive demos
- 🎮 Rhythm game fans who love Geometry Dash meets Just Shapes & Beats
- 🎓 Students learning game development with p5.js
- 🏆 Game jam projects and quick prototypes

---

## 🎮 Elevator Pitch

*Trials of Tempo* is a student-built rhythm-action game where you pilot a jetpack hero through chambers that pulse, shift, and attack in sync with an EDM soundtrack. Every song loop amps up the BPM and obstacle density—stay on beat or get obliterated. Featuring 4 playable characters, custom parallax backgrounds, and a powerup system built from scratch.

---

## 🎥 Gameplay Preview

![Gameplay](assets/visuals/gameplay-preview.mp4)

> 💡 **Tip:** Convert this to GIF using `ffmpeg -i assets/visuals/Opening.mp4 -vf "fps=10,scale=640:-1" assets/visuals/gameplay.gif`

---

## ✨ Features

- **Music-driven difficulty scaling** — Game speed and obstacle density increase with BPM and loop count, keeping every run tense as you survive longer
- **Beat-synchronized visuals** — Screen pulses, camera shake, and obstacle spawns are all timed to the music's rhythm
- **Dynamic powerup system** — Speed boosts alter jet visuals; shockwave clears the screen in a burst of RGB energy
- **Dash mechanic with cooldown UI** — Slide through tight gaps with a SHIFT-powered burst, tracked by an on-screen gauge
- **Parallax scrolling backgrounds** — Multi-layer depth creates a sense of speed and immersion
- **4 customizable characters** — Unlock and swap between animated GIF sprites mid-game
- **Combo multiplier system** — Chain gem pickups to rack up massive scores
- **Local high score persistence** — Beat your best and challenge friends on the same machine

---

## 🛠️ Tech Stack

- **Pure JavaScript + p5.js** — No webpack, no build step. Clone and serve.
- **p5.sound** — Real-time audio analysis and playback rate manipulation
- **p5play + Planck.js** — Physics helpers for collision and smooth movement
- **GitHub Pages** — Deploy with zero configuration

---

## 📦 Installation & Run Locally

### Prerequisites
- Python 3 (for local server) or any HTTP server

### Steps
```bash
# 1. Clone the repository
git clone https://github.com/saturn-amarbat/Trials-Of-Tempo-The-Game.git
cd Trials-Of-Tempo-The-Game

# 2. Start a local server
python3 -m http.server 8000

# 3. Open in browser
# Navigate to http://localhost:8000
# Click once to enable audio (browser policy)
# Press any key to skip intro video
```

**Alternative servers:**
```bash
# Node.js
npx serve

# PHP
php -S localhost:8000
```

---

## 🎮 Controls

| Key | Action |
|-----|--------|
| **WASD / Arrow Keys** | Fly up, down, left, right |
| **Shift** | Dash (with cooldown) |
| **Space** | Activate queued powerup |
| **P** | Pause / resume |
| **R** | Restart run |
| **M** | Return to main menu |

---

## 📸 Screenshots

### Main Menu
![Menu Screenshot](assets/visuals/screenshot-menu.png)
> Neon RGB aesthetic with beat-synced title pulsing

### In-Game Action
![Gameplay Screenshot](assets/visuals/screenshot-gameplay.png)
> Dynamic obstacles spawning on beat with parallax depth

> 📷 **Note:** Screenshots coming soon! Run locally and capture your own gameplay.

---

## 🚀 Project Status

**Current Version:** Prototype (v0.8)  
**Status:** Active Development

### Next Steps
- [ ] Polish level design (transition zones between BPM shifts)
- [ ] Add online leaderboard (Firebase integration)
- [ ] Mobile touch controls + responsive scaling
- [ ] Boss encounter at high loop counts
- [ ] Additional character animations (damage states)

---

## 👥 Credits

### Team
- **Saturn Amarbat** — Lead Developer  
  *Game loop architecture, rhythm synchronization system, input handling, audio integration, GitHub Pages deployment, UI/UX design*
  
- **Tsuyoshi Harayama (Yoshi)** — Developer  
  *Code refactoring, modular component design, optimization*
  
- **Frankie Salud** — Artist  
  *Character sprite animation, level layout sketches, visual theme direction*

### Music
- **Cacola** — Original soundtrack (EDM compositions)

### Tools
- p5.js, p5.sound, p5play, Planck.js

---

## 🔮 Future Work

1. **Difficulty selector UI** — Easy/Normal/Hard modes with distinct balance curves
2. **Level progression** — Unlock new songs and stages with checkpoints
3. **Visual polish** — Add particle trails, screen distortion effects, and boss animations
4. **Score analytics** — Track metrics like "longest dash chain" and "perfect beat hits"
5. **Accessibility** — Colorblind mode, visual beat indicators for non-audio play

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.  
Music © Cacola — All rights reserved.

---

## 📚 Documentation

- [Game Design Doc](docs/GAME_DESIGN.md) — Full concept, narrative, mechanics
- [Development Roadmap](docs/ROADMAP.md) — Phase-by-phase task breakdown
- [Git Guide](docs/GIT_GUIDE.md) — Learn Git & GitHub workflow

---

## 🌐 Links

- **Play Live:** https://saturn-amarbat.github.io/Trials-Of-Tempo-The-Game/
- **Source Code:** https://github.com/saturn-amarbat/Trials-Of-Tempo-The-Game
- **Report Issues:** https://github.com/saturn-amarbat/Trials-Of-Tempo-The-Game/issues

---

**Made with ❤️ for ART151 — Winter 2025**
