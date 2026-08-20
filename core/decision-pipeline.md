# Decision Pipeline

This document defines the strict sequential pipeline for evaluating options.

```mermaid
graph TD
    Intake[1. Intake Question] --> Classification[2. Classification]
    Classification --> Validation[3. Option Validation]
    Validation --> Stage1[4. Stage 1 Constraint Gating]
    Stage1 --> Dominance[5. Dominance Analysis]
    Dominance --> Stage2[6. Stage 2 Criteria Scoring]
    Stage2 --> Tradeoff[7. Trade-off Analysis]
    Tradeoff --> Uncertainty[8. Uncertainty / Sensitivity Analysis]
    Uncertainty --> Selection[9. Recommendation Selection]
    Selection --> Output[10. Output Generation]
```

Every execution step MUST verify the prerequisites of the previous step. No skipping of steps is allowed.
If any step fails validation, the execution stops and reports a Quality Gate violation.
