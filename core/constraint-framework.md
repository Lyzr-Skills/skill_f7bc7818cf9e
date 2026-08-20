# Constraint Gating Framework (Stage 1)

Before scoring options, they must pass the Stage 1 Feasibility Gate.

## How it works:
1. Identify all hard constraints in the input (e.g., `max_budget`, `max_effort_hours`, `deadline_days`).
2. Evaluate each option's values against these hard limits.
3. If an option violates even *one* hard constraint, mark it as `INELIGIBLE` and set `eligible: false` with the violated constraint logged.
4. Do *not* calculate a Stage 2 decision score for ineligible options.

```
Option Proposed 
      ↓
Check Constraints (Budget, Engineering Capacity, Legal, Timeline)
      ↓
[Any Violations?]
   ├── YES ──> Mark INELIGIBLE (Skip Stage 2 Scoring)
   └── NO  ──> Mark ELIGIBLE (Proceed to Dominance Analysis)
```
