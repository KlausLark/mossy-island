# Roadmap

## Milestone 0 — Playable vertical slice (current)

- [x] Seeded tile-based island map (56×42)
- [x] Separate terrain families: grass, path, sand, water, rock
- [x] Separate sprite entities for vegetation, buildings, furniture, player and NPC
- [x] Camera follows player
- [x] WASD / arrow movement and click-to-walk
- [x] Tile/object collision
- [x] Depth sorting and basic ambient animation
- [x] Gatherable wood and stone nodes
- [x] Lumo NPC and first quest chain
- [x] Inventory and placement of buildings
- [x] Focus timer and simple task list
- [x] Single permanent world identity, autosave snapshots and backup export/import
- [x] Local developer time/resource/quest shortcuts
- [ ] Complete Windows desktop runtime QA
- [ ] Commit the full source and binary art package to this repository

## Milestone 1 — Make the island feel alive

- [ ] Replace placeholder player frames with directional walk/idle/interaction animation sets
- [ ] Add proper NPC idle/walk schedules, conversations and reactions
- [ ] Add object-specific interaction and gathering animations
- [ ] Add audio: restrained ambient layers, interface feedback and interaction sounds
- [ ] Add day/night and weather transitions driven by the world clock
- [ ] Add a small authored first region with clear paths, shore, camp and landmarks
- [ ] Verify collision masks for every building and large tree
- [ ] Add save migration/versioning and recovery UI

## Milestone 2 — ADHD-friendly productivity core

- [ ] One-tap "start with 5 minutes" flow
- [ ] Optional 15/25/45/60-minute focus lengths
- [ ] Gentle pause/resume, no punishment for ending early
- [ ] One visible next action at a time
- [ ] Task capture in one field; categories and planning are optional
- [ ] Start ritual and re-entry prompt after interruption
- [ ] Sensory controls: reduce motion, mute ambience, lower visual effects
- [ ] Avoid streak loss, shame copy, urgent red UI, infinite notifications and punitive reminders
- [ ] Measure engagement by return-to-task and completed focus, not total screen time

## Milestone 3 — Personalisation and content

- [ ] Layered avatar customisation (hair, face, clothes, backpack, accessories)
- [ ] More biome regions and unlockable island areas
- [ ] More buildings, furniture, vegetation and seasonal variations
- [ ] Quest authoring data separated from game code
- [ ] Content collection and discoveries
- [ ] Accessibility pass: keyboard-only, remappable keys, scalable UI, readable type and colour contrast

## Milestone 4 — Desktop product

- [ ] Package for Windows with a proper desktop shell
- [ ] Crash-safe save journal and automatic backup rotation
- [ ] Update mechanism and versioned migration
- [ ] Performance profiling on integrated GPUs
- [ ] Installer, app icon, signing and clean uninstall
- [ ] QA matrix for Windows 10/11 and common resolutions

## Release gate

A milestone is not "done" because a screenshot looks good. It needs working interaction, persistence, keyboard accessibility, no blocking defects and a documented test pass on an ordinary Windows machine.
