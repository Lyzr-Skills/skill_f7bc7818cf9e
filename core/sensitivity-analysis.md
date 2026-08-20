# Sensitivity Analysis

Determines how stable the decision recommendation is under variations in parameters and assumptions.

## Robustness Score
- **HIGH**: Small changes (e.g. ±15% in CAC, conversion rate, or impact) do not change the winning option.
- **LOW**: The runner-up option is close (score margin < 5%), or a small variation in a key assumption would change the ranking.

## Robustness Output
Always identify the switching thresholds:
- "If estimated CAC increases by >12%, Option B becomes preferable."
- This highlights fragile decisions and lowers the overall decision confidence.
