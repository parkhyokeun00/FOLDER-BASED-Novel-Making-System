# Schema

This workspace uses a folder-as-object model.

## Folder contract

Every object folder should contain:

- `entity.md`: what this object is
- `agent.md`: persona and speaking/acting rules
- `state.md`: current status in the world
- `links.md`: relationships and references
- `hooks.md`: scene hooks, tensions, secrets, or possible uses

Every scene folder should contain:

- `brief.md`: intent of the scene
- `cast.md`: summoned object agents
- `draft.md`: generated scene text or notes
- `aftermath.md`: consequences and updates to propagate

## Arc contract

Longer stories should also maintain arc boards under `01_world/arcs/`.

Required arc boards:

- `character-state-arc.md`
- `relationship-arc.md`
- `world-conflict-arc.md`
- `foreshadow-payoff-arc.md`

These are not object folders.
They are long-range tracking boards for the whole story.

## Architecture contract

Stories that may extend to long-form or ultra-long-form should also maintain planning boards under `01_world/architecture/`.

Required architecture boards:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `pov-map.md`

These boards define intended future structure.
They are planning documents, not frozen canon.

## What each arc means

### Character state arc

Track how each major character changes across the story.

Examples:

- resignation -> anger -> murderous intent -> helplessness -> ruin
- innocence -> suspicion -> obsession -> collapse

### Relationship arc

Track how key relationships evolve across scenes and acts.

Examples:

- love -> strain -> guilt -> conspiracy -> joint destruction
- trust -> rivalry -> betrayal -> dependence

### World conflict arc

Track the large hidden truth, pressure, or structural conflict that keeps the story moving.

Examples:

- exploitation structure behind the art world
- curse governing a village
- concealed murder that shaped the town
- class system, war pressure, religious power, inherited debt

### Foreshadow / payoff arc

Track planted motifs, objects, lines, promises, and when they return.

Examples:

- sunset
- hand washing
- money envelope
- knife
- "How long do we have to endure?"

## Thread contract

Longer stories should maintain unresolved story promises under `01_world/threads/`.

Required thread boards:

- `plot-thread-ledger.md`

This ledger tracks:

- open plot threads
- mysteries
- emotional promises
- political or world tensions
- setup/payoff obligations that are not yet closed

## Timeline contract

Stories with more than a few scenes should maintain chronology under `01_world/timeline/`.

Required timeline boards:

- `master-timeline.md`

Timeline truth records:

- when scenes happen
- event order
- elapsed time
- age / season / calendar implications
- what is already locked into canon

## Canon contract

Stories expected to survive long serialization should maintain canon control under `01_world/canon/`.

Required canon boards:

- `canon-laws.md`
- `continuity-watchlist.md`

`canon-laws.md` records stable world rules.
`continuity-watchlist.md` records possible contradictions, risky drift, and unresolved continuity concerns.

## Checkpoint contract

At the end of every major act, volume, or irreversible reveal, create a snapshot in `01_world/checkpoints/`.

Checkpoint files are frozen summaries of canon up to that point.
They should not be silently rewritten after later planning changes.

Recommended moments for a checkpoint:

- end of act
- end of volume
- major status-quo break
- major death, reveal, or world change

## Object types

Suggested top-level object categories:

- `characters`
- `locations`
- `items`
- `forces`

`forces` can include weather, beliefs, factions, curses, moods, rumors, seasons, or historical pressure.

## Naming

- One object = one folder.
- Use short, stable folder names in lowercase with hyphens.
- Example: `01_world/objects/characters/mara`
- Example: `01_world/objects/locations/old-well`
- Example: `01_world/objects/forces/ash-rain`

For architecture and checkpoint files, use stable numeric prefixes when scale matters.

Examples:

- `volume-001`
- `act-01`
- `chapter-012`
- `checkpoint-001-end-of-act-01`

## Update rule

If a scene changes the world, update the affected object folders after updating the scene folder.

If a scene changes a long-running narrative axis, also update the relevant arc board.

If a scene resolves or escalates an open promise, also update the relevant thread ledger.

If a scene locks new chronology, also update the timeline board.

If a scene crosses a major boundary, consider creating a checkpoint.

## Arc update rule

After each important scene, check whether it changes:

- a character's trajectory
- a relationship's trajectory
- the world-level conflict
- a planted motif or its payoff
- an unresolved plot thread
- the story timeline
- a future chapter or act plan

If yes, record that change in `01_world/arcs/`.

## Authority model

- Object folders are the source of truth for individual entities.
- Scene folders are the source of truth for scene-level events.
- Arc boards are the source of truth for long-range story continuity.
- Thread ledgers are the source of truth for unresolved promises and obligations.
- Timeline boards are the source of truth for event ordering.
- Architecture boards are the source of truth for future intent, but they may change.
- Checkpoints are frozen canon summaries for all material before their cutoff.

## Planning vs canon rule

Always distinguish between:

- written past
- frozen checkpointed past
- live current state
- planned future

The future may be revised.
The frozen past may not be casually rewritten.

## Ultra-long-form anti-collapse rule

When the story becomes large, never trust memory alone.
Before generating major new material, the agent should inspect:

- relevant object folders
- relevant arc boards
- active plot threads
- master timeline
- latest checkpoint
- relevant chapter / act plan

## Source of truth

- Raw notes go into `02_sources/`.
- Structured world truth lives in `01_world/objects/`.
- Scene truth lives in `01_world/scenes/`.
- Long-range continuity truth lives in `01_world/arcs/`.
- Future story structure lives in `01_world/architecture/`.
- Open obligations live in `01_world/threads/`.
- Chronology truth lives in `01_world/timeline/`.
- Stable rules and contradiction tracking live in `01_world/canon/`.
- Frozen milestone summaries live in `01_world/checkpoints/`.
