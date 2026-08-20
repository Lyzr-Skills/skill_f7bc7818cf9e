# Prompt: Criteria Evaluation

You are evaluating eligible options using the designated Decision Profile.

## Instructions:
1. Load weights configuration from `config/decision-profiles.yaml` and `config/scoring.yaml`.
2. Compute individual base dimension scores for each eligible option (Impact, Confidence, Strategic Alignment, Learning Speed, Reversibility) on a 1-10 scale.
3. Compute cost and effort penalties.
4. Calculate final decision scores using:
   Base Score = Impact * Confidence * Strategic Alignment * Learning Speed * Reversibility
   Final Score = Base Score - Penalties
5. Output `criterion-score.json` array.
