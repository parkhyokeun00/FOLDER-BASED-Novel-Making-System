# Workspace Blueprint

This document is the detailed reconstruction guide for the current workspace.

Its purpose is twofold:

1. diagnose the current structure as a fiction operating system
2. preserve enough detail that the same structure can be rebuilt from an empty folder without guessing

---

## 1. Executive diagnosis

### What is already strong

- The workspace separates object truth, scene truth, long-range change, open obligations, chronology, reader state, traction, canon, and frozen history.
- The object model is strong enough for both concrete entities and abstract forces.
- The system now supports not only continuity preservation, but also emotional rhythm, reader memory, subtext, and page-turn pull.
- Checkpoints create frozen summaries, which remain the main anti-retcon mechanism.
- `aftermath.md` is now the official update hub, reducing duplicated maintenance labor.

### What still requires discipline

- `01_world/scenes/` is still flat for the pilot. This is acceptable now, but `volume-002` should trigger a directory split.
- `02_sources/` now has a protocol, but it still depends on actual use to stay clean.
- Reader, pulse, subtext, and traction layers only help if they are kept current.
- Dashboards reduce friction, but they do not remove the need for chapter-close and volume-close review.

### Overall verdict

The structure is now good enough to support:

- short fiction
- long-form fiction
- ultra-long serialization

Its main remaining risk is no longer missing architecture.
It is the human or agent habit of skipping updates.

---

## 2. Core design philosophy

This workspace is not a normal notes folder.
It is a layered story operating system.

Each layer answers a different question:

- `objects/`: what exists now
- `scenes/`: what happened locally
- `arcs/`: what is changing over long distances
- `threads/`: what promises are still open
- `timeline/`: when things happened
- `pulse/`: what the emotional rhythm is doing
- `reader/`: what the reader remembers, wants, fears, or misreads
- `subtext/`: what is being said underneath what is spoken
- `traction/`: why the reader continues
- `architecture/`: what the future is currently supposed to look like
- `canon/`: what may not be broken
- `checkpoints/`: what part of the past is now frozen
- `manuscript/`: what the reader-facing output currently is

This separation is the reason the system can scale.

---

## 3. Root directory model

The root contains four main top-level directories and one root overview file.

```text
README.md
00_system/
01_world/
02_sources/
03_manuscript/
```

### Meaning

- `README.md`
  Global orientation document.

- `00_system/`
  The operating system.
  Rules, contracts, templates, and reconstruction logic live here.

- `01_world/`
  The active story world.
  Objects, scenes, boards, canon, and checkpoints live here.

- `02_sources/`
  Intake layer.
  Raw material, research, fragments, mood boards, and voice notes live here.

- `03_manuscript/`
  Output layer.
  Reader-facing compiled drafts live here.

---

## 4. Exact current tree

The following tree represents the current structure after reinforcement.

```text
README.md
00_system/
  ACT_CLOSE_CHECKLIST.md
  AUTHORITY_MATRIX.md
  CHAPTER_BUILD_CHECKLIST.md
  CONTINUITY_AUDIT_CHECKLIST.md
  MASTER_AGENT.md
  SCHEMA.md
  SOURCE_INGEST_PROTOCOL.md
  STRUCTURAL_REINFORCEMENT.md
  ULTRA_LONGFORM.md
  VOICE_CONTRACT.md
  VOLUME_CLOSE_CHECKLIST.md
  WORKSPACE_BLUEPRINT.md
  templates/
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
    pov-map.md
    resonance-map.md
    series-bible.md
    storyline-weave.md
    volume-map.md
  arcs/
    character-state-arc.md
    foreshadow-payoff-arc.md
    relationship-arc.md
    thematic-compass.md
    world-conflict-arc.md
  canon/
    canon-laws.md
    continuity-watchlist.md
  checkpoints/
    README.md
    checkpoint-001-end-of-volume-001.md
  indexes/
    character-index.md
    index.md
    log.md
    object-index.md
    thread-dashboard.md
  objects/
    characters/
    forces/
    items/
    locations/
  pulse/
    emotional-pulse.md
  reader/
    misreading-design.md
    reader-memory-model.md
  scenes/
    story-core/
    scene-001-room-at-dusk/
    scene-002-gallery-visit/
    scene-003-sumin-alone/
    scene-004-the-price/
    scene-005-return-and-crack/
    scene-006-blood-on-wrist/
    scene-007-the-truth-breaks/
    scene-008-plan-to-kill/
    scene-009-failed-revenge/
    scene-010-sunset-fall/
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
  노을 아래, 끝내.md
```

---

## 5. Layer-by-layer contract

### 5.1 `00_system/`

This directory defines how the workspace works.

#### Required operating documents

- `SCHEMA.md`
  File contracts and cadence.

- `MASTER_AGENT.md`
  Orchestration, writer/editor pass, rejection and breathing-scene rules.

- `ULTRA_LONGFORM.md`
  Scale-aware operation manual.

- `AUTHORITY_MATRIX.md`
  Question-by-question truth resolution.

- `SOURCE_INGEST_PROTOCOL.md`
  Intake and provenance rules.

- `CHAPTER_BUILD_CHECKLIST.md`
- `ACT_CLOSE_CHECKLIST.md`
- `VOLUME_CLOSE_CHECKLIST.md`
- `CONTINUITY_AUDIT_CHECKLIST.md`
  Operational checklists.

- `VOICE_CONTRACT.md`
  Style continuity contract.

- `STRUCTURAL_REINFORCEMENT.md`
  Overlay rules for long and ultra-long work.

- `WORKSPACE_BLUEPRINT.md`
  This reconstruction guide.

#### Required template families

- `templates/object_agent/`
- `templates/scene/`
- `templates/arc/`
- `templates/architecture/`
- `templates/thread/`
- `templates/timeline/`
- `templates/canon/`
- `templates/checkpoint/`
- `templates/pulse/`
- `templates/reader/`
- `templates/subtext/`
- `templates/traction/`

### 5.2 `01_world/`

This directory contains live story truth and live planning.

#### `objects/`

Stores one folder per story-bearing object.

Minimum object contract:

- `entity.md`
- `agent.md`
- `state.md`
- `links.md`
- `hooks.md`

Advanced extensions:

- `evolution.md`
- `thematic-role.md`

#### `scenes/`

Stores one folder per scene or scene bundle.

Minimum scene contract:

- `brief.md`
- `cast.md`
- `draft.md`
- `aftermath.md`

Advanced extension:

- `emotion-map.md`

`aftermath.md` is the update hub.

#### `arcs/`

Stores long-range transformation boards.

Required:

- `character-state-arc.md`
- `relationship-arc.md`
- `world-conflict-arc.md`
- `foreshadow-payoff-arc.md`

Advanced:

- `thematic-compass.md`

#### `architecture/`

Stores intended future structure.

Required:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `pov-map.md`

Advanced:

- `resonance-map.md`
- `storyline-weave.md`

#### `threads/`

Stores unresolved obligations.

Required:

- `plot-thread-ledger.md`

#### `timeline/`

Stores chronology truth.

Required:

- `master-timeline.md`

#### `pulse/`

Stores emotional rhythm.

Required once the project moves beyond a short pilot:

- `emotional-pulse.md`

#### `reader/`

Stores reader-facing memory and controlled misunderstanding.

Required once the project depends on delayed payoff:

- `reader-memory-model.md`

Recommended:

- `misreading-design.md`

#### `subtext/`

Stores recurring hidden meaning patterns.

Recommended for long literary, psychological, or multi-volume work:

- `subtext-registry.md`

#### `traction/`

Stores why the next page or volume is necessary.

Recommended once chapters become the main drafting unit:

- `traction-log.md`

#### `canon/`

Stores stable rules and contradiction watch.

Required:

- `canon-laws.md`
- `continuity-watchlist.md`

#### `checkpoints/`

Stores frozen summaries.

Each checkpoint is a snapshot of canon up to a boundary and should not be casually rewritten.

#### `indexes/`

Stores navigation and dashboard views.

Required:

- `index.md`
- `log.md`

Recommended once scale increases:

- `object-index.md`
- `character-index.md`
- `thread-dashboard.md`

### 5.3 `02_sources/`

This directory is intake, not canon.

Recommended future subfolders:

- `raw/`
- `parsed/`
- `canon-integrated/`
- `deprecated/`
- `fragments/`
- `research/`
- `mood-boards/`
- `voice-notes/`

Follow `00_system/SOURCE_INGEST_PROTOCOL.md`.

### 5.4 `03_manuscript/`

This directory contains output-facing drafts.

Current contract:

- `README.md` explains what manuscript lives here
- one or more compiled draft files live beside it

---

## 6. Authority hierarchy and matrix

### Hierarchy

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

### Matrix

Use `00_system/AUTHORITY_MATRIX.md` when a question mixes multiple truth types.

Do not resolve mixed conflicts by intuition alone.

---

## 7. Operating cadence

### Scene-close

1. Write or revise the scene folder.
2. Write `aftermath.md`.
3. Update affected object state and hooks.
4. Update immediate timeline truth.
5. Update scene emotion map if used.

### Chapter-close

1. Update affected arc boards.
2. Update `plot-thread-ledger.md`.
3. Update `chapter-map.md`.
4. Update `emotional-pulse.md`.
5. Update `reader-memory-model.md` and `misreading-design.md` if needed.
6. Update `traction-log.md`.
7. Update `continuity-watchlist.md` if risk appeared.

### Act-close

1. Create a checkpoint.
2. Review due threads.
3. Review act-level arc movement.
4. Review planning drift.

### Volume-close

1. Create a checkpoint.
2. Review canon integrity.
3. Review theme and resonance.
4. Sync reader-facing manuscript output.

---

## 8. Reconstruction order from an empty folder

### Step 1. Create root

Create:

```text
README.md
00_system/
01_world/
02_sources/
03_manuscript/
```

### Step 2. Create system layer

Inside `00_system/`, create:

- `SCHEMA.md`
- `MASTER_AGENT.md`
- `ULTRA_LONGFORM.md`
- `AUTHORITY_MATRIX.md`
- `SOURCE_INGEST_PROTOCOL.md`
- `VOICE_CONTRACT.md`
- `STRUCTURAL_REINFORCEMENT.md`
- `CHAPTER_BUILD_CHECKLIST.md`
- `ACT_CLOSE_CHECKLIST.md`
- `VOLUME_CLOSE_CHECKLIST.md`
- `CONTINUITY_AUDIT_CHECKLIST.md`

### Step 3. Create all template families

Inside `00_system/templates/`, create:

- `arc/`
- `architecture/`
- `canon/`
- `checkpoint/`
- `object_agent/`
- `pulse/`
- `reader/`
- `scene/`
- `subtext/`
- `thread/`
- `timeline/`
- `traction/`

### Step 4. Create live world subdirectories

Inside `01_world/`, create:

- `architecture/`
- `arcs/`
- `canon/`
- `checkpoints/`
- `indexes/`
- `objects/`
- `pulse/`
- `reader/`
- `scenes/`
- `subtext/`
- `threads/`
- `timeline/`
- `traction/`

### Step 5. Create object categories

Inside `01_world/objects/`, create:

- `characters/`
- `locations/`
- `items/`
- `forces/`

### Step 6. Create base navigation and dashboard files

Create:

- `index.md`
- `log.md`
- `object-index.md`
- `character-index.md`
- `thread-dashboard.md`

### Step 7. Create core boards

Create:

- arc boards
- architecture boards
- thread ledger
- master timeline
- canon laws
- continuity watchlist
- pulse board
- reader boards
- traction board

### Step 8. Create object folders

For each live object, create the five-file minimum contract.

### Step 9. Create scene folders

For each scene, create the four-file minimum contract.
If scene-level emotion tracking is active, also add `emotion-map.md`.

### Step 10. Create manuscript layer

Create:

- `03_manuscript/README.md`
- one or more compiled manuscripts

### Step 11. Freeze finished boundaries

When the first coherent act or volume exists, create a checkpoint.

---

## 9. Scene partition policy

Use these thresholds:

- single pilot or single-volume draft: flat scenes allowed
- beginning of `volume-002`: partition by volume
- larger multi-volume work: partition by volume and act
- chapter-heavy work: add chapter folders beneath act folders

Do not wait until hundreds of scenes already exist.

---

## 10. Current pilot-specific content

The workspace is already tested by a complete pilot tragedy.

### Current pilot object set

- characters: `namju`, `sumin`, `fake-artist`
- location: `atelier-room`
- item: `ghost-paintings`
- forces: `poverty`, `guilt`, `sunset`

### Current pilot scene set

- `story-core`
- `scene-001-room-at-dusk`
- `scene-002-gallery-visit`
- `scene-003-sumin-alone`
- `scene-004-the-price`
- `scene-005-return-and-crack`
- `scene-006-blood-on-wrist`
- `scene-007-the-truth-breaks`
- `scene-008-plan-to-kill`
- `scene-009-failed-revenge`
- `scene-010-sunset-fall`

### Current pilot manuscript

- `03_manuscript/노을 아래, 끝내.md`

### Current frozen checkpoint

- `checkpoint-001-end-of-volume-001.md`

---

## 11. Final summary

To reproduce the current system correctly, remember this:

- objects are not scenes
- scenes are not arcs
- arcs are not plans
- plans are not canon
- canon is not output
- checkpoints freeze the past
- reader state is not author memory
- traction is not the same thing as thread count

If those distinctions remain intact, the structure can survive very large fiction.
