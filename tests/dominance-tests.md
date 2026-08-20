# Test: Dominance Analysis

Verify that dominated options are eliminated before scoring.

## Test Case 1: Dominated option
- Option A: Impact: 9, Confidence: 8, Cost: $1k, Effort: 20h
- Option B: Impact: 7, Confidence: 6, Cost: $2k, Effort: 40h
- **Expectation**: Option A strictly dominates Option B. Option B must be marked `DOMINATED_BY_OPTION_A` and eliminated immediately.
