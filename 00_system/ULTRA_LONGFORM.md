# Ultra-Long-Form Operations

This document upgrades the workspace from a scene-and-object system into a system that can support very long fiction.

## Core principle

Long fiction collapses when the agent tries to remember too much in its head.

This system avoids collapse by splitting story truth into layers:

1. `objects/`: who and what exists
2. `scenes/`: what happened locally
3. `arcs/`: what is changing over long distances
4. `threads/`: what promises are still open
5. `timeline/`: when everything happened
6. `architecture/`: what the future is currently supposed to look like
7. `canon/`: what rules cannot be violated
8. `checkpoints/`: what parts of the past are now frozen

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

## Mandatory boards for scale

When the project grows beyond short fiction, maintain at least:

- `series-bible.md`
- `volume-map.md`
- `act-map.md`
- `chapter-map.md`
- `plot-thread-ledger.md`
- `master-timeline.md`
- `continuity-watchlist.md`

## Chapter workflow

Before writing a new chapter:

1. Read the relevant chapter entry in `chapter-map.md`.
2. Read the latest related object states.
3. Read relevant arc boards.
4. Read active thread entries that the chapter touches.
5. Read the master timeline.
6. Read the latest checkpoint if the story is already large.

After writing a new chapter:

1. Save the chapter's scenes.
2. Update affected object folders.
3. Update affected arcs.
4. Update plot-thread ledger.
5. Update master timeline.
6. Update chapter status in `chapter-map.md`.
7. Update continuity watchlist if any risk appeared.

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

## Planning rule

Architecture boards are allowed to change.
Checkpointed past is not.

When future plans change, revise:

- series / volume / act / chapter maps
- thread targets
- timeline of future material if needed

Do not silently revise already-written canon to make the plan look cleaner.

## Why this works

The system stays stable because each board answers a different question:

- object: what is this thing now
- scene: what happened here
- arc: how is the story transforming
- thread: what still needs payoff
- timeline: when did it happen
- architecture: where are we trying to go
- canon: what may never be broken
- checkpoint: what is now frozen
