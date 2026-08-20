# Configuration Guide

Configure evaluation weights and penalties inside `config/decision-profiles.yaml` and `config/scoring.yaml`.

## Profile Configurations
Create custom profiles under `decision-profiles.yaml`:
```yaml
custom_profile:
  impact: 0.30
  confidence: 0.20
  cost: 0.10
  effort: 0.10
  learning_speed: 0.10
  reversibility: 0.10
  strategic_alignment: 0.10
```
Use profiles to alter prioritization automatically based on the decision category.
