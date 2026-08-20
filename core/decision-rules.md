# Decision Rules

Core rules guiding the engine's reasoning:

1. **The Reversibility Rule**:
   - If two options have similar expected value, prefer the option with higher reversibility and speed to learning.

2. **The Evidence Consistency Rule**:
   - "We think" must never be translated into "The data shows". Subjective thoughts are Hypotheses or Assumptions. Explicit data is Observed or Fact.

3. **No False Precision Rule**:
   - Scores with minute differences (e.g. 84 vs 83) must not be treated as distinct outcomes. They represent a close tie and must trigger Sensitivity Analysis to flag "Low Confidence".

4. **Strategic Guardrail Rule**:
   - High impact cannot override a "Low" Strategic Alignment score. Any option with Strategic Alignment < 3 (out of 10) must be flagged for manual review or penalization.
