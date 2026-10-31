# Mossy Island — Made by Klaus

A small browser-playable island-life and focus game. The repository now contains a self-contained playable prototype rather than a mockup screenshot.

## Play it

Open **[the GitHub Pages build](https://klauslark.github.io/mossy-island/)** after Pages is enabled for this repository, or download the repository and open `index.html` in a current Chrome or Edge browser.

No npm, build system, or external game engine is required. The Google Fonts import is optional; the game itself runs offline after the page is loaded.

## Controls

- **WASD / arrow keys** — walk.
- **Click / tap a reachable location** — walk toward it.
- **E** — interact with Lumo or a nearby resource.
- **Build** — select build mode, then click a free location.
- **Esc** — cancel build mode.
- **My tasks** — add and complete personal tasks.
- **Focus** — start or pause a 5, 15, 25, or 45 minute session.

## Included in this prototype

- A seeded 64 × 48 tile island assembled at runtime from individual terrain cells (grass, sand, path, rock, water).
- Camera tracking, keyboard movement, click-to-walk path search, and basic collision.
- Independently rendered world objects: trees, flowers, rocks, cottage, camp and Lumo.
- Animated water highlights, tree sway, player idle/walk bob and a progressing island clock.
- Introductory dialogue and a small quest chain.
- Resource gathering, building placement, task capture and a focus timer.
- One local persistent save in browser storage.

## Save data

The save is stored in the browser's localStorage under `mossy-island-world-v1`. Clearing browser data removes the save. Export/backup UI is not included yet; do not clear site data if you want to keep progress.

## Honest status

This is a **playable prototype**, not a finished commercial game and not a clinically validated ADHD treatment. The world is a tile-based scene, not a single background image. Its current art is stylized canvas-drawn placeholder art; dedicated hand-painted sprite sheets, layered avatar customization, rich NPC schedules, sound, accessibility settings, robust save migration, and native Windows packaging are not yet complete. There has not yet been a verified smoke test on the user's Windows machine.

## Roadmap

See [ROADMAP.md](ROADMAP.md). The release gate is real interaction and reliable play, not a promotional screenshot.
