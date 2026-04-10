# Novel Agent Wiki

This workspace is a folder-based novel wiki where each object in the world can be represented as its own agent folder.

It is currently kept in a structure-only state.
No active story world, pilot cast, or manuscript is loaded.

## Core concept

- One folder can represent one object in the story world.
- An object may be a character, location, item, weather system, social force, rumor, institution, event seed, or any other story-bearing entity.
- Each object folder contains structured attributes and a persona prompt so it can be "summoned" during scene creation.
- A master agent orchestrates scenes by selecting and combining relevant object agents.
- `aftermath.md` acts as the update hub so scene consequences can propagate into the wider system without relying on memory.

## World model

- `00_system/`: operating rules, templates, checklists, and master-agent contracts
- `01_world/objects/`: one folder per world object
- `01_world/scenes/`: one folder per scene or scene bundle
- `01_world/arcs/`: long-running change tracks for characters, relationships, world conflicts, motifs, and theme
- `01_world/architecture/`: series, volume, act, chapter, POV, resonance, and storyline planning boards
- `01_world/threads/`: plot-thread and promise ledgers
- `01_world/timeline/`: chronology and event-order truth
- `01_world/pulse/`: emotional rhythm across scenes and chapters
- `01_world/reader/`: reader memory, desire, fear, and controlled misreading
- `01_world/subtext/`: hidden meaning and surface/underlayer tension
- `01_world/traction/`: chapter and volume closing pull devices
- `01_world/canon/`: world laws, continuity watchlists, and taboo boundaries
- `01_world/checkpoints/`: frozen canon snapshots at act and volume milestones
- `01_world/indexes/`: indexes, dashboards, and logs
- `02_sources/`: raw notes, research, fragments, mood boards, and source material
- `03_manuscript/`: compiled reader-facing drafts

## Scale hierarchy

This workspace can operate at multiple scales:

- Series
- Volume
- Act
- Chapter
- Scene
- Beat

## Operating cadence

This workspace uses layered closure rather than one giant update pass.

### Scene-close

- write or revise the scene
- write `aftermath.md`
- update local object state and immediate timeline

### Chapter-close

- update arcs
- update threads
- update chapter map
- update reader, pulse, and traction layers

### Act-close

- freeze a checkpoint
- review due threads and drift

### Volume-close

- freeze a checkpoint
- audit canon, theme, resonance, and manuscript sync

## Long-form support

For longer fiction, object state alone is not enough.

This workspace also tracks:

- `character-state-arc.md`: how major characters change over time
- `relationship-arc.md`: how important relationships evolve
- `world-conflict-arc.md`: the major hidden truth, structure, or ongoing conflict
- `foreshadow-payoff-arc.md`: planted motifs, lines, objects, and their eventual return
- `thematic-compass.md`: what the story is really arguing and how each volume varies that argument

Objects are the local truth.
Arcs are the long-range truth.

## Reader-facing support

To keep a long project from becoming technically coherent but unreadably inert, the workspace also tracks:

- reader memory and forgetting
- controlled misreading
- emotional rhythm
- subtext
- chapter and volume traction
- POV limitations and voice stability

## Authority

The workspace uses both:

- a truth hierarchy
- a question-by-question authority matrix

If two boards disagree, resolve the conflict through `00_system/AUTHORITY_MATRIX.md` rather than intuition.

## Current state

- the workspace contains system rules, templates, and empty live-world scaffolding
- previous pilot-specific objects, scenes, checkpoints, and manuscript content have been removed
- the next step is to test the structure with a completely new story case rather than extending old material
