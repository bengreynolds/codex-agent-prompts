# Release Readiness Workflow

## Purpose
Evaluate whether a release is ready, identify gaps, and define a clear go or no-go decision with mitigation steps.

## Inputs
- Release scope and changelog.
- Target environments and deployment plan.
- Test results and known issues.

## Constraints
- Do not approve release without verified evidence.
- Flag any missing test coverage or unclear rollback steps.
- Prefer explicit, measurable criteria.

## Steps
1. Define scope
   - List included features, fixes, and breaking changes.
   - Confirm what is explicitly out of scope.
2. Verify quality gates
   - Test pass rates, critical path coverage, and regression status.
   - Static analysis and lint status.
3. Validate operational readiness
   - Monitoring and alerting coverage.
   - Runbook or on-call guidance.
   - Rollback plan and recovery time expectations.
4. Assess risk
   - Identify high-risk changes and dependencies.
   - Classify overall risk (low, medium, high) with rationale.
5. Decide
   - Go or no-go with specific reasons.
   - Required follow-up actions if no-go.

## Output format
- Release scope summary.
- Quality gates status.
- Operational readiness checklist.
- Risks and mitigations.
- Go or no-go decision.

## Completion criteria
- All critical checks are evaluated.
- A clear decision is documented with rationale.
- Any blockers or follow-ups are explicit.
