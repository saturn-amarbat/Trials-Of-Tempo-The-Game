# Trials of Tempo

An endless, rhythm-driven action game built with p5.js and p5play. Fly, dash, and collect while the music ramps difficulty over time.

> For the full game concept and development plan, see:
>
> - docs/GAME_DESIGN.md
> - docs/ROADMAP.md

## Features

- Music-driven difficulty: BPM and scroll speed scale with loop count
- Parallax background, pulse effects, and shockwave visuals
- Powerups (speed, shield), dash mechanic with cooldown UI
- Customizable character sprites and animated collectibles
- Robust audio guards for reliable web demos

## Tech Stack

- p5.js (graphics, input)
- p5.sound (audio)
- p5play + Planck.js (helpers/physics utilities)

## Run Locally

```bash
cd Trials_Of_Tempo_Game_Project
python3 -m http.server 8000
```

Open http://localhost:8000, click once to enable audio, press any key to skip the intro.

## Controls

- WASD / Arrow keys: Move
- Shift: Dash
- Space: Use powerup (when queued)
- P: Pause / resume
- R: Restart
- M: Return to menu

## Deploy (GitHub Pages)

- Push this folder to a GitHub repo (e.g., `trials-of-tempo`)
- In Repository Settings → Pages → Deploy from branch → set branch and folder
- Visit the published URL (click once in the page to enable audio)

## Credits

- Team: Saturn (Lead), Yoshi (Developer), Frankie (Artist)
- Music: Cacola

## Repo Name

Recommended: `trials-of-tempo` (alternatives: `tempo-runner`, `rhythm-runner-p5`).

## Notes

- Favicon included (SVG)
- Libraries are loaded locally for reliability on GitHub Pages
- If hosting elsewhere, CDNs work too but local files avoid third-party outages
