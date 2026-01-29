# Confirm Implementation Against Plan

## Purpose
Verify that implemented changes match the approved plan and task goals, and that nothing critical was missed or altered unintentionally.

## Inputs
- Task goal and success criteria.
- `agent.md` and `planning.md` (if present).
- Implemented changes (diffs, files, or commit range).
- Tests or verification results (if any).

## Constraints
- Focus on plan adherence and behavioral correctness.
- Do not approve changes if evidence is missing or incomplete.
- If plan or inputs are missing, request them before concluding.

## Steps
1. Restate the task and plan
   - Summarize the intended goal and planned steps.
   - Identify explicit constraints and out-of-scope items.
2. Compare implementation to plan
   - Map each planned change to actual edits.
   - Flag any missing steps or unexpected additions.
3. Validate outcomes
   - Check that success criteria are met.
   - Review tests or verification evidence.
4. Identify gaps and risks
   - Note unverified areas, regressions, or unresolved questions.
5. Decide
   - Confirm implementation or request fixes/clarifications.

## Output format
- Plan summary and constraints.
- Implementation-to-plan mapping.
- Verification evidence.
- Gaps, risks, or deviations.
- Confirmation or required follow-ups.

## Completion criteria
- Implementation aligns with the plan and task goals, or
- Deviations and missing evidence are documented with clear next steps.
