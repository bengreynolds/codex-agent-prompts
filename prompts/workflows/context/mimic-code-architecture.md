# Mimic Existing Code Style and Architecture

## Purpose
Align new or modified code with an existing codebase's architecture, structure, naming conventions, organization, and syntax. This prompt prioritizes consistency and low-risk integration.

## Inputs
- Reference code or directories to model.
- Target files or areas for the new work.
- Any explicit style or architecture constraints (if known).

## Constraints
- Match the existing codebase conventions unless explicitly told to change them.
- Prefer the established architectural patterns and module boundaries.
- Do not introduce new patterns, dependencies, or naming schemes without approval.
- If reference code is missing, ask the user for it before proceeding.

## Steps
1. Identify reference patterns
   - Locate representative files that show the dominant style.
   - Note structure: directories, module layout, and file roles.
2. Extract conventions
   - Naming (files, functions, classes, variables, constants).
   - Formatting and syntax choices.
   - Error handling and logging conventions.
   - Dependency usage and import style.
3. Determine architectural fit
   - Identify where the change belongs.
   - Respect existing layers and boundaries.
4. Apply conventions to the task
   - Draft changes using the same patterns.
   - Keep changes minimal and consistent with neighbors.
5. Validate consistency
   - Compare against nearby code for alignment.
   - Flag any deviations that require approval.

## Output format
- Reference files used.
- Key conventions observed.
- Proposed placement and structure for the change.
- Notes on any deviations or open questions.

## Completion criteria
- The change plan aligns with existing style and architecture.
- Any required deviations are identified and explicitly called out.
