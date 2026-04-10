# Schema

This workspace uses a folder-as-object model and a layered fiction operating system.

The goal is not only to keep canon stable, but to keep long fiction writable, reviewable, and compelling.

## Core model

- One folder can represent one story-bearing object.
- A scene is a local event bundle.
- `aftermath.md` is the structured update hub for all scene consequences.
- Long-form truth is separated into layers so memory does not become the source of truth.

## Object contract

Every object folder must contain:

- `entity.md`: what this object is
- `agent.md`: persona and speaking/acting rules
- `state.md`: current status in the world
- `links.md`: relationships and references
- `hooks.md`: scene hooks, tensions, secrets, or possible uses

Advanced long-form object files:

- `evolution.md`: checkpoint-to-checkpoint change history
- `thematic-role.md`: what this object carries at the theme level

Objects may represent:

- characters
- locations
- items
- forces
- factions
- rumors
- institutions
- symbolic or atmospheric pressures

## Scene contract

Every scene folder must contain:

- `brief.md`: intent of the scene
- `cast.md`: summoned object agents
- `draft.md`: generated scene text or notes
- `aftermath.md`: structured consequences and propagation notes

Advanced long-form scene files:

- `emotion-map.md`: POV, dominant emotion, texture, intensity, and relation to nearby scenes

`aftermath.md` is the update hub.
Write the scene, then write the aftermath, then derive downstream updates from the aftermath.

## Arc contract

Required arc boards:

- `character-state-arc.md`
- `relationship-arc.md`
- `world-conflict-arc.md`
- `foreshadow-payoff-arc.md`

Recommended advanced arc boards:

- `thematic-compass.md`

## Architecture contract

Required architecture boards:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `pov-map.md`

Recommended advanced architecture boards:

- `resonance-map.md`
- `storyline-weave.md`

## Reader, emotion, and traction contract

Stories expected to survive beyond a short pilot should maintain:

- `01_world/pulse/emotional-pulse.md`
- `01_world/reader/reader-memory-model.md`
- `01_world/reader/misreading-design.md`
- `01_world/subtext/subtext-registry.md`
- `01_world/traction/traction-log.md`

## Thread contract

Required thread boards:

- `plot-thread-ledger.md`

Each thread entry should track:

- id
- name
- category
- status
- introduced in
- latest touch
- maturity
- deadline
- reader-memory risk
- reminder plan
- intended payoff
- owners
- notes

Recommended statuses:

- `introduced`
- `active`
- `maturing`
- `due`
- `closed`
- `broken`
- `retired`

## Timeline contract

Required timeline boards:

- `master-timeline.md`

Timeline truth records:

- when scenes happen
- event order
- elapsed time
- off-page time when relevant
- age / season / calendar implications
- what is already locked into canon

## Canon contract

Required canon boards:

- `canon-laws.md`
- `continuity-watchlist.md`

Recommended advanced canon boards:

- `taboo-registry.md`

## Checkpoint contract

At the end of every major act, volume, or irreversible reveal, create a snapshot in `01_world/checkpoints/`.

Each checkpoint should summarize:

- locked plot facts
- current object states
- current arc positions
- active and resolved threads
- chronology up to the cutoff
- contradictions avoided or still risky
- handoff conditions for the next act or volume

## Index contract

At minimum, keep:

- `01_world/indexes/index.md`
- `01_world/indexes/log.md`

As the project grows, also maintain:

- `object-index.md`
- `character-index.md`
- `thread-dashboard.md`

## Naming

- One object = one folder.
- Use short, stable folder names in lowercase with hyphens.
- Use stable numeric prefixes for volume, act, chapter, scene, and checkpoint boundaries.

## Operating cadence

### Scene-close

- save or revise the scene folder
- write `aftermath.md`
- update affected object `state.md`
- update `hooks.md` if new obligations or scene levers appeared
- update local or immediate timeline truth
- update `emotion-map.md` if the project is using scene-level emotion tracking

### Chapter-close

- update affected arc boards
- update `plot-thread-ledger.md`
- update `chapter-map.md`
- update `reader-memory-model.md` if memory state changed
- update `emotional-pulse.md`
- update `continuity-watchlist.md` if risk appeared
- record traction in `traction-log.md`

### Act-close

- create a checkpoint
- review due threads and unresolved obligations
- review character and relationship arc movement
- review architecture drift

### Volume-close

- create a checkpoint
- review canon laws and continuity watchlist
- review `thematic-compass.md`
- review `resonance-map.md`
- sync manuscript output with the frozen state

## Authority model

The hierarchy still matters:

- checkpoints > canon > timeline > objects > scenes > arcs > threads > pulse > reader > subtext > traction > architecture > manuscript

The workspace also uses a query-based authority matrix.
See `00_system/AUTHORITY_MATRIX.md`.

## Planning vs canon rule

Always distinguish between:

- written past
- frozen checkpointed past
- live current state
- planned future
- reader-facing derived output

The future may be revised.
The frozen past may not be casually rewritten.

## Source ingest rule

Raw notes and external materials belong in `02_sources/`.

Suggested source statuses:

- `raw`
- `parsed`
- `canon-integrated`
- `deprecated`

Suggested creative intake streams:

- `fragments`
- `research`
- `mood-boards`
- `voice-notes`

See `00_system/SOURCE_INGEST_PROTOCOL.md`.

## Scene partition rule

Flat `01_world/scenes/` is acceptable for a pilot.

Recommended transition:

- pilot or single-volume draft: flat allowed
- by `volume-002`: partition by volume
- by large multi-volume scale: partition by volume and act
- when chapter count becomes large: promote chapter folders beneath act folders

## Ultra-long-form anti-collapse rule

When the story becomes large, never trust memory alone.
Before generating major new material, the agent should inspect:

- relevant object folders
- relevant scene aftermaths
- relevant arc boards
- active thread entries
- relevant timeline entries
- latest checkpoint
- relevant chapter / act plan
- reader-memory and traction state when suspense matters

## Source of truth

- raw notes and source materials live in `02_sources/`
- structured world truth lives in `01_world/objects/`
- scene truth lives in `01_world/scenes/`
- long-range continuity truth lives in `01_world/arcs/`
- future story structure lives in `01_world/architecture/`
- open obligations live in `01_world/threads/`
- emotional rhythm lives in `01_world/pulse/`
- reader memory and misreading live in `01_world/reader/`
- hidden meaning tracking lives in `01_world/subtext/`
- page-turn and volume-turn devices live in `01_world/traction/`
- chronology truth lives in `01_world/timeline/`
- stable rules and contradiction tracking live in `01_world/canon/`
- frozen milestone summaries live in `01_world/checkpoints/`
- reader-facing compiled output lives in `03_manuscript/`
