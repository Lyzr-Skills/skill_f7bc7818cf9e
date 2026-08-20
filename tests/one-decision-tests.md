# Test: One Decision Gate

Verify that the Decision Framework enforces the "One Decision" rule:
1. **Scenario 1**: Two options score similarly (e.g. A is 84, B is 83). The framework must NOT recommend choosing "A or B". It must choose one, justify the tie-breaker, and flag sensitivity robustness as LOW.
2. **Scenario 2**: Absolute lack of evidence. The framework must recommend `DEFERRED` and return a concrete next-action experiment. It must not list options as equal possibilities without choosing.
