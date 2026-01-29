# Create Codebase Context

## Purpose
Build a high-fidelity internal model of the codebase before making changes. This prompt is explicitly for context-building, not editing.

## Phase separation (critical)
- Current role: context builder.
- Future role: decision-making and implementation.
- Treat these as separate phases.

## Key mental constraint
Anything you do not explicitly understand now is a future risk. If something is unclear, fragile, or implicit, surface it during this phase.

## What to capture as context (for your future self)
When reviewing the codebase, explicitly note:

### 1) Intent and invariants
- What the system appears designed to do.
- Assumptions that are relied upon (ordering, timing, shapes, types, side effects).
- What must not change for the system to remain correct.

### 2) Behavioral contracts
- Inputs and outputs of major components.
- Side effects (I/O, state mutation, global effects).
- Error handling expectations.

### 3) Dependency and coupling map
- Tight vs loose coupling.
- Hidden dependencies.
- Modules that are transitively critical.

### 4) Sharp edges
- Code that is easy to break.
- Code that is hard to reason about.
- Code that has non-local effects.

### 5) Change sensitivity
- Areas likely to cause merge conflicts.
- Areas likely to cause behavioral drift.
- Areas safe for localized edits.

## How to record context (inside the chat)
Write findings directly into the chat using:
- Clear headings.
- Stable terminology (reuse names consistently).
- Explicit notes such as:
  - "Future-edit warning: ..."
  - "Invariant: ..."
  - "Unclear intent: ..."
  - "Do not change unless intentional: ..."

Treat this as internal documentation for later action.

## Forbidden during this phase
You must not:
- Suggest fixes.
- Draft refactors.
- Normalize small improvements.
- Plan edits without documenting the reasoning.
- Let implementation ideas influence interpretation.

If you notice a potential change:
- Record it as an observation.
- Defer judgment.

## Transition rule (critical)
You may only transition from context phase to change phase when:
- Major components and data flows are understood.
- Invariants and risks are explicitly recorded.
- You can articulate why each future change would be safe.
- Remaining unknowns are acknowledged.

If these conditions are not met, delay changes.

## Future-self constraint
When you later modify the codebase, you are bound by:
- The context you constructed here.
- The invariants you identified.
- The risks you flagged.

If a future change contradicts earlier context:
- Pause.
- Reconcile the discrepancy.
- Update the context explicitly.
- Never silently override your earlier understanding.

## Success criteria
This phase is successful when:
- You can explain the system without opening files again.
- You know where edits are safe vs dangerous.
- You trust your own understanding enough to make intentional changes.
- A reviewer can follow your reasoning from context to decision to change.
