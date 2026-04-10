# Workspace Blueprint

This document is a detailed reconstruction guide for the current workspace.

Its purpose is twofold:

1. Diagnose the current structure as a fiction operating system.
2. Preserve enough detail that the same structure can be rebuilt from an empty folder without guessing.

---

## 1. Executive diagnosis

### What is already strong

- The workspace clearly separates local entity truth, scene truth, long-range narrative truth, planning truth, chronology truth, and frozen canon.
- The object model is strong enough for both concrete entities and abstract forces.
- The structure already supports short fiction, long-form fiction, and ultra-long-form serialization without changing the core philosophy.
- Arc boards, thread ledgers, and timeline boards reduce drift that usually destroys long projects.
- Checkpoints create frozen summaries, which is the most important anti-retcon mechanism in large fiction systems.

### What is still structurally risky

- `01_world/scenes/` is currently flat. This is acceptable for a pilot and small novels, but a true ultra-long serial should eventually partition scenes by volume and act.
- `01_world/objects/` is global. This is correct as a canon layer, but very large projects will need disciplined indexing and naming to avoid object sprawl.
- `02_sources/` exists, but the current pilot does not yet define a detailed per-source ingest protocol with provenance metadata.
- The system is excellent at preserving continuity, but it still depends on disciplined updates. If boards are not updated after each major chapter, drift can still happen.

### Overall verdict

The structure is already good enough to support ultra-long fiction in principle.

It is not "fragile".
Its main remaining risk is operational discipline at scale, not missing architecture.

---

## 2. Core design philosophy

This workspace is not a normal notes folder.
It is a layered story operating system.

Each layer answers a different question:

- `objects/`: what exists
- `scenes/`: what happened locally
- `arcs/`: what is changing over long distances
- `architecture/`: what the future is currently supposed to look like
- `threads/`: what promises are still open
- `timeline/`: when things happened
- `canon/`: what may not be broken
- `checkpoints/`: what part of the past is now frozen
- `manuscript/`: what the reader-facing output currently is

This separation is the reason the system can scale.

---

## 3. Root directory model

The current root contains four main top-level directories and one root overview file.

### Root files and folders

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
  This is where the rules, contracts, templates, and reconstruction logic live.

- `01_world/`
  The active story world.
  This is where objects, scenes, arcs, plans, threads, and canon boards live.

- `02_sources/`
  Immutable or semi-immutable raw materials.
  These are not the story world itself.
  They are inputs to be interpreted and integrated.

- `03_manuscript/`
  Output-facing draft zone.
  This is where compiled human-readable manuscripts live.

---

## 4. Exact current tree

The following tree represents the current structure at the time this blueprint was written.

```text
README.md
00_system/
  MASTER_AGENT.md
  SCHEMA.md
  ULTRA_LONGFORM.md
  WORKSPACE_BLUEPRINT.md
  templates/
    arc/
      character-state-arc.md
      relationship-arc.md
      world-conflict-arc.md
      foreshadow-payoff-arc.md
    architecture/
      series-bible.md
      volume-map.md
      act-map.md
      chapter-map.md
      pov-map.md
    canon/
      canon-laws.md
      continuity-watchlist.md
    checkpoint/
      canon-snapshot.md
    object_agent/
      entity.md
      agent.md
      state.md
      links.md
      hooks.md
    scene/
      brief.md
      cast.md
      draft.md
      aftermath.md
    thread/
      plot-thread-ledger.md
    timeline/
      master-timeline.md

01_world/
  architecture/
    series-bible.md
    volume-map.md
    act-map.md
    chapter-map.md
    pov-map.md
  arcs/
    character-state-arc.md
    relationship-arc.md
    world-conflict-arc.md
    foreshadow-payoff-arc.md
  canon/
    canon-laws.md
    continuity-watchlist.md
  checkpoints/
    README.md
    checkpoint-001-end-of-volume-001.md
  indexes/
    index.md
    log.md
  objects/
    characters/
      namju/
      sumin/
      fake-artist/
    forces/
      poverty/
      guilt/
      sunset/
    items/
      ghost-paintings/
    locations/
      atelier-room/
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
  threads/
    plot-thread-ledger.md
  timeline/
    master-timeline.md

02_sources/

03_manuscript/
  README.md
  노을 아래, 끝내.md
```

---

## 5. Layer-by-layer contract

### 5.1 `00_system/`

This directory defines how the workspace works.

#### Required operating documents

- `MASTER_AGENT.md`
  Defines the role of the orchestration agent.

- `SCHEMA.md`
  Defines the file contracts and authority model.

- `ULTRA_LONGFORM.md`
  Defines how to operate the system when the project becomes large.

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

These templates are the fastest way to recreate the system consistently.

### 5.2 `01_world/`

This directory contains live story truth and live planning.

#### `objects/`

Stores one folder per story-bearing object.

Each object folder must contain:

- `entity.md`
- `agent.md`
- `state.md`
- `links.md`
- `hooks.md`

These five files are the minimum object contract.

#### `scenes/`

Stores one folder per scene or scene bundle.

Each scene folder must contain:

- `brief.md`
- `cast.md`
- `draft.md`
- `aftermath.md`

These four files are the minimum scene contract.

#### `arcs/`

Stores long-range transformation boards.

Current required boards:

- `character-state-arc.md`
- `relationship-arc.md`
- `world-conflict-arc.md`
- `foreshadow-payoff-arc.md`

#### `architecture/`

Stores intended future structure.

Current required boards:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `pov-map.md`

#### `threads/`

Stores unresolved obligations.

Current required board:

- `plot-thread-ledger.md`

#### `timeline/`

Stores chronology truth.

Current required board:

- `master-timeline.md`

#### `canon/`

Stores stable rules and contradiction watch.

Current required boards:

- `canon-laws.md`
- `continuity-watchlist.md`

#### `checkpoints/`

Stores frozen summaries.

Each checkpoint is a snapshot of canon up to a boundary and should not be casually rewritten.

#### `indexes/`

Stores high-level navigation and chronological change history.

Current required files:

- `index.md`
- `log.md`

### 5.3 `02_sources/`

This directory is intentionally raw.
It is the intake layer, not the interpreted story layer.

Recommended future subfolders:

- `articles/`
- `notes/`
- `images/`
- `research/`
- `interviews/`
- `fragments/`

### 5.4 `03_manuscript/`

This directory contains output-facing drafts.

Current contract:

- `README.md` explains what manuscript lives here
- one or more compiled draft files live beside it

---

## 6. Authority hierarchy

This is the most important rule in the whole system.

Do not let two files claim the same kind of truth.

### Current authority order

1. `checkpoints/`
   Frozen canon before the cutoff.

2. `canon/`
   Stable world laws and continuity warnings.

3. `timeline/`
   Chronological truth.

4. `objects/`
   Current truth for specific entities.

5. `scenes/`
   Local event truth and aftermath.

6. `arcs/`
   Long-range interpretation of change.

7. `threads/`
   Open obligations and unresolved promises.

8. `architecture/`
   Future plan, revisable.

9. `manuscript/`
   Reader-facing compilation, derived from lower layers.

### Important distinction

- `architecture/` may change.
- `checkpoint/` may not casually change.

This single distinction is what prevents ultra-long projects from dissolving into silent retcons.

---

## 7. Reconstruction order from an empty folder

To recreate the current system without guessing, follow this order.

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

```text
MASTER_AGENT.md
SCHEMA.md
ULTRA_LONGFORM.md
```

### Step 3. Create all template families

Inside `00_system/templates/`, create:

```text
arc/
architecture/
canon/
checkpoint/
object_agent/
scene/
thread/
timeline/
```

Then create the current template files exactly as listed in the tree above.

### Step 4. Create live world subdirectories

Inside `01_world/`, create:

```text
architecture/
arcs/
canon/
checkpoints/
indexes/
objects/
scenes/
threads/
timeline/
```

### Step 5. Create object categories

Inside `01_world/objects/`, create:

```text
characters/
locations/
items/
forces/
```

### Step 6. Create base navigation files

Create:

- `01_world/indexes/index.md`
- `01_world/indexes/log.md`

### Step 7. Create arc boards

Create:

- `01_world/arcs/character-state-arc.md`
- `01_world/arcs/relationship-arc.md`
- `01_world/arcs/world-conflict-arc.md`
- `01_world/arcs/foreshadow-payoff-arc.md`

### Step 8. Create architecture boards

Create:

- `01_world/architecture/series-bible.md`
- `01_world/architecture/volume-map.md`
- `01_world/architecture/act-map.md`
- `01_world/architecture/chapter-map.md`
- `01_world/architecture/pov-map.md`

### Step 9. Create thread, timeline, canon, checkpoint base files

Create:

- `01_world/threads/plot-thread-ledger.md`
- `01_world/timeline/master-timeline.md`
- `01_world/canon/canon-laws.md`
- `01_world/canon/continuity-watchlist.md`
- `01_world/checkpoints/README.md`

### Step 10. Create object folders

For each live object, create a folder in its category and place:

- `entity.md`
- `agent.md`
- `state.md`
- `links.md`
- `hooks.md`

### Step 11. Create scene folders

For each scene, create a folder and place:

- `brief.md`
- `cast.md`
- `draft.md`
- `aftermath.md`

### Step 12. Create manuscript layer

Create:

- `03_manuscript/README.md`
- one or more compiled manuscripts

### Step 13. Freeze finished boundaries

When the first fully coherent unit is done, create:

- a checkpoint in `01_world/checkpoints/`

This is mandatory if the project is going to grow.

---

## 8. Naming rules

### Objects

Use lowercase and hyphen-separated folder names.

Examples:

- `namju`
- `fake-artist`
- `atelier-room`
- `ghost-paintings`
- `ash-rain`

### Scenes

Use explicit numeric prefixes when ordering matters.

Current pattern:

- `scene-001-room-at-dusk`
- `scene-002-gallery-visit`

### Chapters

Use:

- `chapter-001`
- `chapter-002`

### Volumes

Use:

- `volume-001`
- `volume-002`

### Checkpoints

Use:

- `checkpoint-001-end-of-volume-001`
- `checkpoint-002-end-of-act-02`

---

## 9. Operating procedure after writing a scene

This is the current mandatory update order.

1. Write or revise the scene folder.
2. Update affected object `state.md`, `links.md`, and `hooks.md`.
3. Update relevant arc boards.
4. Update the thread ledger if an obligation opened, advanced, or resolved.
5. Update the master timeline if chronology was locked.
6. Update chapter or act planning boards if the plan drifted.
7. Update `index.md` if navigation changed.
8. Append a new entry to `log.md`.
9. If a major boundary was crossed, create or revise a checkpoint.

This order matters because it keeps local truth, long-range truth, and future plan aligned.

---

## 10. What makes the current structure scalable

### Reason 1. It treats abstract forces like objects

`poverty`, `guilt`, and `sunset` can be tracked like entities.
This is unusually powerful for literary fiction, gothic fiction, psychological fiction, and dark fantasy.

### Reason 2. It separates scene truth from future planning

Most story systems collapse because the plan and the canon blur together.
This one separates them cleanly.

### Reason 3. It freezes past boundaries

Checkpoints stop silent rewriting.

### Reason 4. It keeps multiple long-range views alive

No single board has to do everything.

- arcs track transformation
- threads track obligations
- timeline tracks chronology
- architecture tracks future shape

That division is what makes scale possible.

---

## 11. Structural review findings

These are review findings, not fatal flaws.

### Finding 1: flat scene storage will eventually strain navigation

Current structure stores all scene folders directly under `01_world/scenes/`.
This is fine now, but once the project reaches hundreds of scenes, the directory will become heavy to navigate and easy to misuse.

Recommended future rule:

- for pilot and small novels: keep flat
- for larger novels: partition by volume
- for ultra-long serials: partition by volume and act

Example future shape:

```text
01_world/scenes/
  volume-001/
    act-01/
      scene-001-...
    act-02/
      scene-...
  volume-002/
    act-01/
      scene-...
```

This is not required yet, but it is the first scale pressure to watch.

### Finding 2: source ingestion is still under-specified

`02_sources/` exists, but the current workspace does not yet define a full source contract such as:

- required metadata
- ingest log entry format
- provenance links back into world objects
- source status such as raw / ingested / deprecated

This matters once the system starts absorbing lots of research material.

### Finding 3: operational discipline remains a dependency

The architecture is strong, but it still depends on updating boards after important scenes and chapters.
If the team stops updating arcs, threads, or timeline, continuity drift can still reappear.

This is not a structural defect.
It is a maintenance requirement.

---

## 12. Recommended next hardening steps

These are not required to preserve the current structure, but they are the logical next layer.

### Hardening step A

Add a formal source-ingest contract for `02_sources/`.

### Hardening step B

Introduce volume/act subfolders under `01_world/scenes/` once scene count becomes large.

### Hardening step C

Create reusable "chapter build checklist" and "volume close checklist" documents under `00_system/`.

### Hardening step D

Add a per-object metadata index once object count becomes high.

---

## 13. Minimum viable reproduction checklist

If someone wants to recreate the structure fast, this is the minimal checklist.

- Create root folders.
- Create `00_system/` contracts.
- Create all template families.
- Create `01_world/` live subdirectories.
- Create indexes.
- Create arc boards.
- Create architecture boards.
- Create thread, timeline, canon, and checkpoint files.
- Create object category folders.
- Create at least one object folder using the 5-file contract.
- Create at least one scene folder using the 4-file contract.
- Create one manuscript output file.
- Freeze at least one checkpoint once a coherent unit is finished.

If all of the above exists, the system is alive.

---

## 14. Current pilot-specific content

The current workspace is not empty.
It already contains a fully built pilot tragedy.

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

### Current pilot frozen checkpoint

- `checkpoint-001-end-of-volume-001.md`

This means the workspace is not merely prepared.
It is already tested by a complete end-to-end story cycle.

---

## 15. Final summary

To reproduce the current system correctly, remember this:

- objects are not scenes
- scenes are not arcs
- arcs are not plans
- plans are not canon
- canon is not output
- checkpoints freeze the past

If those distinctions remain intact, the structure can survive very large fiction.
