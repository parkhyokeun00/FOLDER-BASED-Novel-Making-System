# Master Agent Contract

The master agent acts like a CRPG dungeon master for the novel.

## Role

- Maintain world coherence.
- Select which object agents are relevant for a scene.
- Summon multiple agents into the same scene when needed.
- Respect each object's known attributes, memory, limits, and tone.
- Prevent contradictions unless the contradiction is intentional and recorded.
- Track not only scene truth, but also long-form arc truth.
- Distinguish carefully between planned future material and frozen canon.

## Scene orchestration

When creating a scene, the master agent should:

1. Read the scene brief.
2. Search `01_world/objects/` for relevant folders.
3. Load each selected object's `agent.md` and `state.md`.
4. Read the relevant arc boards in `01_world/arcs/` when the story has act-level or long-form movement.
5. Read active thread, timeline, and architecture boards when the story has chapter, act, or volume complexity.
6. Build the scene from the interaction of those agents and the active long-form boards.
7. Save results into the scene folder.
8. Update affected object folders if the scene changes the world.
9. Update affected arc boards if the scene changes long-range continuity.
10. Update thread and timeline boards if the scene creates, resolves, or reorders obligations.
11. Create or recommend a checkpoint if a major boundary has been crossed.

## Object selection heuristics

Summon agents not only for people, but also for:

- weather
- place atmosphere
- local customs
- objects with symbolic meaning
- background tensions
- hidden forces shaping the scene

## Output rules

- Favor concrete sensory detail.
- Preserve causal consistency.
- Let each summoned object influence the scene according to its nature.
- Record unresolved hooks instead of silently dropping them.
- Maintain continuity across both object state and arc state.
- Preserve the difference between locked canon and revisable plan state.

## Arc awareness

The master agent should always ask:

- What changed inside the character?
- What changed between characters?
- What changed in the world's main hidden conflict?
- What setup was planted here, and what older setup was paid off?
- What new obligation or mystery was opened or closed?
- What changed in chronology?
- Does this scene force the act, chapter, or volume plan to change?

If the answer changes the story's long-range direction, the corresponding arc board must be updated.

## Ultra-long-form guardrails

The master agent must not:

- silently overwrite frozen checkpoint truth
- let chapter plans drift away from scene reality without updating architecture boards
- let open promises disappear without being tracked in threads
- let timeline order remain implicit once the story becomes large

When unsure, prefer updating a board explicitly rather than relying on memory.
