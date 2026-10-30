# Mossy Island — Made by Klaus

**Mossy Island** — cozy, story-driven productivity game about arriving on a small island and rebuilding a home at your own pace.

The central design principle: the island is a real, persistent game world assembled from a tile map and independent entities — never a single flattened background image.

## Product pillars

- **One permanent world.** The player has one continuing island and one save identity. No New Game or delete-world button in the normal UI.
- **A living 2D world.** Tile-based terrain, independent objects, player movement, collision, camera tracking, depth sorting, ambient animation and NPC interaction.
- **Gentle productivity.** Focus sessions and small real-life tasks help the island grow. The app should support ADHD-friendly use: low-friction start, clear next action, forgiving pacing, low visual clutter, predictable feedback and no punitive streak mechanics.
- **A story that teaches by doing.** The player arrives after a long journey, meets Lumo and learns the island through short contextual quests.
- **Local-first and recoverable.** Autosaves, rotating snapshots and explicit export/import backups.

## Current prototype

A playable vertical-slice prototype is being developed in the working build. It currently contains a seeded 56×42 tile map, five terrain families with variants, camera-follow movement, collision, independent sprite entities, basic player/tree/water animation, resource nodes, Lumo, introductory quests, building placement, focus timer, tasks, avatar colour controls, save snapshots and a local developer panel.

See [PROJECT_STATUS.md](PROJECT_STATUS.md) and [ROADMAP.md](ROADMAP.md) for known gaps and next milestones.

## Run the current local build

The current intermediate package is delivered separately as **Mossy_Island_Intermediate.zip**. Extract it and run `Start_Mossy_Island.bat` on Windows, or open `index.html` in Chrome/Edge.

The runtime is an offline-first HTML Canvas prototype. It is not yet a signed native Windows executable.

## Controls

- WASD / arrow keys — move
- Click ground — walk toward location
- E — interact when close to an object or NPC
- Build menu, then click a clear ground tile — place an object
- Escape — cancel placement / close modal
- Ctrl+Shift+D — local developer tools

## Safety of saves

The game uses a single permanent world ID in local storage. Export a backup before clearing browser data or moving the project to another browser profile. Import validates the world ID and saves a recovery snapshot before replacing current state.

## Project status honesty

This repository is the canonical project home. The local prototype and its asset package are under active development; do not treat the current vertical slice as a finished commercial product. Browser automation in the development container is currently blocked by its browser policy, so end-to-end runtime QA must also be performed on a normal Windows desktop.
