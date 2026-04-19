# Failure Recovery Rules

Use this when the system starts drifting during active drafting.

## Common failure modes

- stale boards
- canon contamination
- subplot disappearance
- opening drift
- reader desire collapse
- overgrown structure with unwritable chapters
- parallel-pass status mismatch

## Recovery order

1. stop adding new design layers
2. identify the smallest broken contract
3. if multiple workers or agents touched the pass, compare landed files with `git diff --name-only` or `git status --short` before trusting any status summary
4. repair source-of-truth boards first
5. repair chapter and traction logic second
6. only then resume drafting

## Never recover by

- silently retconning frozen truth
- inventing a new board to avoid a decision
- trusting narrative status reports over landed file state after parallel work
- continuing to draft while a core contradiction is unresolved
