# Mossy Island — Made by Klaus

An offline-first productivity game built around one persistent island. The gameplay world is a seeded 56×42 tile map rendered from terrain tiles and independent sprite entities, not a flattened screenshot.

## Run
Extract the project archive, keep the `assets` directory beside `index.html` and `src`, then launch `Start_Mossy_Island.bat`. Chrome or Edge opens the game in an app-like window. No npm, build step, or network connection is required.

## Controls
- WASD / arrows: walk.
- Click reachable land: move to the point.
- E: interact with nearby resources or Lumo.
- Select a build item, then click a free location to place it.
- Esc: cancel placement.
- Ctrl+Shift+D: developer tools (time, resources, quest testing).

## Current vertical slice
- Fixed-seed 56×42 tile world, camera tracking, keyboard movement, click-to-walk and basic collisions.
- Independent terrain and world sprites; five player frames, tree sway, water shimmer and a day/night overlay.
- Lumo, introductory quests, resource gathering, inventory and placed buildings saved at world coordinates.
- Focus timer, task list, avatar palette, single world ID, automatic local saves and export/import.
- First-arrival story scene and local developer console.

## Save safety
There is one world slot and no reset/delete-world command. Progress is stored locally in the browser and rolling snapshots are kept when possible. This is not cloud storage: browser data cleanup or a different browser profile can make local saves unavailable. Export backups periodically.

## Honest limitations
This is an early browser prototype, not a finished commercial ADHD product. Some terrain crops are not final seamless tiles. Avatar customization currently recolours existing pixels instead of using a fully layered wardrobe. Click-to-walk is direct steering, not full pathfinding. Native Windows packaging, sound, gamepad, remappable controls, richer NPC schedules and a completed browser runtime test remain future work. It is not clinically validated.

## Source
`index.html` — title/arrival/game screens.  
`src/game.js` — map, entities, quests, interaction, focus timer, saving.  
`src/style.css` — interface and visual motion.  
`assets/terrain`, `assets/sprites`, `assets/story` — art resources.
