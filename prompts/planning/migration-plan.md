# Migration Plan

## Purpose
Design a safe, reversible plan for migrating systems, data, or infrastructure with minimal downtime and clear rollback.

## Inputs
- Source and target systems.
- Data shape and volume estimates.
- Cutover constraints and downtime tolerance.

## Constraints
- Preserve backward compatibility where required.
- Ensure rollback is possible at every phase.
- Avoid irreversible steps without explicit approval.

## Steps
1. Define scope and success criteria
   - What moves, what stays, and what changes.
   - Measurable success signals.
2. Inventory dependencies
   - Upstream and downstream systems.
   - Data producers and consumers.
3. Choose migration strategy
   - Big bang, phased, or dual-write.
   - Justify choice against risk and downtime.
4. Plan data movement
   - Data mapping and transformation rules.
   - Validation and reconciliation approach.
5. Plan cutover
   - Cutover sequence and timing.
   - Feature flags or traffic shifting.
6. Rollback plan
   - Clear rollback triggers.
   - Steps to restore previous state.
7. Validation and monitoring
   - Post-migration checks and metrics.
   - Alerting for anomalies.

## Output format
- Scope and success criteria.
- Migration strategy with rationale.
- Data movement plan.
- Cutover checklist.
- Rollback steps.
- Validation and monitoring plan.

## Completion criteria
- A phased, reversible plan is documented.
- Dependencies and risks are explicit.
- Rollback steps are concrete and feasible.
