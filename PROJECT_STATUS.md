# Project status — vertical slice under development

Last updated: 2026-10-30

## Implemented in the current working build

- Procedural fixed-seed island grid (56 × 42, 64 px tiles), assembled at runtime from separate terrain textures.
- Five terrain families with multiple art variations: grass, path, sand, water and rock.
- Camera follows the player; four-direction movement, click-to-walk and terrain/object collision.
- Independent world entities with depth sorting: trees, bushes, flowers, rocks, buildings, furniture, resources and NPC.
- Ambient animation: player walk frames, tree sway and water shimmer.
- Gathering nodes for wood and stone, interaction range and guide character Lumo.
- Introductory quest chain, inventory, building placement and saved object coordinates.
- Focus countdown, pause/resume, rewards and world clock.
- Task list, avatar palette customisation, hidden local developer panel.
- One permanent world ID, local autosave, rotating local snapshots and save export/import.

## Current local package

The current working directory is mossy-island-product/; a test archive is available as Mossy_Island_Intermediate.zip. It contains the source, art files and Windows start script.

## Verification

- [x] JavaScript syntax check with Node.js (node --check src/game.js).
- [x] HTML local references checked for missing files.
- [x] ZIP archive integrity checked.
- [ ] Full browser runtime check. The browser in the current development container rejects both file and localhost navigation with ERR_BLOCKED_BY_ADMINISTRATOR; this is an environment restriction, not a successful test. Must be checked on a normal Windows Chrome/Edge installation.
- [ ] Windows desktop smoke test.

## Known gaps

- The current character editor mainly recolours a base character sprite; it is not yet a full layered wardrobe with independently selectable hair/clothes/accessories.
- The map is seeded and generated from a deterministic island mask/path data; it is not yet a hand-authored multi-region world.
- NPC behaviour and schedule are basic. More autonomous movement, daily routines and dialogue are needed.
- Art and interaction coverage is not final; every object needs its own readable interaction feedback and appropriate hitbox.
- Accessibility controls (reduced motion, adjustable audio, UI scale, remappable controls) still need implementation.
- A native signed Windows build and installer do not exist yet.

## Developer tools

Ctrl+Shift+D opens the local test panel. It can advance world time, finish focus, grant materials and advance quests. It is intentionally absent from the normal game interface.

## Important repository note

The repository currently contains the product README and roadmap. The complete working source/art package has not yet been committed here. Do not claim GitHub is a full source backup until src/ and the required assets/ files appear in the repository tree.
