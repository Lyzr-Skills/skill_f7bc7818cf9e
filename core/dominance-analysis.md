# Dominance Analysis

Before running scoring, check if any option is dominated.

## Rules:
Option A dominates Option B if:
1. $A$ is better than or equal to $B$ in *every* evaluation criterion (Impact, Confidence, Cost, Effort, Learning Speed, Reversibility, Strategic Alignment).
2. $A$ is strictly better than $B$ in at least *one* evaluation criterion.

## Action:
If Option A dominates Option B, Option B is flagged as `DOMINATED_BY_A` and eliminated from final selection. This prevents wasting calculation on sub-optimal choices and avoids false precision.
