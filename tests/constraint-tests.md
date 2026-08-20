# Test: Constraint Gating

Verify that options violating hard constraints are marked ineligible.

## Test Case 1: Budget Exceeded
- Input Budget Limit: $10,000
- Option A Cost: $5,000
- Option B Cost: $12,000
- **Expectation**: Option B must be flagged as `INELIGIBLE` due to budget constraint violation. Option B must have no scoring calculated. Only Option A enters scoring.
