# Novel Agent Wiki

This workspace is a folder-based novel wiki where each object in the world can be represented as its own agent folder.

## Core concept

- One folder can represent one object in the story world.
- An object may be a character, location, item, weather system, social force, rumor, event seed, or any other story-bearing entity.
- Each object folder contains structured attributes and a persona prompt so it can be "summoned" during scene creation.
- A master agent orchestrates scenes by selecting and combining relevant object agents.

## World model

- `00_system/`: operating rules, templates, master-agent contract
- `01_world/objects/`: one folder per world object
- `01_world/scenes/`: one folder per scene
- `01_world/arcs/`: long-running change tracks for characters, relationships, world conflicts, and foreshadowing
- `01_world/architecture/`: series, volume, act, chapter, and POV planning boards
- `01_world/threads/`: plot-thread and promise ledgers
- `01_world/timeline/`: chronology and event ordering truth
- `01_world/canon/`: world laws and contradiction watchlists
- `01_world/checkpoints/`: frozen canon snapshots at act/volume milestones
- `01_world/indexes/`: global indexes and logs
- `02_sources/`: raw notes and source materials

## Scale hierarchy

This workspace can operate at multiple scales:

- Series
- Volume
- Act
- Chapter
- Scene
- Beat

## Working loop

1. Create or refine object folders.
2. Define or revise architecture boards when planning at volume, act, or chapter scale.
3. Ask the master agent to summon relevant object agents.
4. Generate a scene or chapter using object state, arc state, active threads, and timeline state.
5. Write back consequences into object folders and scene records.
6. Update the relevant arc, thread, timeline, and chapter boards so long-form continuity does not drift.
7. Freeze major milestones into checkpoints when an act or volume boundary is crossed.

## Long-form support

For longer fiction, object state alone is not enough.

This workspace also tracks four long-form axes:

- `character-state-arc.md`: how major characters change over time
- `relationship-arc.md`: how important relationships evolve
- `world-conflict-arc.md`: the major hidden truth, structure, or ongoing conflict
- `foreshadow-payoff-arc.md`: planted motifs, lines, objects, and their eventual return

Objects are the local truth.
Arcs are the long-range truth.

## Ultra-long-form support

To survive very long fiction, this workspace separates:

- local entity truth: `objects/`
- scene event truth: `scenes/`
- long-range emotional and structural truth: `arcs/`
- future shape and pacing plans: `architecture/`
- open promises and unresolved tensions: `threads/`
- chronological truth: `timeline/`
- frozen canon and contradiction control: `canon/` and `checkpoints/`

This means the system can keep past canon stable while still allowing future plans to change.

## Current goal

This repository currently defines the structure only. The next step is to create the first village or world and then add the first object agents.
