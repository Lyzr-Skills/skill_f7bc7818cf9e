# Architecture of Decision Framework

## Data Flow
```
Growth Experiment / GTM Strategy / Comp Intel
       ↓
Options, Evidence, Constraints & Context
       ↓
Decision Intake (Check Decision Clarity Gate)
       ↓
Option & Evidence Classification (Facts, Hypotheses, Assumptions)
       ↓
Constraint Gate (Stage 1 Feasibility Gate: Pass / Ineligible)
       ↓
Dominance Analysis (Filter out strictly dominated options)
       ↓
Criteria Scoring Engine (Stage 2 Configurable Scoring)
       ↓
Trade-off & Uncertainty Analysis
       ↓
Sensitivity & Robustness Analysis
       ↓
Selection (One Decision Rule)
       ↓
Decision Recommendation Output
       ↓
Decision Agent
```
This framework produces `decision-recommendation.json` as a structured proposal for the Decision Agent, which issues the final organizational decree and logs it into decision memory.
