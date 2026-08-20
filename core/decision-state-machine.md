# Decision State Machine

Defines states and valid transitions during a decision lifecycle.

## States:
1. **DRAFT**: Intake phase.
2. **INTAKE_COMPLETE**: Questions and constraints defined.
3. **OPTIONS_VALIDATED**: At least two structured options.
4. **EVIDENCE_READY**: Evidence mapped and classified.
5. **EVALUATED**: Constraints checked, dominance verified, scoring complete.
6. **DECISION_READY**: Sensitivity and recommendation generated.
7. **DECIDED**: Decision Agent formally commits.
8. **EXECUTING**: Implementation of actions.
9. **REVIEW**: Evaluation trigger tripped.
10. **CLOSED**: Retrospective completed.

```
DRAFT -> INTAKE_COMPLETE -> OPTIONS_VALIDATED -> EVIDENCE_READY
       -> EVALUATED -> DECISION_READY -> DECIDED -> EXECUTING
       -> REVIEW -> CLOSED
```
