# Authority Matrix

The hierarchy in `SCHEMA.md` tells you which layers outrank others.
This matrix tells you which file family should answer which question first.

## Query-first authority

| Question type | Primary source | Secondary source | Notes |
|---|---|---|---|
| What is true about a specific entity right now? | `01_world/objects/` | latest relevant `01_world/scenes/*/aftermath.md` | Objects hold current local truth. |
| Did this event happen? | `01_world/scenes/` | `01_world/timeline/` | Scene truth outranks interpretation. |
| In what order did events happen? | `01_world/timeline/` | relevant scenes, checkpoints | Timeline holds chronological truth. |
| What is changing over long distance? | `01_world/arcs/` | checkpoints, chapter-map | Arcs interpret direction, not raw event fact. |
| What promises are still open? | `01_world/threads/` | scenes, traction | Threads hold unresolved obligations. |
| What does the reader remember, fear, or misread? | `01_world/reader/` | traction, subtext | Reader state is its own layer. |
| What is really being said beneath the surface? | `01_world/subtext/` | scenes, thematic-compass | Subtext is interpretive but deliberate. |
| Why should the next page or volume be opened? | `01_world/traction/` | chapter-map, reader | Traction records the active pull device. |
| What is the emotional rhythm doing? | `01_world/pulse/` | scene emotion maps | Pulse tracks sequence-level feeling. |
| What rules may not be broken? | `01_world/canon/` | checkpoints | Canon holds live law; checkpoints hold frozen past summaries. |
| What is already frozen about the past? | `01_world/checkpoints/` | canon, timeline | Checkpoints outrank future plans. |
| What is the future currently intended to be? | `01_world/architecture/` | traction, threads | Architecture is revisable intent, not canon. |
| What does the reader-facing draft currently say? | `03_manuscript/` | scenes and checkpoints | Manuscript is output, not planning truth. |

## Conflict rules

- If `architecture/` conflicts with `checkpoints/`, the checkpoint wins.
- If `arcs/` conflict with explicit scene fact, the scene wins and the arc must be revised.
- If `objects/` conflict with a later canonical scene aftermath, update the object.
- If `reader/` conflicts with author memory, trust the reader board when planning reminders.
- If `manuscript/` drifts from canonical lower layers, either revise the manuscript or record the divergence explicitly.

## Practical use

When a question mixes multiple truth types, answer them in order:

1. identify the query type
2. consult the primary layer
3. confirm against the secondary layer
4. if conflict remains, escalate to `checkpoints/` and `canon/`

Do not solve authority conflicts by intuition alone.
