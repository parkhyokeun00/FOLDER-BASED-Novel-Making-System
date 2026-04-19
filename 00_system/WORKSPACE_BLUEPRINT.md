# Workspace Blueprint

This document is the reconstruction guide for the current workspace.

Its purpose is:

1. to describe the structure as it exists now
2. to let the same structure be rebuilt from an empty folder without guessing

---

## 1. Current state

The workspace is intentionally in a structure-only state.

That means:

- system rules exist
- templates exist
- live world directories exist
- core board files exist
- no active cast, plot, scene set, or manuscript is loaded

This is the correct state for architecture work before a new test story begins.

---

## 2. Design philosophy

This is not a normal notes folder.
It is a layered fiction operating system.

Each layer answers a different question:

- `objects/`: what exists now
- `scenes/`: what happened locally
- `arcs/`: what is changing over long distances
- `threads/`: what promises are still open
- `timeline/`: when things happened
- `pulse/`: what the emotional rhythm is doing
- `reader/`: what the reader remembers, wants, fears, or misreads
- `subtext/`: what is being meant beneath the explicit text
- `traction/`: why the next chapter or volume must be opened
- `architecture/`: what the future is currently supposed to look like
- `canon/`: what may not be broken
- `checkpoints/`: what part of the past is frozen
- `manuscript/`: reader-facing output

---

## 3. Root structure

```text
README.md
000_*.md (optional durable clone closeout notes)
00_system/
01_world/
02_sources/
03_manuscript/
```

### Meaning

- `README.md`
  Global orientation.

- `000_*.md`
  Optional root-front durable notes for disposable clones that reached a meaningful stop state.

- `00_system/`
  Rules, contracts, checklists, templates, and reconstruction logic.

- `01_world/`
  Live story structure and runtime boards.

- `02_sources/`
  Intake layer for research, fragments, mood, and raw material.

- `03_manuscript/`
  Reader-facing output zone.

---

## 4. Exact current tree

```text
README.md
00_system/
  ACT_CLOSE_CHECKLIST.md
  AUTHORITY_MATRIX.md
  CANON_RATIFICATION_PROTOCOL.md
  CANON_CONTAMINATION_FIREWALL.md
  CHAPTER_ACCEPTANCE_GATE.md
  CHAPTER_BUILD_CHECKLIST.md
  CHAPTER_EXTENSION_GATE.md
  CHAPTER_PACKET_PROTOCOL.md
  PRE_CHAPTER_SYNC_GATE.md
  BOARD_FRESHNESS_AUDIT.md
  COMPLEXITY_BUDGET.md
  CONTINUITY_AUDIT_CHECKLIST.md
  FAILURE_RECOVERY_RULES.md
  GOLDEN_EXECUTION_FIXTURE.md
  LONGFORM_EXPANSION_PROTOCOL.md
  MASTER_AGENT.md
  NEW_STORY_BOOTSTRAP.md
  PREWRITE_SIMULATION_TEST.md
  PRODUCTION_REWRITE_MODE.md
  ROLE_MODES.md
  SCHEMA.md
  SERIES_START_PROTOCOL.md
  SYSTEM_SMOKE_AUDIT.md
  SOURCE_INGEST_PROTOCOL.md
  START_READINESS_GATE.md
  STRUCTURAL_REINFORCEMENT.md
  STRUCTURE_DONE_DEFINITION.md
  SHORTFORM_START_PROTOCOL.md
  ULTRA_LONGFORM.md
  VOLUME_001_LAUNCH_PROTOCOL.md
  VOLUME_HANDOFF_REENTRY_PROTOCOL.md
  VOICE_CONTRACT.md
  VOLUME_CLOSE_CHECKLIST.md
  WORLD_SEED_CONTRACT.md
  WORKSPACE_BLUEPRINT.md
  templates/
    archive/
    arc/
    architecture/
    canon/
    checkpoint/
    object_agent/
    pulse/
    reader/
    scene/
    subtext/
    thread/
    timeline/
    traction/

01_world/
  architecture/
    act-map.md
    chapter-map.md
    ending-lock.md
    early-payoff-schedule.md
    opening-10-blueprint.md
    opening-promise.md
    pov-map.md
    resonance-map.md
    series-bible.md
    storyline-weave.md
    volume-handoff-reentry.md
    volume-map.md
    world-seed.md
  arcs/
    character-state-arc.md
    foreshadow-payoff-arc.md
    relationship-arc.md
    thematic-compass.md
    world-conflict-arc.md
  canon/
    canon-ratification-ledger.md
    canon-laws.md
    continuity-watchlist.md
    taboo-registry.md
  checkpoints/
    README.md
  indexes/
    character-index.md
    index.md
    log.md
    object-index.md
    thread-dashboard.md
  objects/
    characters/
      README.md
    forces/
      README.md
    items/
      README.md
    locations/
      README.md
  pulse/
    emotional-pulse.md
  reader/
    misreading-design.md
    reader-desire-state.md
    reader-memory-model.md
  scenes/
    README.md
  subtext/
    subtext-registry.md
  threads/
    plot-thread-ledger.md
  timeline/
    master-timeline.md
  traction/
    traction-log.md

02_sources/
  README.md

03_manuscript/
  README.md
```

---

## 5. Operating documents in `00_system/`

Required system documents:

- `SCHEMA.md`
- `MASTER_AGENT.md`
- `ULTRA_LONGFORM.md`
- `AUTHORITY_MATRIX.md`
- `SOURCE_INGEST_PROTOCOL.md`
- `VOICE_CONTRACT.md`
- `STRUCTURAL_REINFORCEMENT.md`
- `NEW_STORY_BOOTSTRAP.md`
- `CHAPTER_BUILD_CHECKLIST.md`
- `ACT_CLOSE_CHECKLIST.md`
- `VOLUME_CLOSE_CHECKLIST.md`
- `CONTINUITY_AUDIT_CHECKLIST.md`
- `START_READINESS_GATE.md`
- `VOLUME_001_LAUNCH_PROTOCOL.md`
- `SERIES_START_PROTOCOL.md`
- `PREWRITE_SIMULATION_TEST.md`
- `SYSTEM_SMOKE_AUDIT.md`
- `CANON_CONTAMINATION_FIREWALL.md`
- `CANON_RATIFICATION_PROTOCOL.md`
- `CHAPTER_PACKET_PROTOCOL.md`
- `PRE_CHAPTER_SYNC_GATE.md`
- `CHAPTER_EXTENSION_GATE.md`
- `CHAPTER_ACCEPTANCE_GATE.md`
- `BOARD_FRESHNESS_AUDIT.md`
- `COMPLEXITY_BUDGET.md`
- `FAILURE_RECOVERY_RULES.md`
- `GOLDEN_EXECUTION_FIXTURE.md`
- `LONGFORM_EXPANSION_PROTOCOL.md`
- `ROLE_MODES.md`
- `PRODUCTION_REWRITE_MODE.md`
- `STRUCTURE_DONE_DEFINITION.md`
- `SHORTFORM_START_PROTOCOL.md`
- `VOLUME_HANDOFF_REENTRY_PROTOCOL.md`
- `WORLD_SEED_CONTRACT.md`
- `WORKSPACE_BLUEPRINT.md`

These files define how the workspace behaves.

---

## 6. Live world layer in `01_world/`

### `objects/`

One folder per story-bearing object.

Minimum object contract:

- `entity.md`
- `agent.md`
- `state.md`
- `links.md`
- `hooks.md`

Optional extensions:

- `evolution.md`
- `thematic-role.md`

### `scenes/`

One folder per scene or scene bundle.

Minimum scene contract:

- `brief.md`
- `cast.md`
- `draft.md`
- `aftermath.md`

Optional extension:

- `emotion-map.md`

### `arcs/`

Long-range story change boards.

### `architecture/`

Future-facing structure boards.

Also includes launch-stage boards such as:

- `world-seed.md`
- `opening-promise.md`
- `ending-lock.md`
- `opening-10-blueprint.md`
- `early-payoff-schedule.md`
- `volume-handoff-reentry.md`

### `threads/`

Open obligations and unresolved promises.

### `timeline/`

Chronology truth.

### `pulse/`

Emotional rhythm.

### `reader/`

Reader memory and controlled misreading.

Launch-stage reader pressure may also be tracked in:

- `reader-desire-state.md`

### `subtext/`

Surface/underlayer meaning.

### `traction/`

Page-turn and volume-turn force.

### `canon/`

Stable rules and contradiction watch.

Optional expansion:

- `taboo-registry.md`
- `canon-ratification-ledger.md`

### `checkpoints/`

Frozen summaries of canon.

### `indexes/`

Navigation and dashboard views.

---

## 7. Authority

The workspace uses:

- a hierarchy
- a matrix

Hierarchy:

1. `checkpoints/`
2. `canon/`
3. `timeline/`
4. `objects/`
5. `scenes/`
6. `arcs/`
7. `threads/`
8. `pulse/`
9. `reader/`
10. `subtext/`
11. `traction/`
12. `architecture/`
13. `manuscript/`

Matrix:

Use `00_system/AUTHORITY_MATRIX.md` when a question mixes multiple truth types.

---

## 8. Cadence

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
- audit canon, resonance, and output sync

---

## 9. Reconstruction order

1. create root folders
2. create system documents
3. create template families
4. create `01_world/` subdirectories
5. create object category folders
6. create base board files
7. create dashboard files
8. create intake and manuscript READMEs
9. create launch-ready boards such as `world-seed.md`, `opening-promise.md`, `ending-lock.md`, and `reader-desire-state.md`
10. create objects, scenes, checkpoints only when a new story actually starts

---

## 10. Structure-only reset rule

If a completed story begins to interfere with architecture work:

- remove story-specific object folders
- remove story-specific scene folders
- remove story-specific checkpoints
- remove compiled manuscript files
- reset live world boards to generic scaffold state
- preserve any root-front `000_*.md` durable note that carries stop-state, rollback, or reopen instructions
- keep system rules and templates intact

This workspace is currently in that reset state.

---

## 11. Disposable clone archival rule

- A disposable clone may hold a fully finished manuscript while remaining non-canonical to the reusable engine.
- When a clone reaches a meaningful stop state, create one root-front durable note from `templates/archive/root-durable-note.md`.
- That note should carry the stop state, useful artifact trail, intentional rollbacks, and first-read order for the next agent.
- Treat the files as the durable memory of the clone. Do not assume branch names, commit hashes, or checkout survival will preserve the meaning.
- If work is moving from manuscript-close into outward packaging, start from copied frozen files in a fresh workspace or explicit packaging branch.

---

## 12. Final summary

To reproduce the current system correctly, remember this:

- system docs define the operating law
- templates define repeatable file contracts
- live world boards define the active runtime structure
- no story is loaded until new objects, scenes, and checkpoints are created
