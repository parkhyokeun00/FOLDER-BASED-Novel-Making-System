# Source Ingest Protocol

`02_sources/` is not a dumping ground.
It is the intake layer for research, fragments, references, and raw inspiration.

## Purpose

Separate:

- raw material that has not been processed
- interpreted material that has been read and summarized
- canon-integrated claims that now affect the story system
- deprecated or rejected ideas that should remain searchable but not live

## Recommended source areas

- `02_sources/raw/`: untouched intake
- `02_sources/parsed/`: summarized or normalized material
- `02_sources/canon-integrated/`: source notes whose claims were adopted into the story system
- `02_sources/deprecated/`: superseded, rejected, or misleading material
- `02_sources/fragments/`: stray lines, images, motifs, ideas, or partial scenes worth saving
- `02_sources/research/`: factual investigation and references
- `02_sources/mood-boards/`: tone, atmosphere, and visual anchors
- `02_sources/voice-notes/`: direct author intuition, diary-like notes, or spoken discoveries

## Required metadata for a source note

Every source note should record:

- `source-id`
- `type`
- `status`
- `origin`
- `date`
- `trust-level`
- `linked-objects`
- `linked-scenes`
- `adopted-claims`
- `rejected-claims`
- `notes`

## Status vocabulary

- `raw`: captured but not interpreted
- `parsed`: read and summarized
- `canon-integrated`: claims from this source now affect world truth
- `deprecated`: intentionally set aside

## Ingest flow

1. Capture the material into `raw/`, `fragments/`, `research/`, `mood-boards/`, or `voice-notes/`.
2. Summarize or normalize it into `parsed/` if it has reusable value.
3. Decide what, if anything, enters the story system.
4. If a claim is adopted into canon, record it in `canon-integrated/` and propagate the change into the correct boards.
5. If the material is no longer trusted or useful, move or mirror it into `deprecated/`.

## Canon adoption rule

No source note changes canon by itself.

Canon changes only when its claims are explicitly adopted into:

- objects
- scenes
- arcs
- threads
- timeline
- canon
- checkpoints

## Creative intake rule

Fragments, mood boards, and voice notes are valid sources even if they are not factual.
Treat them as inspiration inputs, not factual authorities.

## Provenance rule

When a source materially changes the story system, record the destination in the source note and record the source in the affected downstream note when useful.

## Chapter re-entry rule

If a chapter depends on source-derived material, reopen the relevant parsed or canon-integrated notes before drafting.

The chapter packet should record the reference set actually used.
