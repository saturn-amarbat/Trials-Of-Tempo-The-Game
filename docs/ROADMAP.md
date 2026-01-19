# Trials of Tempo — Roadmap

_Last updated: 11/05/2025 (by Saturn)_

We develop in phases with a top-down approach: implement core ideas first, then fine-tune visuals and polish.

## Phase 1: Design the game characters and objects

(NPC, main character, collectible objects, items and powerups)

- Find out how to implement these in p5.play (research examples)
- Experiment with custom designs using p5.play functions

### Tasks

- [ ] Create final animated character GIF sprites (Frankie) — replace placeholder art in `drawPlayer()`
- [ ] Design and import obstacle sprites — replace placeholder rectangles in `Obstacle.draw()`
- [ ] Design powerup animations — replace placeholder shapes in `drawPowerup()`
- [ ] Create and import boss sprite + attack animations — replace placeholder in `drawBoss()`
- [ ] Confirm final soundtrack imports (Cacola tracks) and match stages
- [ ] Update title screen & menu visuals

## Phase 2: Level design

One strong level with eight stages for deadline feasibility.

### Tasks

- [ ] Review Frankie's Level 1 layout sketch and match camera movement
- [ ] Add distinct visual changes per stage (color shifts, parallax tweaks)
- [ ] Sync stage patterns to BPM (start at 140 BPM)
- [ ] Add tutorial hints in early beats (e.g., “Press ↑ to fly”)
- [ ] Plan locked stages (Level 2–6 placeholders hidden for now)

## Phase 3: Implement mechanics

Core interactions and abilities, tuned to rhythm.

### Tasks

- [ ] Integrate rhythm-based obstacle spawns (`onBeat()`)
- [ ] Refine jetpack control and fuel rate
- [ ] Balance shield/speed powerups and durations
- [ ] Add hit effects when colliding with obstacles
- [ ] Add simple boss AI with multi-phase attacks
- [ ] Add beat pulse visuals (screen flashes, camera shake tied to BPM)

## Phase 4: Test and improve

Polish and bug fixing.

### Tasks

- [ ] Test collision logic (`checkCollision()`)
- [ ] Verify health, score, and combo systems
- [ ] Add visual polish — particles, glow, transitions
- [ ] Sync soundtrack transitions (title → level → boss → credits)
- [ ] Adjust difficulty curve per stage
- [ ] Confirm state transitions (`title`, `playing`, `victory`, etc.)

## Phase 5: Finalize

Final cleanup and packaging.

### Tasks

- [ ] Insert final credits (`drawCredits()` with roles + real names)
- [ ] Clean code comments, remove placeholders, ensure clarity
- [ ] Organize project folders: `/assets/sprites/`, `/assets/music/`, `/scripts/`
- [ ] Test full-screen and scaling for 1920×1080
- [ ] Create “How to Play” for slides/UI overlay
- [ ] Export playable `.zip` or publish via GitHub Pages

## Current Work (as of 11/12)

- Saturn: Home screen design + character choosing; gameplay iteration
- Frankie: Character design and Level 1 (8 stages; 2–5 minutes)
- Tsuyoshi: Refactor into reusable components

References: p5.js drafts

- https://editor.p5js.org/Saturn_A/sketches/ySWKm_4vM
- https://editor.p5js.org/tsuyosi81/sketches/-dYIafUx7
