# SpaceRoboShooter

A free, retro-flavored twin-stick arena shooter with modern neon graphics and a head nod to classic 80s arcade survival shooters. You are alone in a walled arena against waves of robots. Rescue the wandering colonists, dodge, shoot and survive all 40 waves.

**Play it in your browser:** https://nbwillcox.github.io/SpaceRoboShooter/

Everything is generated in code: sprites are vector-drawn on the fly, and all sound effects and music are synthesized with the Web Audio API. There are no image or audio files and no build step. A sibling of [SpaceGalaShooter](https://github.com/nbwillcox/SpaceGalaShooter), [SpaceCentiShooter](https://github.com/nbwillcox/SpaceCentiShooter), [SpaceVaderShooter](https://github.com/nbwillcox/SpaceVaderShooter), [SpaceStroids](https://github.com/nbwillcox/SpaceStroids), [SpaceCommand](https://github.com/nbwillcox/SpaceCommand) and [lightCycles](https://github.com/nbwillcox/lightCycles), with the same look and feel.

## Controls

| Action | Keys |
| --- | --- |
| Move | `W` `A` `S` `D` |
| Aim | Mouse (follow the red reticle) |
| Fire (hold to auto-fire) | Left mouse button or `Space` |
| Fire in 8 directions (keyboard twin-stick) | Arrow keys |
| Smart bomb | `B`, `Shift` or right mouse button |
| Choose a free upgrade | `1` `2` `3` or click a card |
| Pause | `P` or `Esc` |

## Gameplay

- One touch from any robot or shot is fatal, so you are always moving. You start with 3 lives and earn an extra life every 25,000 points.
- **Colonists** wander the arena. Touch one to rescue it: the bonus climbs 1,000 → 2,000 → 3,000 → 4,000 → 5,000 within a wave. Colonists left alive at the end of a wave still pay out a survivor bonus.
- **Rescue meter:** every 4 colonists rescued freezes the action and lets you pick 1 of 3 free upgrades.
- **The robots:**
  - **Swarmer:** the fast, endless swarm that homes in on you.
  - **Bulwark:** indestructible. Shots only push it back, and it crushes colonists. Stay away.
  - **Mindcore:** hunts colonists and turns them into fast **Thralls**; it also fires homing missiles you can shoot down.
  - **Sentinel:** drifts around and spawns **Strikers**, which hover and fire aimed shots.
  - **Nexus:** spawns **Crawlers**, slow tanks that fire bouncing shells.
  - **Pylons:** static hazards you can shoot or avoid.
- **Power-ups** drop from the tougher robots: weapon tier (single → twin → spread → piercing lances; a death drops you one tier), rapid fire, speed boost, shield, and smart bombs (wipe the screen, but Bulwarks only get shoved away).
- Chain kills for a score multiplier (up to x8) and clear a wave without dying for a Perfect bonus.
- 40 waves in five themed arenas, with a victory screen at the end and an optional endless mode afterwards.
- Local top-10 high scores with arcade-style 3-letter initials (stored in your browser).

## Run locally

It is plain HTML/CSS/JS. Either open `index.html` directly, or serve the folder:

```bash
python -m http.server 8000
```

then visit http://localhost:8000. Desktop browsers with keyboard and mouse only for now.

## License and attribution

Licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/): free to play, share and remix **non-commercially**, as long as you give credit and **link back to this repository**: https://github.com/nbwillcox/SpaceRoboShooter

This is an original game inspired by classic arcade shooters. It uses no assets, names or code from any existing game.
