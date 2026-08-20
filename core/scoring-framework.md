# Scoring Framework (Stage 2)

Only options passing Stage 1 gating enter Stage 2 scoring.

## Mathematical Formulation

$$\text{Base Score} = \text{Impact} \times \text{Confidence} \times \text{Strategic Alignment} \times \text{Learning Speed} \times \text{Reversibility}$$

Each dimension is scored $1$ to $10$.

## Penalties
Cost and Effort are subtracted as penalties:

$$\text{Final Score} = \text{Base Score} - (\text{Cost Penalty} \times W_{\text{cost}}) - (\text{Effort Penalty} \times W_{\text{effort}})$$

*Note: Weights and penalty calculations are configured inside `config/scoring.yaml` and `config/decision-profiles.yaml`.*
This avoids hardcoded rules in prompts and allows profiles like Growth or Exploration to scale weights dynamically.
