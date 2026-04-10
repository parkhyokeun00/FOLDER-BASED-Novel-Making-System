# Ultra-Long-Form Operations

This document upgrades the workspace from a scene-and-object system into a system that can support multi-volume fiction without continuity collapse or reader drift.

## Core principle

Long fiction collapses when the agent tries to remember too much in its head, and long series lose readers when the system tracks facts but not traction.

This system avoids both failures by splitting story truth into layers.

## Truth layers

1. `objects/`: who and what exists now
2. `scenes/`: what happened locally
3. `arcs/`: what is changing over long distances
4. `threads/`: what promises are still open
5. `timeline/`: when everything happened
6. `pulse/`: how the emotional rhythm is beating
7. `reader/`: what the reader remembers, wants, fears, or misreads
8. `subtext/`: what is meant but not said
9. `traction/`: why the next chapter or volume must be opened
10. `architecture/`: what the future is currently supposed to look like
11. `canon/`: what rules cannot be violated
12. `checkpoints/`: what parts of the past are now frozen
13. `manuscript/`: reader-facing compiled output

## Scale model

- `Series`: the whole work across multiple books or major parts
- `Volume`: one large movement with its own start, middle, and end
- `Act`: a major pressure block inside a volume
- `Chapter`: the smallest default planning unit for sustained drafting
- `Scene`: the smallest default event unit
- `Beat`: optional micro-step inside a scene

## Operating rule

Never jump directly from "big vision" to "scene" in a very large work.
Always keep the middle layers alive:

- volume
- act
- chapter
- thread
- timeline
- reader state

## Mandatory boards for scale

When the project grows beyond short fiction, maintain at least:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `pov-map.md`
- `plot-thread-ledger.md`
- `master-timeline.md`
- `continuity-watchlist.md`
- `emotional-pulse.md`
- `reader-memory-model.md`
- `traction-log.md`

For true ultra-long form, also maintain:

- `misreading-design.md`
- `thematic-compass.md`
- `resonance-map.md`
- `storyline-weave.md`
- `subtext-registry.md`
- `canon-ratification-ledger.md`
- `volume-handoff-reentry.md`

## Cadence model

The system runs on layered closure, not constant full maintenance.

### Scene-close

- save scene files
- write `aftermath.md`
- update local object state and hooks
- update immediate timeline truth
- write `emotion-map.md` if scene-level emotion tracking is active

### Chapter-close

- update arcs
- update threads
- update `chapter-map.md`
- update `emotional-pulse.md`
- update reader memory or misreading state when needed
- record traction
- update `continuity-watchlist.md` if risk appeared

### Act-close

- create a checkpoint
- review due threads
- review arc movement and pacing drift
- review whether act promises were actually answered

### Volume-close

- create a checkpoint
- audit canon and continuity
- audit theme and resonance
- sync manuscript outputs
- define carryover conditions for the next volume

## Chapter workflow

Before writing a new chapter:

1. Read the relevant entry in `chapter-map.md`.
2. Read the relevant `pov-map.md` entry.
3. Read the latest related object states.
4. Read relevant arc boards.
5. Read active and due thread entries.
6. Read the master timeline.
7. Read relevant reader-memory and traction entries.
8. Read the latest checkpoint if the story is already large.

After writing a new chapter:

1. Save the chapter's scenes.
2. Write or revise each scene aftermath.
3. Update affected object folders.
4. Update affected arcs.
5. Update plot-thread ledger.
6. Update master timeline.
7. Update emotional pulse.
8. Update reader state if needed.
9. Update chapter status in `chapter-map.md`.
10. Update continuity watchlist if any risk appeared.
11. Record closing traction.

## Checkpoint workflow

Create a checkpoint when:

- an act ends
- a volume ends
- the status quo breaks permanently
- a major reveal changes how earlier material must be interpreted

Each checkpoint should summarize:

- locked plot facts
- current object states
- current arc positions
- active and resolved threads
- chronology up to the cutoff
- contradictions avoided or still risky
- handoff conditions to the next act or volume

## Scene storage transition rule

Flat scene storage is allowed for a pilot.

Recommended transition:

- volume 001 pilot: flat allowed
- by volume 002: partition by volume
- by multi-volume scale: partition by volume and act
- by heavy chapter counts: add chapter folders beneath act folders

Do not postpone this too long.
Late migrations are messier than early discipline.

## Reader retention rule

Continuity alone does not keep a reader.

At chapter and volume scale, the system must also ask:

- what does the reader want right now
- what does the reader fear right now
- what is the reader likely misunderstanding
- why is the next page necessary
- why is the next volume necessary

If those questions are not answered anywhere in the boards, the structure is stable but the series is at risk.

## Voice rule

Very long fiction drifts stylistically even when its plot remains coherent.

Use `00_system/VOICE_CONTRACT.md` to preserve:

- sentence temperature
- sensory emphasis
- POV-specific prose variation
- volume-to-volume voice drift

## Source pipeline rule

Ultra-long fiction needs more than canon protection.
It also needs an intake pipeline for research and raw inspiration.

Use `00_system/SOURCE_INGEST_PROTOCOL.md` and keep `02_sources/` structured enough to distinguish:

- unprocessed material
- interpreted material
- canon-integrated claims
- discarded or deprecated claims

## Start gate rule

Do not begin a real ultra-long story because the structure feels impressive.

Before drafting starts:

- pass `START_READINESS_GATE.md`
- run `PREWRITE_SIMULATION_TEST.md`
- complete `VOLUME_001_LAUNCH_PROTOCOL.md`
- confirm the design is done enough through `STRUCTURE_DONE_DEFINITION.md`

## Why this works

The system stays stable because each layer answers a different question, and it stays readable because traction, reader state, and emotional rhythm are tracked beside canon.
